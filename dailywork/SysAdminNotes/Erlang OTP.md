```shell
efm@efm-ThinkPad-T580:~$ erl
Command 'erl' not found, but can be installed with:
sudo snap install erlang       # version 25.3, or
sudo apt  install erlang-base  # version 1:25.3.2.8+dfsg-1ubuntu4.1
See 'snap info erlang' for additional versions.
efm@efm-ThinkPad-T580:~$ sudo snap install erlang
[sudo] password for efm: 
error: This revision of snap "erlang" was published using classic confinement
       and thus may perform arbitrary system changes outside of the security
       sandbox that snaps are usually confined to, which may put your system at
       risk.

       If you understand and want to proceed repeat the command including
       --classic.
efm@efm-ThinkPad-T580:~$ sudo snap install erlang --classic
erlang 25.3 from Tristan Sloughter (t-7) installed
efm@efm-ThinkPad-T580:~$ erl
Erlang/OTP 25 [erts-13.2] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:1] [jit:ns]

Eshell V13.2  (abort with ^G)
1> 2 + 5
1> .
7
2> 2 + 5.
7
3> (42 + 77) * 66 / 3.
2618.0
4> 
BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
p
=proc:<0.0.0>
State: Waiting
Name: init
Spawned as: erl_init:start/2
Spawned by: []
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 4
Link list: [<0.10.0>, <0.44.0>, <0.42.0>]
Reductions: 4742
Stack+heap: 987
OldHeap: 1598
Heap unused: 600
OldHeap unused: 1372
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 21608
Stack dump:
Program counter: 0x00007081bde0aaa0 (init:loop/1 + 80)
arity = 0
y(0)     {state,[{root,[<<"/snap/erlang/113/usr/bin/../lib/erlang">>]},{bindir,[<<"/snap/erlang/113/usr/bin/../lib/erlang/erts-13.2/bin">>]},{progname,[<<"erl">>]},{home,[<<"/home/efm">>]}],[],[],[{application_controller,<0.44.0>},{logger,<0.42.0>},{erl_prim_loader,<0.10.0>}],<0.9.0>,{started,started},{"Erlang/OTP","25"},[],[],#{},{"/home/efm","/snap/erlang/113/usr/bin/../lib/erlang/bin/start.boot"}}

0x00007081bc750988 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.1.0>
State: Waiting
Name: erts_code_purger
Spawned as: erts_code_purger:start/0
Current call: erlang:hibernate/3
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 9
Stack+heap: 4
OldHeap: 0
Heap unused: 4
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 808
Stack dump:
Program counter: 0x00007081bde01bc8 (unknown function)
arity = 3
   erts_code_purger
   wait_for_request
   []

0x00007082004041d8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_HIGH | USR_PRIO_HIGH | PRQ_PRIO_HIGH | OFF_HEAP_MSGQ
=proc:<0.2.0>
State: Waiting
Spawned as: erts_literal_area_collector:start/0
Current call: erlang:hibernate/3
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 8
Stack+heap: 4
OldHeap: 0
Heap unused: 4
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 808
Stack dump:
Program counter: 0x00007081bde01bc8 (unknown function)
arity = 3
   erts_literal_area_collector
   start
   []

0x00007081bc45a808 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_HIGH | USR_PRIO_HIGH | PRQ_PRIO_HIGH | OFF_HEAP_MSGQ
=proc:<0.3.0>
State: Waiting
Spawned as: erts_dirty_process_signal_handler:start/0
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 7
Stack+heap: 233
OldHeap: 0
Heap unused: 233
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2640
Stack dump:
Program counter: 0x00007081bde92750 (erts_dirty_process_signal_handler:msg_loop/0 + 80)
arity = 0
y(0)     []

0x00007081c02ceab8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL | OFF_HEAP_MSGQ
=proc:<0.4.0>
State: Waiting
Spawned as: erts_dirty_process_signal_handler:start/0
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 7
Stack+heap: 233
OldHeap: 0
Heap unused: 233
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2640
Stack dump:
Program counter: 0x00007081bde92750 (erts_dirty_process_signal_handler:msg_loop/0 + 80)
arity = 0
y(0)     []

0x00007081c02cf208 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_HIGH | USR_PRIO_HIGH | PRQ_PRIO_HIGH | OFF_HEAP_MSGQ
=proc:<0.5.0>
State: Waiting
Spawned as: erts_dirty_process_signal_handler:start/0
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 7
Stack+heap: 233
OldHeap: 0
Heap unused: 233
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2640
Stack dump:
Program counter: 0x00007081bde92750 (erts_dirty_process_signal_handler:msg_loop/0 + 80)
arity = 0
y(0)     []

0x00007081c02cf958 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_MAX | USR_PRIO_MAX | PRQ_PRIO_MAX | OFF_HEAP_MSGQ
=proc:<0.6.0>
State: Waiting
Spawned as: prim_file:start/0
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 6
Stack+heap: 233
OldHeap: 0
Heap unused: 233
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2640
Stack dump:
Program counter: 0x00007081bde3598c (prim_file:helper_loop/0 + 68)
arity = 0

0x00007081c0358900 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.7.0>
State: Waiting
Name: socket_registry
Spawned as: socket_registry:start/0
Spawned by: <0.0.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Reductions: 8
Stack+heap: 233
OldHeap: 0
Heap unused: 233
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2640
Stack dump:
Program counter: 0x00007081bde454dc (socket_registry:loop/1 + 92)
arity = 0
y(0)     []
y(1)     []
y(2)     {state,#{},#{},#{}}

0x00007081c0359050 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.10.0>
State: Waiting
Name: erl_prim_loader
Spawned as: erlang:apply/2
Spawned by: <0.9.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.0.0>]
Reductions: 56680
Stack+heap: 2586
OldHeap: 28690
Heap unused: 815
OldHeap unused: 28446
BinVHeap: 98622
OldBinVHeap: 0
BinVHeap unused: 22905
OldBinVHeap unused: 46422
Memory: 251104
Stack dump:
Program counter: 0x00007081bde61e34 (erl_prim_loader:loop/3 + 116)
arity = 0
y(0)     []
y(1)     360000
y(2)     ["/snap/erlang/113/usr/bin/../lib/erlang/lib/kernel-8.5.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/stdlib-4.3/ebin"]
y(3)     <0.9.0>
y(4)     {state,efile,[],noport,360000,{prim_state,false,undefined}}

0x00007081bc4cfb08 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.42.0>
State: Waiting
Name: logger
Spawned as: proc_lib:init_p/5
Spawned by: <0.9.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.0.0>]
Dictionary: [{'$logger_cb_process',true},{'$ancestors',[<0.9.0>]},{'$initial_call',{logger_server,init,1}}]
Reductions: 642
Stack+heap: 987
OldHeap: 376
Heap unused: 575
OldHeap unused: 352
BinVHeap: 88
OldBinVHeap: 4
BinVHeap unused: 46334
OldBinVHeap unused: 46418
Memory: 11888
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     logger_server
y(3)     {state,#Ref<0.1867266066.399638531.123667>,undefined,{[],[]},undefined}
y(4)     logger
y(5)     <0.9.0>

0x00007081bc7338a0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc7338c0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.44.0>
State: Waiting
Name: application_controller
Spawned as: erlang:apply/2
Spawned by: <0.9.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 4
Link list: [<0.0.0>, <0.46.0>]
Dictionary: [{'$ancestors',[<0.9.0>]},{'$initial_call',{application_controller,start,1}}]
Reductions: 789
Stack+heap: 2586
OldHeap: 2586
Heap unused: 2112
OldHeap unused: 2578
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 42432
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     application_controller
y(3)     {state,[],[],[],[{stdlib,undefined},{kernel,<0.46.0>}],[],[{stdlib,permanent},{kernel,permanent}],[],[]}
y(4)     application_controller
y(5)     <0.9.0>

0x00007081bc738998 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.46.0>
State: Waiting
Spawned as: proc_lib:init_p/5
Spawned by: <0.45.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.44.0>, <0.47.0>]
Dictionary: [{'$ancestors',[<0.45.0>]},{'$initial_call',{application_master,init,4}}]
Reductions: 40
Stack+heap: 376
OldHeap: 0
Heap unused: 33
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 3952
Stack dump:
Program counter: 0x00007081bdec520c (application_master:main_loop/2 + 84)
arity = 0
y(0)     {state,<0.47.0>,{appl_data,kernel,[application_controller,erl_reply,auth,boot_server,code_server,disk_log_server,disk_log_sup,erl_prim_loader,error_logger,file_server_2,fixtable_server,global_group,global_name_server,heart,init,kernel_config,kernel_refc,kernel_sup,logger,logger_handler_watcher,logger_sup,net_kernel,net_sup,rex,user,os_server,ddll_server,erl_epmd,inet_db,pg],undefined,{kernel,[]},[application,application_controller,application_master,application_starter,auth,code,code_server,dist_util,erl_boot_server,erl_compile_server,erl_distribution,erl_erts_errors,erl_reply,erl_kernel_errors,erl_signal_handler,erpc,error_handler,error_logger,file,file_server,file_io_server,global,global_group,global_search,group,group_history,heart,inet6_tcp,inet6_tcp_dist,inet6_udp,inet6_sctp,inet_config,inet_hosts,inet_gethost_native,inet_tcp_dist,kernel,kernel_config,kernel_refc,local_tcp,local_udp,logger,logger_backend,logger_config,logger_disk_log_h,logger_filters,logger_formatter,logger_h_common,logger_handler_watcher,logger_olp,logger_proxy,logger_server,logger_simple_h,logger_std_h,logger_sup,net,net_adm,net_kernel,os,ram_file,rpc,user,user_drv,user_sup,disk_log,disk_log_1,disk_log_server,disk_log_sup,dist_ac,erl_ddll,erl_epmd,erts_debug,gen_tcp,gen_tcp_socket,gen_udp,gen_udp_socket,gen_sctp,inet,inet_db,inet_dns,inet_parse,inet_res,inet_tcp,inet_udp,inet_sctp,pg,pg2,raw_file_io,raw_file_io_compressed,raw_file_io_deflate,raw_file_io_delayed,raw_file_io_inflate,raw_file_io_list,seq_trace,socket,standard_error,wrap_log_reader],infinity,infinity},[],0,init,[]}
y(1)     <0.44.0>

0x00007081bc70efa0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc70efc0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.47.0>
State: Waiting
Spawned as: application_master:start_it/4
Spawned by: <0.46.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>, <0.46.0>]
Reductions: 507
Stack+heap: 233
OldHeap: 376
Heap unused: 201
OldHeap unused: 370
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 5728
Stack dump:
Program counter: 0x00007081bdec724c (application_master:loop_it/4 + 108)
arity = 0
y(0)     []
y(1)     []
y(2)     kernel
y(3)     <0.49.0>
y(4)     <0.46.0>

0x00007081bc706128 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.49.0>
State: Waiting
Name: kernel_sup
Spawned as: proc_lib:init_p/5
Spawned by: <0.47.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.47.0>, <0.51.0>, <0.50.0>, <0.55.0>, <0.60.0>, <0.58.0>, <0.62.0>, <0.68.0>, <0.71.0>, <0.70.0>, <0.69.0>, <0.64.0>, <0.61.0>, <0.53.0>]
Dictionary: [{'$ancestors',[<0.47.0>]},{'$initial_call',{supervisor,kernel,1}}]
Reductions: 3107
Stack+heap: 1598
OldHeap: 376
Heap unused: 768
OldHeap unused: 105
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 17216
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     supervisor
y(3)     {state,{local,kernel_sup},one_for_all,{[logger_sup,kernel_safe_sup,kernel_refc,kernel_config,user,standard_error,erl_signal_server,file_server_2,global_group,net_sup,global_name_server,rex,inet_db,code_server],#{code_server=>{child,<0.50.0>,code_server,{code,start_link,[]},permanent,false,2000,worker,[code]},erl_signal_server=>{child,<0.61.0>,erl_signal_server,{gen_event,start_link,[{local,erl_signal_server}]},permanent,false,2000,worker,dynamic},file_server_2=>{child,<0.60.0>,file_server_2,{file_server,start_link,[]},permanent,false,2000,worker,[file,file_server,file_io_server,prim_file]},global_group=>{child,<0.58.0>,global_group,{global_group,start_link,[]},permanent,false,2000,worker,[global_group]},global_name_server=>{child,<0.55.0>,global_name_server,{global,start_link,[]},permanent,false,2000,worker,[global]},inet_db=>{child,<0.51.0>,inet_db,{inet_db,start_link,[]},permanent,false,2000,worker,[inet_db]},kernel_config=>{child,<0.68.0>,kernel_config,{kernel_config,start_link,[]},permanent,false,2000,worker,[kernel_config]},kernel_refc=>{child,<0.69.0>,kernel_refc,{kernel_refc,start_link,[]},permanent,false,2000,worker,[kernel_refc]},kernel_safe_sup=>{child,<0.70.0>,kernel_safe_sup,{supervisor,start_link,[{local,kernel_safe_sup},kernel,safe]},permanent,false,infinity,supervisor,[kernel]},logger_sup=>{child,<0.71.0>,logger_sup,{logger_sup,start_link,[]},permanent,false,infinity,supervisor,[logger_sup]},net_sup=>{child,undefined,net_sup,{erl_distribution,start_link,[]},permanent,false,infinity,supervisor,[erl_distribution]},rex=>{child,<0.53.0>,rex,{rpc,start_link,[]},permanent,false,2000,worker,[rpc]},standard_error=>{child,<0.62.0>,standard_error,{standard_error,start_link,[]},temporary,false,2000,supervisor,[standard_error]},user=>{child,<0.64.0>,user,{user_sup,start,[]},temporary,false,2000,supervisor,[user_sup]}}},undefined,0,1,[],0,never,kernel,[]}
y(4)     kernel_sup
y(5)     <0.47.0>

0x00007081bc74b890 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc74b8b0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.50.0>
State: Waiting
Name: code_server
Spawned as: erlang:apply/2
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>]
Reductions: 114416
Stack+heap: 2586
OldHeap: 17731
Heap unused: 1160
OldHeap unused: 4084
BinVHeap: 98765
OldBinVHeap: 4
BinVHeap unused: 22762
OldBinVHeap unused: 46418
Memory: 163432
Stack dump:
Program counter: 0x00007081bdede798 (code_server:loop/1 + 128)
arity = 0
y(0)     []
y(1)     <0.49.0>
y(2)     {state,<0.49.0>,"/snap/erlang/113/usr/bin/../lib/erlang",[".","/snap/erlang/113/usr/bin/../lib/erlang/lib/kernel-8.5.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/stdlib-4.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/xmerl-1.3.31/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/wx-2.2.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/tools-3.5.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/tftp-1.0.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/syntax_tools-3.0.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/ssl-10.9/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/ssh-4.15.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/snmp-5.13.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/sasl-4.2/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/runtime_tools-1.19/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/reltool-0.9.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/public_key-1.13.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/parsetools-2.4.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/os_mon-2.8.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/observer-2.14/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/mnesia-4.21.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/megaco-4.4.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/inets-8.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/ftp-1.1.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/eunit-2.8.2/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/et-1.6.5/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/erts-13.2/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/erl_interface-5.3.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/erl_docgen-1.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/eldap-1.2.10/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/edoc-1.2/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/diameter-2.2.7/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/dialyzer-5.0.5/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/debugger-5.3.1/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/crypto-5.1.3/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/compiler-8.2.4/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/common_test-1.24/ebin","/snap/erlang/113/usr/bin/../lib/erlang/lib/asn1-5.0.21/ebin"],#Ref<0.1867266066.399638531.123711>,code_names,interactive,[]}

0x00007081bc452ae8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.51.0>
State: Waiting
Name: inet_db
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{inet_db,init,1}}]
Reductions: 373
Stack+heap: 376
OldHeap: 0
Heap unused: 100
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 3992
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     inet_db
y(3)     {state,inet_db,inet_cache,inet_hosts_byname,inet_hosts_byaddr,inet_hosts_file_byname,inet_hosts_file_byaddr,inet_sockets,#Ref<0.1867266066.399507459.123730>}
y(4)     inet_db
y(5)     <0.49.0>

0x00007081bc70c970 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc70c990 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.53.0>
State: Waiting
Name: rex
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>, {to,<0.54.0>,#Ref<0.1867266066.399507459.123752>}]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{rpc,init,1}}]
Reductions: 35
Stack+heap: 233
OldHeap: 0
Heap unused: 165
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2832
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     rpc
y(3)     #{nodes_observer=>{<0.54.0>,#Ref<0.1867266066.399507459.123752>}}
y(4)     rex
y(5)     <0.49.0>

0x00007081bc70d0c0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc70d0e0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL | OFF_HEAP_MSGQ
=proc:<0.54.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.53.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [{from,<0.53.0>,#Ref<0.1867266066.399507459.123752>}]
Reductions: 47
Stack+heap: 233
OldHeap: 0
Heap unused: 192
OldHeap unused: 0
BinVHeap: 24
OldBinVHeap: 0
BinVHeap unused: 46398
OldBinVHeap unused: 46422
Memory: 2844
Stack dump:
Program counter: 0x00007081be0c8cc8 (rpc:nodes_observer_loop/1 + 96)
arity = 0
y(0)     []
y(1)     #Ref<0.1867266066.399638531.123753>
y(2)     []

0x00007081bc7059d8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_HIGH | USR_PRIO_HIGH | PRQ_PRIO_HIGH | MAYBE_SELF_SIGS
=proc:<0.55.0>
State: Waiting
Name: global_name_server
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 1
Heap fragment data: 4
Link list: [<0.49.0>, <0.57.0>, <0.56.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{global,init,1}},{creation_extension,1117981915589115904},{rand_seed,{#{bits=>58,jump=>#Fun<rand.3.34006561>,next=>#Fun<rand.0.34006561>,type=>exsss,uniform=>#Fun<rand.1.34006561>,uniform_n=>#Fun<rand.2.34006561>},[270203173280664854|82607594423879392]}}]
Reductions: 243
Stack+heap: 376
OldHeap: 376
Heap unused: 291
OldHeap unused: 336
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 7172
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     global
y(3)     {state,{conf,true,true},#{},[],[],[],'nonode@nohost',<0.56.0>,<0.57.0>,no_trace,false}
y(4)     global_name_server
y(5)     <0.49.0>

0x00007081bc754738 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc754758 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.56.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.55.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.55.0>]
Reductions: 41
Stack+heap: 233
OldHeap: 0
Heap unused: 169
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2680
Stack dump:
Program counter: 0x00007081be0dc904 (global:loop_the_locker/1 + 524)
arity = 0
y(0)     infinity
y(1)     {multi,[],[],[],'nonode@nohost',false,false}

0x00007081bc7510d8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.57.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.55.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.55.0>]
Reductions: 7
Stack+heap: 233
OldHeap: 0
Heap unused: 226
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2680
Stack dump:
Program counter: 0x00007081be0e48b8 (global:loop_the_registrar/0 + 80)
arity = 0
y(0)     []

0x00007081bc751828 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.58.0>
State: Waiting
Name: global_group
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.59.0>, <0.49.0>]
Dictionary: [{global_group_check,<0.59.0>},{registered_names,[undefined]},{'$ancestors',[kernel_sup,<0.47.0>]},{send,[undefined]},{'$initial_call',{global_group,init,1}},{whereis_name,[undefined]}]
Reductions: 78
Stack+heap: 233
OldHeap: 0
Heap unused: 103
OldHeap unused: 0
BinVHeap: 20
OldBinVHeap: 0
BinVHeap unused: 46402
OldBinVHeap unused: 46422
Memory: 2868
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     global_group
y(3)     {state,no_conf,[],#{},[],[],normal,#{},#{},undefined}
y(4)     global_group
y(5)     <0.49.0>

0x00007081bc752fa0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc752fc0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_MAX | USR_PRIO_MAX | PRQ_PRIO_MAX
=proc:<0.59.0>
State: Waiting
Name: global_group_check
Spawned as: erlang:apply/2
Spawned by: <0.58.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.58.0>]
Reductions: 6
Stack+heap: 233
OldHeap: 0
Heap unused: 226
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2680
Stack dump:
Program counter: 0x00007081be125544 (global_group:global_group_check_dispatcher/0 + 68)
arity = 0

0x00007081bc707590 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.60.0>
State: Waiting
Name: file_server_2
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 4
Link list: [<0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{file_server,init,1}}]
Reductions: 136
Stack+heap: 376
OldHeap: 0
Heap unused: 235
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 4024
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     file_server
y(3)     undefined
y(4)     file_server_2
y(5)     <0.49.0>

0x00007081bc75b9c8 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc75b9e8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.61.0>
State: Waiting
Name: erl_signal_server
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{gen_event,init_it,6}}]
Reductions: 48
Stack+heap: 233
OldHeap: 0
Heap unused: 157
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2768
Stack dump:
Program counter: 0x00007081bdf6e550 (gen_event:fetch_msg/6 + 112)
arity = 0
y(0)     false
y(1)     []
y(2)     infinity
y(3)     [{handler,erl_signal_handler,false,{state},false}]
y(4)     erl_signal_server
y(5)     <0.49.0>

0x00007081bc75d8a8 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc75d8c8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.62.0>
State: Waiting
Name: standard_error_sup
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.63.0>, <0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{supervisor_bridge,standard_error,1}}]
Reductions: 51
Stack+heap: 233
OldHeap: 0
Heap unused: 149
OldHeap unused: 0
BinVHeap: 20
OldBinVHeap: 0
BinVHeap unused: 46402
OldBinVHeap unused: 46422
Memory: 2808
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     supervisor_bridge
y(3)     {state,standard_error,<0.63.0>,<0.63.0>,{local,standard_error_sup}}
y(4)     standard_error_sup
y(5)     <0.49.0>

0x00007081bc708738 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc708758 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.63.0>
State: Waiting
Name: standard_error
Spawned as: erlang:apply/2
Spawned by: <0.62.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [#Port<0.3>, <0.62.0>]
Dictionary: [{encoding,latin1}]
Reductions: 14
Stack+heap: 233
OldHeap: 0
Heap unused: 222
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2808
Stack dump:
Program counter: 0x00007081be136d58 (standard_error:server_loop/1 + 80)
arity = 0
y(0)     #Port<0.3>

0x00007081bc708ea8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.64.0>
State: Waiting
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.66.0>, <0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{supervisor_bridge,user_sup,1}}]
Reductions: 93
Stack+heap: 233
OldHeap: 0
Heap unused: 146
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2808
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     supervisor_bridge
y(3)     {state,user_sup,<0.66.0>,<0.66.0>,{<0.64.0>,user_sup}}
y(4)     <0.64.0>
y(5)     <0.49.0>

0x00007081bc70a4b0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc70a4d0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.65.0>
State: Waiting
Name: user_drv
Spawned as: user_drv:server/2
Spawned by: <0.64.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.66.0>, #Port<0.4>, <0.67.0>]
Dictionary: [{eof,false},{current_group,<0.67.0>}]
Reductions: 4381
Stack+heap: 987
OldHeap: 610
Heap unused: 350
OldHeap unused: 396
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 13760
Stack dump:
Program counter: 0x00007081be13f8d4 (user_drv:server_loop/6 + 124)
arity = 0
y(0)     []
y(1)     []
y(2)     {false,{[],[]}}
y(3)     {2,1,<0.67.0>,[{0,<0.66.0>,{}},{1,<0.67.0>,{shell,start,[init]}}]}
y(4)     <0.66.0>
y(5)     <0.67.0>
y(6)     #Port<0.4>
y(7)     #Port<0.4>

0x00007081bc442090 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.66.0>
State: Waiting
Name: user
Spawned as: group:server/3
Spawned by: <0.65.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.64.0>, <0.65.0>]
Dictionary: [{echo,true},{line_buffer,[]},{expand_fun,#Fun<group.0.126211949>},{read_mode,list},{user_drv,<0.65.0>},{kill_buffer,[]}]
Reductions: 100
Stack+heap: 233
OldHeap: 0
Heap unused: 139
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2808
Stack dump:
Program counter: 0x00007081be146b94 (group:server_loop/3 + 92)
arity = 0
y(0)     []
y(1)     undefined
y(2)     <0.65.0>

0x00007081bc7095f8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.67.0>
State: Waiting
Spawned as: group:server/3
Spawned by: <0.65.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.75.0>, <0.65.0>, {from,<0.86.0>,#Ref<0.1867266066.399507459.123906>}]
Dictionary: [{line_buffer,["(42 + 77) * 66 / 3.\n","2 + 5.\n",".\n","2 + 5\n"]},{shell,<0.75.0>},{echo,true},{expand_fun,#Fun<group.0.126211949>},{read_mode,list},{user_drv,<0.65.0>},{kill_buffer,[]}]
Reductions: 3098
Stack+heap: 610
OldHeap: 610
Heap unused: 476
OldHeap unused: 406
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 10768
Stack dump:
Program counter: 0x00007081be14bf6c (group:more_data/6 + 132)
arity = 0
y(0)     infinity
y(1)     unicode
y(2)     {stack,["(42 + 77) * 66 / 3.\n","2 + 5.\n",".\n","2 + 5\n"],{},[]}
y(3)     <0.75.0>
y(4)     <0.65.0>
y(5)     {line,"4> ",{[],[]},none}
y(6)     more_chars

0x00007081bc45a2f0 Return addr 0x00007081be14a038 (group:get_chars_loop/9 + 216)
y(0)     unicode
y(1)     start
y(2)     <0.75.0>
y(3)     <0.65.0>
y(4)     {erl_scan,tokens,[{1,1},[text,{reserved_word_fun,fun erl_scan:reserved_word/1}]]}
y(5)     get_until
y(6)     "4> "

0x00007081bc45a330 Return addr 0x00007081be147900 (group:io_request/6 + 160)
y(0)     []
y(1)     #Ref<0.1867266066.399507459.123906>
y(2)     <0.86.0>

0x00007081bc45a350 Return addr 0x00007081be146c84 (group:server_loop/3 + 332)
y(0)     <0.75.0>
y(1)     <0.65.0>

0x00007081bc45a368 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.68.0>
State: Waiting
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{kernel_config,init,1}}]
Reductions: 52
Stack+heap: 233
OldHeap: 0
Heap unused: 167
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2768
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     kernel_config
y(3)     []
y(4)     <0.68.0>
y(5)     <0.49.0>

0x00007081bc70ac00 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc70ac20 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.69.0>
State: Waiting
Name: kernel_refc
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 3
Link list: [<0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{kernel_refc,init,1}}]
Reductions: 46
Stack+heap: 233
OldHeap: 0
Heap unused: 173
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2792
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     kernel_refc
y(3)     #{scheduler_wall_time=>#{}}
y(4)     kernel_refc
y(5)     <0.49.0>

0x00007081bc756d68 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc756d88 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.70.0>
State: Waiting
Name: kernel_safe_sup
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{supervisor,kernel,1}}]
Reductions: 93
Stack+heap: 233
OldHeap: 0
Heap unused: 70
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2768
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     supervisor
y(3)     {state,{local,kernel_safe_sup},one_for_one,{[],#{}},undefined,4,3600,[],0,never,kernel,safe}
y(4)     kernel_safe_sup
y(5)     <0.49.0>

0x00007081bc7574b8 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc7574d8 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.71.0>
State: Waiting
Name: logger_sup
Spawned as: proc_lib:init_p/5
Spawned by: <0.49.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.49.0>, <0.76.0>, <0.73.0>, <0.72.0>]
Dictionary: [{'$ancestors',[kernel_sup,<0.47.0>]},{'$initial_call',{supervisor,logger_sup,1}}]
Reductions: 407
Stack+heap: 610
OldHeap: 376
Heap unused: 378
OldHeap unused: 319
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 8912
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     supervisor
y(3)     {state,{local,logger_sup},one_for_one,{[default,logger_proxy,logger_handler_watcher],#{default=>{child,<0.76.0>,default,{logger_olp,start_link,undefined},temporary,false,2000,worker,[logger_h_common]},logger_handler_watcher=>{child,<0.72.0>,logger_handler_watcher,{logger_handler_watcher,start_link,[]},permanent,false,brutal_kill,worker,[logger_handler_watcher]},logger_proxy=>{child,<0.73.0>,logger_proxy,{logger_proxy,start_link,[]},temporary,false,2000,worker,[logger_proxy]}}},undefined,1,5,[],0,never,logger_sup,[]}
y(4)     logger_sup
y(5)     <0.49.0>

0x00007081bc7319c0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc7319e0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.72.0>
State: Waiting
Name: logger_handler_watcher
Spawned as: proc_lib:init_p/5
Spawned by: <0.71.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.71.0>, {to,<0.76.0>,#Ref<0.1867266066.399507459.123835>}]
Dictionary: [{'$ancestors',[logger_sup,kernel_sup,<0.47.0>]},{'$initial_call',{logger_handler_watcher,init,1}}]
Reductions: 52
Stack+heap: 233
OldHeap: 0
Heap unused: 145
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2832
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     logger_handler_watcher
y(3)     {state,[{default,#Ref<0.1867266066.399507459.123835>}]}
y(4)     logger_handler_watcher
y(5)     <0.71.0>

0x00007081bc757c08 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc757c28 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.73.0>
State: Waiting
Name: logger_proxy
Spawned as: proc_lib:init_p/5
Spawned by: <0.71.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.71.0>]
Dictionary: [{'$ancestors',[logger_sup,kernel_sup,<0.47.0>]},{'$initial_call',{logger_olp,init,1}},{olp_ref,{logger_proxy,<0.73.0>,{logger_olp,logger_proxy}}}]
Reductions: 89
Stack+heap: 376
OldHeap: 0
Heap unused: 232
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 3912
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     logger_olp
y(3)     #{burst_limit_enable=>false,burst_limit_max_count=>500,burst_limit_window_time=>1000,burst_msg_count=>0,burst_win_ts=>-576460751474932,cb_state=>no_state,drop_mode_qlen=>1000,flush_qlen=>5000,id=>logger_proxy,idle=>true,last_load_ts=>-576460751474932,last_qlen=>0,mode=>async,mode_ref=>{logger_olp,logger_proxy},module=>logger_proxy,overload_kill_enable=>false,overload_kill_mem_size=>3000000,overload_kill_qlen=>20000,overload_kill_restart_after=>5000,sync_mode_qlen=>500}
y(4)     <0.73.0>
y(5)     <0.71.0>

0x00007081bc75a6b0 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc75a6d0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL | OFF_HEAP_MSGQ
=proc:<0.75.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.67.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 128
Link list: [<0.67.0>, <0.86.0>, <0.82.0>]
Dictionary: [{{result,1},7},{{result,3},2.618000e+03},{{command,1},[{op,{1,3},'+',{integer,{1,1},2},{integer,{1,5},5}}]},{{result,2},7},{evaluator,<0.82.0>},{{command,3},[{op,{1,16},'/',{op,{1,11},'*',{op,{1,5},'+',{integer,{1,2},42},{integer,{1,7},77}},{integer,{1,13},66}},{integer,{1,18},3}}]},{{command,2},[{op,{1,3},'+',{integer,{1,1},2},{integer,{1,5},5}}]}]
Reductions: 20720
Stack+heap: 28690
OldHeap: 0
Heap unused: 2676
OldHeap unused: 0
BinVHeap: 1227
OldBinVHeap: 0
BinVHeap unused: 45195
OldBinVHeap unused: 46422
Memory: 231608
Stack dump:
Program counter: 0x00007081be181aac (shell:get_command1/5 + 108)
arity = 0
y(0)     []
y(1)     #Ref<0.1867266066.399638531.123867>
y(2)     []
y(3)     <0.82.0>
y(4)     <0.86.0>

0x00007081bc492948 Return addr 0x00007081be1811f4 (shell:server_loop/7 + 236)
y(0)     []
y(1)     []
y(2)     []
y(3)     []
y(4)     4
y(5)     20
y(6)     20
y(7)     #Ref<0.1867266066.399638531.123867>
y(8)     3

0x00007081bc492998 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.76.0>
State: Waiting
Name: logger_std_h_default
Spawned as: proc_lib:init_p/5
Spawned by: <0.71.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 13
Link list: [<0.77.0>, <0.71.0>, {from,<0.72.0>,#Ref<0.1867266066.399507459.123835>}]
Dictionary: [{'$ancestors',[logger_sup,kernel_sup,<0.47.0>]},{'$initial_call',{logger_olp,init,1}},{olp_ref,{logger_std_h_default,<0.76.0>,{logger_olp,logger_std_h_default}}}]
Reductions: 165
Stack+heap: 376
OldHeap: 0
Heap unused: 29
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 4120
Stack dump:
Program counter: 0x00007081bdf53f54 (gen_server:loop/7 + 596)
arity = 0
y(0)     []
y(1)     infinity
y(2)     logger_olp
y(3)     #{burst_limit_enable=>true,burst_limit_max_count=>500,burst_limit_window_time=>1000,burst_msg_count=>0,burst_win_ts=>-576460751392443,cb_state=>#{ctrl_sync_count=>20,filesync_repeat_interval=>no_repeat,handler_state=>#{file_ctrl_pid=><0.77.0>,type=>standard_io},id=>default,last_op=>sync,module=>logger_std_h},drop_mode_qlen=>200,flush_qlen=>1000,id=>logger_std_h_default,idle=>true,last_load_ts=>-576460751392443,last_qlen=>0,mode=>async,mode_ref=>{logger_olp,logger_std_h_default},module=>logger_h_common,overload_kill_enable=>false,overload_kill_mem_size=>3000000,overload_kill_qlen=>20000,overload_kill_restart_after=>5000,sync_mode_qlen=>10}
y(4)     <0.76.0>
y(5)     <0.71.0>

0x00007081bc75c590 Return addr 0x00007081bdf615a0 (proc_lib:init_p_do_apply/3 + 192)
y(0)     []
y(1)     []
y(2)     Catch 0x00007081bdf615be (proc_lib:init_p_do_apply/3 + 222)

0x00007081bc75c5b0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL | OFF_HEAP_MSGQ
=proc:<0.77.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.76.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.76.0>]
Reductions: 9
Stack+heap: 233
OldHeap: 0
Heap unused: 209
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2680
Stack dump:
Program counter: 0x00007081be19776c (logger_std_h:file_ctrl_loop/1 + 92)
arity = 0
y(0)     []
y(1)     []
y(2)     #{dev=>standard_io,handler_name=>default}

0x00007081bc759690 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.82.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.75.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.75.0>]
Reductions: 3504
Stack+heap: 610
OldHeap: 610
Heap unused: 475
OldHeap unused: 169
BinVHeap: 0
OldBinVHeap: 4
BinVHeap unused: 46422
OldBinVHeap unused: 46418
Memory: 10576
Stack dump:
Program counter: 0x00007081be1868dc (shell:eval_loop/3 + 108)
arity = 0
y(0)     []
y(1)     []
y(2)     []
y(3)     #Ref<0.1867266066.399638531.123867>
y(4)     []
y(5)     <0.75.0>

0x00007081bc455ce0 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=proc:<0.86.0>
State: Waiting
Spawned as: erlang:apply/2
Spawned by: <0.75.0>
Message queue length: 0
Number of heap fragments: 0
Heap fragment data: 0
Link list: [<0.75.0>, {to,<0.67.0>,#Ref<0.1867266066.399507459.123906>}]
Reductions: 17
Stack+heap: 233
OldHeap: 0
Heap unused: 195
OldHeap unused: 0
BinVHeap: 0
OldBinVHeap: 0
BinVHeap unused: 46422
OldBinVHeap unused: 46422
Memory: 2744
Stack dump:
Program counter: 0x00007081be1d2808 (io:execute_request/3 + 504)
arity = 0
y(0)     #Ref<0.1867266066.399507459.123906>
y(1)     error
y(2)     {false,{get_until,unicode,["4",62,32],erl_scan,tokens,[{1,1},[text,{reserved_word_fun,fun erl_scan:reserved_word/1}]]}}
y(3)     <0.67.0>

0x00007081bc456418 Return addr 0x00007081be191fc8 (shell:'-get_command/5-fun-0-'/1 + 184)
y(0)     []
y(1)     []

0x00007081bc456430 Return addr 0x00007081bde01c50 (<terminate process normally>)
Internal State: ACT_PRIO_NORMAL | USR_PRIO_NORMAL | PRQ_PRIO_NORMAL
=port:#Port<0.0>
State: CONNECTED
Slot: 0
Connected: <0.0.0>
Port controls forker process: forker
Input: 0
Output: 0
Queue: 0
=port:#Port<0.3>
State: CONNECTED|BINARY_IO
Slot: 24
Connected: <0.63.0>
Links: <0.63.0>
Port is UNIX fd not opened by emulator: 2/2
Input: 0
Output: 0
Queue: 0
=port:#Port<0.4>
State: CONNECTED|SOFT_EOF
Slot: 32
Connected: <0.65.0>
Links: <0.65.0>
Port controls linked-in driver: tty_sl -c -e
Input: 36
Output: 263
Queue: 0


BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
i
=memory
total: 16746120
processes: 4260504
processes_used: 4260504
system: 12485616
atom: 278697
atom_used: 257140
binary: 804520
code: 5629302
ets: 394440
=hash_table:atom_tab
size: 8192
used: 5580
objs: 9343
depth: 7
=index_table:atom_tab
size: 10240
limit: 1048576
entries: 9344
=hash_table:module_code
size: 128
used: 77
objs: 107
depth: 4
=index_table:module_code
size: 1024
limit: 65536
entries: 107
=hash_table:export_list
size: 4096
used: 2237
objs: 3257
depth: 5
=index_table:export_list
size: 4096
limit: 524288
entries: 3257
=hash_table:export_list
size: 4096
used: 2228
objs: 3243
depth: 5
=hash_table:process_reg
size: 32
used: 18
objs: 25
depth: 3
=hash_table:fun_table
size: 512
used: 409
objs: 686
depth: 5
=hash_table:node_table
size: 16
used: 1
objs: 1
depth: 1
=hash_table:dist_table
size: 16
used: 1
objs: 1
depth: 1
=allocated_areas
sys_misc: 57816
static: 1053984
atom_space: 131104 109547
atom_table: 147593
module_table: 69360
export_table: 197028
export_list: 651400
register_table: 372
fun_table: 4210
module_refs: 5088
loaded_code: 4702216
dist_table: 643
node_table: 291
bits_bufs_size: 0
bif_timer: 0
process_table: 3145728
port_table: 786432
ets_misc: 131072
external_alloc: 4702216
=allocator:sys_alloc
option e: true
option m: libc
option tt: 131072
option tp: 0
=allocator:temp_alloc[0]
versions: 2.1 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option mbsd: 3
option as: gf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 5 5
mbcs blocks[temp_alloc] size: 0 11000 11000
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 920
temp_free calls: 920
temp_realloc calls: 7
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 56 56
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1
temp_free calls: 1
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 4 4
mbcs blocks[temp_alloc] size: 0 5472 5472
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 400
temp_free calls: 400
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 6 6
mbcs blocks[temp_alloc] size: 0 648536 648536
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 2 2
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 1179648 1179648
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 7905
temp_free calls: 7905
temp_realloc calls: 18
mseg_alloc calls: 4
mseg_dealloc calls: 4
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:temp_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 90
option rsbcmt: 80
option rmbcmt: 100
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: af
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 1 1
mbcs blocks[temp_alloc] size: 0 56 56
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
temp_alloc calls: 1
temp_free calls: 1
temp_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 5 78 78
mbcs blocks[sl_alloc] size: 512 39872 39872
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 2 2
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 294912 294912
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 539
sl_free calls: 534
sl_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 2
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 77 77
mbcs blocks[sl_alloc] size: 0 73672 73672
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 2 2
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 294912 294912
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 157
sl_free calls: 157
sl_realloc calls: 0
mseg_alloc calls: 1
mseg_dealloc calls: 1
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 6238 6238
mbcs blocks[sl_alloc] size: 0 1108872 1108872
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 3 3
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 1343488 1343488
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 9691
sl_free calls: 9691
sl_realloc calls: 0
mseg_alloc calls: 17
mseg_dealloc calls: 17
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:sl_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 80
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: S
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
sl_alloc calls: 0
sl_free calls: 0
sl_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 39 43 43
mbcs blocks[std_alloc] size: 136432 144328 144328
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 64
std_free calls: 25
std_realloc calls: 1
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 1 1 1
mbcs blocks[std_alloc] size: 64 64 64
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 1
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 2 3 3
mbcs blocks[std_alloc] size: 128 7296 7296
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 5
std_free calls: 3
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 135 139 139
mbcs blocks[std_alloc] size: 41800 49072 49072
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 405
std_free calls: 270
std_realloc calls: 0
mseg_alloc calls: 7
mseg_dealloc calls: 6
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:std_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: D
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 2 2 2
mbcs blocks[std_alloc] size: 128 128 128
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
std_alloc calls: 2
std_free calls: 0
std_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 3863 3868 3868
mbcs blocks[ll_alloc] size: 7089328 7123832 7123832
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 4 4 4
mbcs mseg carriers: 3
mbcs sys_alloc carriers: 1
mbcs carriers size: 7864320 7864320 7864320
mbcs mseg carriers size: 7340032
mbcs sys_alloc carriers size: 524288
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 3869
ll_free calls: 6
ll_realloc calls: 0
mseg_alloc calls: 3
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acful: 0
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acful: 0
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 240 240 240
mbcs blocks[ll_alloc] size: 15936 15936 15936
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 240
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acful: 0
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 9898 9898 9898
mbcs blocks[ll_alloc] size: 1408208 1408208 1408208
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 3 3 3
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 1
mbcs carriers size: 1835008 1835008 1835008
mbcs mseg carriers size: 1310720
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 9901
ll_free calls: 3
ll_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ll_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 524288
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 85
option acful: 0
option acnl: 1000
option acfml: 0
option cp: L
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 524288 524288 524288
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 524288
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ll_alloc calls: 0
ll_free calls: 0
ll_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 17 26 26
mbcs blocks[eheap_alloc] size: 238912 246136 246136
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 393216 393216 393216
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 131072
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 35
eheap_free calls: 18
eheap_realloc calls: 0
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acful: 0
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 1 1 1
mbcs blocks[eheap_alloc] size: 72 72 72
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 1
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acful: 0
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 1 3 3
mbcs blocks[eheap_alloc] size: 64 56744 56744
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 4
eheap_free calls: 3
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acful: 0
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 58 62 62
mbcs blocks[eheap_alloc] size: 839240 1056800 1056800
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 3 3 3
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 1
mbcs carriers size: 2228224 2228224 2228224
mbcs mseg carriers size: 2097152
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 631
eheap_free calls: 573
eheap_realloc calls: 26
mseg_alloc calls: 3
mseg_dealloc calls: 1
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:eheap_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 50
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 131072
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 45
option acful: 0
option acnl: 1000
option acfml: 0
option cp: H
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 131072 131072 131072
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 131072
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
eheap_alloc calls: 0
eheap_free calls: 0
eheap_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 0 0 0
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 0
mbcs carriers size: 0 0 0
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 0
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 493 493 493
mbcs blocks[ets_alloc] size: 263368 263368 263368
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 496
ets_free calls: 3
ets_realloc calls: 5
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:ets_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: E
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
ets_alloc calls: 0
ets_free calls: 0
ets_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
fix type: enif_select_data_state 0 0
fix type: driver_select_data_state 0 0
fix type: link 0 0
fix type: monitor 0 0
fix type: sl_thr_q_element 0 0
fix type: process_signal_queue_buffers 0 0
fix type: magic_indirection 0 0
fix type: nsched_pid_ref_entry 0 0
fix type: nsched_magic_ref_entry 128 128
fix type: bif_timer 0 0
fix type: hl_ptimer 0 0
fix type: ll_ptimer 0 0
fix type: msg_ref 0 0
fix type: receive_marker_block 0 0
fix type: proc 4656 4656
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 10 27 27
mbcs blocks[fix_alloc] size: 4960 6048 6048
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 98
fix_free calls: 88
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 1 1 1
mbcs blocks[fix_alloc] size: 64 64 64
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 1
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 133 167 167
mbcs blocks[fix_alloc] size: 34792 40744 40744
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 293
fix_free calls: 160
fix_realloc calls: 0
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:fix_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: false
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: F
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
fix_alloc calls: 0
fix_free calls: 0
fix_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:literal_alloc
versions: 0.9 3.0
option e: true
option t: false
option ramv: false
option atags: false
option sbct: 18446744073709551615
option asbcst: 0
option rsbcst: 0
option rsbcmt: 0
option rmbcmt: 0
option mmbcs: 1048576
option mmsbc: 0
option mmmbc: 18446744073709551615
option lmbcs: 10485760
option smbcs: 1048576
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aobf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 133 133 133
mbcs blocks[literal_alloc] size: 1121480 1121480 1121480
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 2
mbcs sys_alloc carriers: 0
mbcs carriers size: 2097152 2097152 2097152
mbcs mseg carriers size: 2097152
mbcs sys_alloc carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
literal_alloc calls: 134
literal_free calls: 1
literal_realloc calls: 0
mseg_alloc calls: 2
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 0
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 3 50 50
mbcs blocks[binary_alloc] size: 141344 1519640 1519640
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 4 4
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 3440640 3440640
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 1 1 1
sbcs blocks[binary_alloc] size: 657232 657232 657232
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 1 1 1
sbcs mseg carriers: 1
sbcs sys_alloc carriers: 0
sbcs carriers size: 659456 659456 659456
sbcs mseg carriers size: 659456
sbcs sys_alloc carriers size: 0
binary_alloc calls: 202
binary_free calls: 198
binary_realloc calls: 4
mseg_alloc calls: 8
mseg_dealloc calls: 6
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 1 1
mbcs blocks[binary_alloc] size: 0 80 80
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 1
binary_free calls: 1
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 3 3
mbcs blocks[binary_alloc] size: 0 1632 1632
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 3
binary_free calls: 3
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 25 45 45
mbcs blocks[binary_alloc] size: 5944 15336 15336
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 460
binary_free calls: 435
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:binary_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: B
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
binary_alloc calls: 0
binary_free calls: 0
binary_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[0]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 0
option acful: 0
option acnl: 0
option acfml: 0
option cp: undefined
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 30 30 30
mbcs blocks[driver_alloc] size: 6240 6240 6240
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 31
driver_free calls: 1
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[1]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[2]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[3]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 18 19 19
mbcs blocks[driver_alloc] size: 37656 37656 37656
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 2 2 2
mbcs mseg carriers: 1
mbcs sys_alloc carriers: 1
mbcs carriers size: 294912 294912 294912
mbcs mseg carriers size: 262144
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 28
driver_free calls: 10
driver_realloc calls: 0
mseg_alloc calls: 1
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:driver_alloc[4]
versions: 0.9 3.0
option e: true
option t: 5
option ramv: false
option atags: true
option sbct: 524288
option asbcst: 4145152
option rsbcst: 20
option rsbcmt: 80
option rmbcmt: 50
option mmbcs: 32768
option mmsbc: 256
option mmmbc: 18446744073709551615
option lmbcs: 5242880
option smbcs: 262144
option mbcgs: 10
option acul: 60
option acful: 0
option acnl: 1000
option acfml: 0
option cp: R
option as: aoffcbf
mbcs blocks[sys_alloc] count: 0 0 0
mbcs blocks[sys_alloc] size: 0 0 0
mbcs blocks[temp_alloc] count: 0 0 0
mbcs blocks[temp_alloc] size: 0 0 0
mbcs blocks[sl_alloc] count: 0 0 0
mbcs blocks[sl_alloc] size: 0 0 0
mbcs blocks[std_alloc] count: 0 0 0
mbcs blocks[std_alloc] size: 0 0 0
mbcs blocks[ll_alloc] count: 0 0 0
mbcs blocks[ll_alloc] size: 0 0 0
mbcs blocks[eheap_alloc] count: 0 0 0
mbcs blocks[eheap_alloc] size: 0 0 0
mbcs blocks[ets_alloc] count: 0 0 0
mbcs blocks[ets_alloc] size: 0 0 0
mbcs blocks[fix_alloc] count: 0 0 0
mbcs blocks[fix_alloc] size: 0 0 0
mbcs blocks[literal_alloc] count: 0 0 0
mbcs blocks[literal_alloc] size: 0 0 0
mbcs blocks[binary_alloc] count: 0 0 0
mbcs blocks[binary_alloc] size: 0 0 0
mbcs blocks[driver_alloc] count: 0 0 0
mbcs blocks[driver_alloc] size: 0 0 0
mbcs blocks[test_alloc] count: 0 0 0
mbcs blocks[test_alloc] size: 0 0 0
mbcs carriers: 1 1 1
mbcs mseg carriers: 0
mbcs sys_alloc carriers: 1
mbcs carriers size: 32768 32768 32768
mbcs mseg carriers size: 0
mbcs sys_alloc carriers size: 32768
mbcs_pool blocks[sys_alloc] count: 0
mbcs_pool blocks[sys_alloc] size: 0
mbcs_pool blocks[temp_alloc] count: 0
mbcs_pool blocks[temp_alloc] size: 0
mbcs_pool blocks[sl_alloc] count: 0
mbcs_pool blocks[sl_alloc] size: 0
mbcs_pool blocks[std_alloc] count: 0
mbcs_pool blocks[std_alloc] size: 0
mbcs_pool blocks[ll_alloc] count: 0
mbcs_pool blocks[ll_alloc] size: 0
mbcs_pool blocks[eheap_alloc] count: 0
mbcs_pool blocks[eheap_alloc] size: 0
mbcs_pool blocks[ets_alloc] count: 0
mbcs_pool blocks[ets_alloc] size: 0
mbcs_pool blocks[fix_alloc] count: 0
mbcs_pool blocks[fix_alloc] size: 0
mbcs_pool blocks[literal_alloc] count: 0
mbcs_pool blocks[literal_alloc] size: 0
mbcs_pool blocks[binary_alloc] count: 0
mbcs_pool blocks[binary_alloc] size: 0
mbcs_pool blocks[driver_alloc] count: 0
mbcs_pool blocks[driver_alloc] size: 0
mbcs_pool blocks[test_alloc] count: 0
mbcs_pool blocks[test_alloc] size: 0
mbcs_pool carriers: 0
mbcs_pool carriers size: 0
sbcs blocks[sys_alloc] count: 0 0 0
sbcs blocks[sys_alloc] size: 0 0 0
sbcs blocks[temp_alloc] count: 0 0 0
sbcs blocks[temp_alloc] size: 0 0 0
sbcs blocks[sl_alloc] count: 0 0 0
sbcs blocks[sl_alloc] size: 0 0 0
sbcs blocks[std_alloc] count: 0 0 0
sbcs blocks[std_alloc] size: 0 0 0
sbcs blocks[ll_alloc] count: 0 0 0
sbcs blocks[ll_alloc] size: 0 0 0
sbcs blocks[eheap_alloc] count: 0 0 0
sbcs blocks[eheap_alloc] size: 0 0 0
sbcs blocks[ets_alloc] count: 0 0 0
sbcs blocks[ets_alloc] size: 0 0 0
sbcs blocks[fix_alloc] count: 0 0 0
sbcs blocks[fix_alloc] size: 0 0 0
sbcs blocks[literal_alloc] count: 0 0 0
sbcs blocks[literal_alloc] size: 0 0 0
sbcs blocks[binary_alloc] count: 0 0 0
sbcs blocks[binary_alloc] size: 0 0 0
sbcs blocks[driver_alloc] count: 0 0 0
sbcs blocks[driver_alloc] size: 0 0 0
sbcs blocks[test_alloc] count: 0 0 0
sbcs blocks[test_alloc] size: 0 0 0
sbcs carriers: 0 0 0
sbcs mseg carriers: 0
sbcs sys_alloc carriers: 0
sbcs carriers size: 0 0 0
sbcs mseg carriers size: 0
sbcs sys_alloc carriers size: 0
driver_alloc calls: 0
driver_free calls: 0
driver_realloc calls: 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
sys_alloc calls: 1
sys_free calls: 0
sys_realloc calls: 0
=allocator:test_alloc
option e: false
=allocator:mseg_alloc[0]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 6
segments: 7 8 8
segments_watermark: 7
segments_size: 8785920 11272192 11272192
mseg_alloc calls: 15
mseg_dealloc calls: 8
mseg_realloc calls: 0
mseg_create calls: 9
mseg_create_resize calls: 0
mseg_destroy calls: 2
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 2
=allocator:mseg_alloc[1]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:mseg_alloc[2]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 1 1
segments_watermark: 0
segments_size: 0 262144 262144
mseg_alloc calls: 1
mseg_dealloc calls: 1
mseg_realloc calls: 0
mseg_create calls: 1
mseg_create_resize calls: 0
mseg_destroy calls: 1
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 1
=allocator:mseg_alloc[3]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 24
segments: 8 11 11
segments_watermark: 8
segments_size: 4456448 6815744 6815744
mseg_alloc calls: 36
mseg_dealloc calls: 28
mseg_realloc calls: 0
mseg_create calls: 12
mseg_create_resize calls: 0
mseg_destroy calls: 5
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 4
=allocator:mseg_alloc[4]
version: 0.9
option amcbf: 4194304
option rmcbf: 20
option mcs: 10
memory kind: all memory
cached_segments: 0
cache_hits: 0
segments: 0 0 0
segments_watermark: 0
segments_size: 0 0 0
mseg_alloc calls: 0
mseg_dealloc calls: 0
mseg_realloc calls: 0
mseg_create calls: 0
mseg_create_resize calls: 0
mseg_destroy calls: 0
mseg_recreate calls: 0
mseg_clear_cache calls: 0
mseg_check_cache calls: 0
=allocator:erts_mmap.default_mmap
option scs: 0
os mmap size used: 13242368
=allocator:erts_mmap.literal_mmap
option scs: 1073676288
option sco: true
option scrpm: false
option scrfsd: 1024
supercarrier total size: 1073741824
supercarrier total sa size: 2097152
supercarrier total sua size: 0
supercarrier used size: 2162688
supercarrier used sa size: 2097152
supercarrier used sua size: 0
supercarrier used free segs: 0
supercarrier max free segs: 0
supercarrier allocated free segs: 0
supercarrier reserved free segs: 1024
supercarrier sa free segs: 0
supercarrier sua free segs: 0
=allocator:alloc_util
option mmc: 18446744073709551615
option ycs: 1048576
option sac: true
=allocator:instr

BREAK: (a)bort (A)bort with dump (c)ontinue (p)roc info (i)nfo
       (l)oaded (v)ersion (k)ill (D)b-tables (d)istribution
l
Current code: 5796792
Old code: 0
erts_code_purger 16192
erl_init 2424
init 72784
prim_buffer 4984
prim_eval 1248
prim_inet 123568
prim_file 43088
zlib 21616
socket_registry 24504
prim_socket 54600
prim_net 10624
prim_zip 29240
erl_prim_loader 66128
erlang 114088
erts_internal 25704
erl_tracer 1520
erts_literal_area_collector 5416
erts_dirty_process_signal_handler 2416
atomics 3704
counters 4744
persistent_term 1448
erl_parse 319048
supervisor 89680
erl_lint 355840
lists 107176
gen_event 61040
proc_lib 50048
gen_server 75616
filename 50168
logger_server 36200
ets 69400
code 47800
file_io_server 54024
erl_eval 109480
gen 34456
logger_config 11224
heart 18064
code_server 70680
logger_simple_h 14688
file_server 15296
logger 57760
logger_backend 7800
error_handler 5560
application_master 21408
error_logger 18816
logger_filters 5280
file 49376
kernel 17664
application_controller 129576
application 11952
logger_proxy 9504
logger_olp 26088
queue 32544
proplists 15944
peer 60672
beam_lib 73784
binary 37664
gb_sets 25104
gb_trees 17312
os 19640
unicode 48320
erl_features 44392
inet_db 77616
inet_config 26904
inet_udp 7024
inet 91464
inet_parse 45728
inet_gethost_native 35016
rpc 33600
global 133528
net_kernel 109520
rand 95448
maps 21744
erl_distribution 7368
global_group 62088
erpc 52152
standard_error 10944
supervisor_bridge 21720
user_sup 5392
user_drv 40568
group 42904
edlin 33976
io_lib 42040
group_history 41904
io_lib_format 42240
timer 18016
kernel_config 7664
kernel_refc 6784
logger_sup 1808
logger_handler_watcher 3824
erl_signal_handler 3936
logger_formatter 30208
shell 89168
logger_std_h 30960
logger_h_common 28496
c 62296
orddict 10576
raw_file_io 3728
epp 112928
erl_anno 12008
erl_abstract_code 3080
ordsets 5912
io 28632
string 134984
unicode_util 1002640
erl_scan 92032
io_lib_pretty 70096


6> halt().



```