# gh actions models
https://docs.github.com/en/github-models/integrating-ai-models-into-your-development-workflow
https://github.com/github/gh-models/blob/main/README.md
```
$ gh auth login
$ gh extension install https://github.com/github/gh-model
$ gh models help
GitHub Models CLI extension allows you to experiment with AI models from the command line.

To see a list of all available commands, run `gh models help`. To run the extension in
interactive mode, run `gh models run`. This will prompt you to select a model and then
enter a prompt. The extension will then return a response from the model.

For more information about what you can do with GitHub Models extension, see the manual
at https://github.com/github/gh-models/blob/main/README.md.

ℹ︎ Azure hosted. AI powered, can make mistakes. Not intended for production/sensitive data.
For more information, see https://github.com/github/gh-models

Usage:
  gh models [command]

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  help        Help about any command
  list        List available models
  run         Run inference with the specified model
  view        View details about a model

Flags:
  -h, --help   help for models

Use "gh models [command] --help" for more information about a command.
(swarms) swarmsefm@efm-ThinkPad-T580:~/git/swarms$ gh models help
GitHub Models CLI extension allows you to experiment with AI models from the command line.

To see a list of all available commands, run `gh models help`. To run the extension in
interactive mode, run `gh models run`. This will prompt you to select a model and then
enter a prompt. The extension will then return a response from the model.

For more information about what you can do with GitHub Models extension, see the manual
at https://github.com/github/gh-models/blob/main/README.md.

ℹ︎ Azure hosted. AI powered, can make mistakes. Not intended for production/sensitive data.
For more information, see https://github.com/github/gh-models

Usage:
  gh models [command]

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  help        Help about any command
  list        List available models
  run         Run inference with the specified model
  view        View details about a model

Flags:
  -h, --help   help for models

Use "gh models [command] --help" for more information about a command.
```

The models run on Azure:
```
$gh models list
Showing 32 available chat models

DISPLAY NAME                    MODEL NAME
AI21 Jamba 1.5 Large            AI21-Jamba-1.5-Large
AI21 Jamba 1.5 Mini             AI21-Jamba-1.5-Mini
Cohere Command R                Cohere-command-r
Cohere Command R 08-2024        Cohere-command-r-08-2024
Cohere Command R+               Cohere-command-r-plus
Cohere Command R+ 08-2024       Cohere-command-r-plus-08-2024
JAIS 30b Chat                   jais-30b-chat
Llama-3.2-11B-Vision-Instruct   Llama-3.2-11B-Vision-Instruct
Llama-3.2-90B-Vision-Instruct   Llama-3.2-90B-Vision-Instruct
Meta-Llama-3-70B-Instruct       Meta-Llama-3-70B-Instruct
Meta-Llama-3-8B-Instruct        Meta-Llama-3-8B-Instruct
Meta-Llama-3.1-405B-Instruct    Meta-Llama-3.1-405B-Instruct
Meta-Llama-3.1-70B-Instruct     Meta-Llama-3.1-70B-Instruct
Meta-Llama-3.1-8B-Instruct      Meta-Llama-3.1-8B-Instruct
Ministral 3B                    Ministral-3B
Mistral Large                   Mistral-large
Mistral Large (2407)            Mistral-large-2407
Mistral Nemo                    Mistral-Nemo
Mistral Small                   Mistral-small
OpenAI GPT-4o                   gpt-4o
OpenAI GPT-4o mini              gpt-4o-mini
OpenAI o1-mini                  o1-mini
OpenAI o1-preview               o1-preview
Phi-3-medium instruct (128k)    Phi-3-medium-128k-instruct
Phi-3-medium instruct (4k)      Phi-3-medium-4k-instruct
Phi-3-mini instruct (128k)      Phi-3-mini-128k-instruct
Phi-3-mini instruct (4k)        Phi-3-mini-4k-instruct
Phi-3-small instruct (128k)     Phi-3-small-128k-instruct
Phi-3-small instruct (8k)       Phi-3-small-8k-instruct
Phi-3.5-mini instruct (128k)    Phi-3.5-mini-instruct
Phi-3.5-MoE instruct (128k)     Phi-3.5-MoE-instruct
Phi-3.5-vision instruct (128k)  Phi-3.5-vision-instruct
```

There are 3 ui modes, chat, questions and provide context to question:
```
# chat with the model you select
$ gh models run  

# ask a question, get an answer
$ gh models run gpt-4o "why is the sky blue?"

# provide context, then ask question (max 8000 tokens)
$ cat README.md | gh models run gpt-4o "summarize this text"
$ head -c 8000 README.md | gh models run gpt-4o "summarize this text"
The text provides an overview of "Swarms," an enterprise-grade, production-ready multi-agent orchestration framework. It outlines the framework’s features, including enterprise architecture, agent orchestration, integration capabilities, scalability, developer tools, security features, advanced features, provider support, production features, and use case support. Swarms supports various providers like OpenAI and Anthropic and is designed for high reliability, modularity, and scalability. The text also includes links to social media, documentation, and installation guides, emphasizing the importance of Python version 3.10 or above, and setting environment variables for successful implementation.
```