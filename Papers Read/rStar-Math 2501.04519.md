# Paper Review: [rStar-Math 2501.04519]

## Quick Reference
- **Paper Link**: [https://arxiv.org/pdf/2501.04519]
- **Code/Resources**: [https://github.com/microsoft/rStar] 20250111 empty
- **Key Innovation**: [One sentence summary of main contribution]
- **Domain**: [math reasoning, small models]
- **Target Audience**: [Researchers]
- **Implementation Complexity**: [High/Medium/Low]
- **Computational Requirements**: [e.g., Enterprise GPU cluster, Single GPU, CPU only]

## Executive Summary
[2-3 sentences describing the key takeaways and practical implications]

## Problem Statement
- **Current Challenge**: [What problem does this paper address?]
- **Existing Solutions**: [Brief overview of current approaches]
- **Limitations Addressed**: [What limitations of current solutions does this work overcome?]

## Innovation Details
### Technical Contribution
- Key components:
  - [Component 1]
  - [Component 2]
  - [Component 3]

### Architecture/Method
[Diagram or description of the system architecture/method]

### Results
- **Benchmarks**: [Key performance metrics]
- **Improvements**: [Quantitative improvements over baselines]
- **Limitations**: [Noted limitations or constraints]

## Practical Applications
### Use Cases
- [Use Case 1]
- [Use Case 2]
- [Use Case 3]

### Implementation Considerations
- **Prerequisites**: [Required knowledge/technologies]
- **Resource Requirements**: [Hardware/software requirements]
- **Integration Points**: [How to integrate with existing systems]

## Critical Analysis
### Strengths
- [Strength 1]
- [Strength 2]
- [Strength 3]

### Weaknesses/Limitations
- [Weakness 1]
- [Weakness 2]
- [Weakness 3]

### Future Directions
- [Potential improvement 1]
- [Potential improvement 2]
- [Research opportunities]

## Business Impact Assessment
### Market Relevance
- **Industries**: [Relevant industries]
- **Timeline**: [When this could be practically implemented]
- **Cost-Benefit**: [Resource investment vs. potential returns]

### Implementation Strategy
1. [Step 1]
2. [Step 2]
3. [Step 3]

## Reference Implementation Notes
```python
# Key code snippets or pseudocode
def example_implementation():
    pass
```

## Follow-up Actions
- [ ] [Action item 1]
- [ ] [Action item 2]
- [ ] [Action item 3]

## Related Papers/Resources
- [Related work 1]
- [Related work 2]
- [Related work 3]

---
## Meta Information
- **Review Date**: [YYYY-MM-DD]
- **Reviewer**: [Name]
- **Time Spent**: [Hours]
- **Tags**: [#tag1, #tag2, #tag3]

--------------------------------------
Reading notes
"small language models (SLMs) can rival
or even surpass the math reasoning capability of OpenAI o1, without distillation
from superior models"
Small = phi-4 14B https://azure.microsoft.com/en-us/products/phi/ https://huggingface.co/collections/microsoft/phi-4-677e9380e514feb5577a40e4 https://ollama.com/library/phi4 

distillation = https://en.wikipedia.org/wiki/Knowledge_distillation 
  https://en.wikipedia.org/wiki/Soft-in_soft-out_decoder
  This paper doesn't use the learned logits of a larger model

"rStar-Math achieves this by exercising “deep thinking”
through Monte Carlo Tree Search (MCTS), where a math policy SLM performs
test-time search guided by an SLM-based process reward model."
  MCTS comes out of game playing and Reinforcement Learning via DeepMind. It is a stochastic (Random, Monte Carlo) Tree search, where branches that cannot lead to a good result are pruned to reduce the search space, leaving more compute resources available for searching deeper in the branches which are likely to lead to a good result. The tree search can use any modern tree search algorithm (Branch and Bound, Depth first, Breadth First, A*) - No, MCTC builds the tree incrementally and evaluates locally. This reduces memory requirements. https://www.geeksforgeeks.org/ml-monte-carlo-tree-search-mcts/

![[Screenshot from 2025-01-11 10-17-39.png]]

```python

# main function for the Monte Carlo Tree Search
def monte_carlo_tree_search(root):
	
	while resources_left(time, computational power):
		leaf = traverse(root) 
		simulation_result = rollout(leaf)
		backpropagate(leaf, simulation_result)
		
	return best_child(root)

# function for node traversal
def traverse(node):
	while fully_expanded(node):
		node = best_uct(node)
		
	# in case no children are present / node is terminal 
	return pick_unvisited(node.children) or node 

# function for the result of the simulation
def rollout(node):
	while non_terminal(node):
		node = rollout_policy(node)
	return result(node) 

# function for randomly selecting a child node
def rollout_policy(node):
	return pick_random(node.children)

# function for backpropagation
def backpropagate(node, result):
	if is_root(node) return
	node.stats = update_stats(node, result) 
	backpropagate(node.parent)

# function for selecting the best child
# node with highest number of visits
def best_child(node):
	pick child with highest number of visits
	
```

In rStar, two small language model agents are used.
The first, is a math policy search agent, which operates at test time, that is, to guide the search for a specific math problem.
The second, is a Process reward model agent, which guides the math policy search agent.

### math policy search

### process reward model PRM
a novel code-augmented CoT data sythesis method, which performs extensive
MCTS rollouts to generate step-by-step verified reasoning trajectories used to train
the policy SLM;
### process preference model PPM
a novel process reward model training method that avoids naïve
step-level score annotation, yielding a more effective process preference model
(PPM);
a novel method that trains an SLM acting as a process preference model, i.e., a PPM to
implement the desired PRM, that reliably predicts a reward label for each math reasoning step

### self-evolution recipe
a self-evolution recipe in which the policy SLM and PPM are built
from scratch and iteratively evolved to improve reasoning capabilities
![[Screenshot from 2025-01-11 10-25-25 1.png]]
Training with Step-by-Step Verified Reasoning Trajectory
Round 1: Bootstrapping an initial strong policy SLM-r1.
Round 2: Training a reliable PPM-r2
Round 3: PPM-augmented MCTS to significantly improve data quality.
Round 4: Solving challenging math problems

Key idea is that the problem space (math) is structured such, that it can be translated into a formal language (Python) which can be used to construct step-by-step verified reasoning (does this step follow logically from the prior step; is the program consistent with the problem statement at this step). Then this verified synthetic data is used to train a policy model for doing math. The policy model can be thought of as doing "I've seen a problem of this shape before, I used these logical moves to solve it, and I verified the answer with this different set of logical move.". The PPM is trained to reliably predict the reward of this reasoning step. "The PPM leverages the fact that, although Q-values are still not precise enough to score each reasoning step despite using extensive MCTS rollouts, the Q-values can reliably distinguish positive (correct) steps from negative (irrelevant/incorrect) ones.""
(Comment: that's interesting. You just need to avoid errors, irrelevant choices, to improve enough to be able  to succeed.)

PPM training: (step, good|bad) -> pairwise ranking loss
"Thus the training method constructs preference pairs
for each step based on Q-values and uses a pairwise ranking loss [Ouyang et al., 2022] to optimize
PPM’s score prediction for each reasoning step, achieving reliable labeling. This approach avoids
conventional methods that directly use Q-values as reward labels [Luo et al., 2024, Chen et al., 2024],
which are inherently noisy and imprecise in stepwise reward assignment."

pairwise ranking loss: https://gombru.github.io/2019/04/03/ranking_loss/
"Unlike other loss functions, such as Cross-Entropy Loss or Mean Square Error Loss, whose objective is to learn to predict directly a label, a value, or a set or values given an input, **the objective of Ranking Losses is to predict relative distances between inputs**. This task if often called **metric learning**."