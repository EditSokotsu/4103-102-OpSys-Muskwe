####Yani Muskwe OpSys-4103-102 Test-add-on


#Multi*

1.  Multitasking refers to an operating system's ability to run multiple processes concurrently, over a certain quantum, ("concurrently" because these processes aren't run in parallel). Processes are executed in an "interleaving" manner, meaning a single process does not need to finish before another is executed. Resources, such as the CPU and main memory, are shared by the OS amongst all processes, via a number of strategies. The concept of multitasking is similar to the Lehman's intuitive idea of what "multitasking" is: doing homework, while listing to music, chewing gum and texting is multitasking; multiple processes (homework, music, ect) are all being done concurrently (one would have to switch oneself between each process, just like processes are switched on and of the CPU). 

2.  Multiprogramming - Multiprogramming is also the ability of an operating system to execute more than one program on a single processor machine. One/multiple programs are loaded into main memory, ready for execution. This is meant to improve the system by increasing the the use of the CPU, i.e. the aim of multiprocessing is to keep the CPU as busy as possible.

  "suppose the currently running process is performing an I/O task (which, by definition, does not need the CPU to be accomplished). Then, the OS may interrupt that process and give the control to one of the other in-main-memory programs that are ready to execute (i.e. process context switching). In this way, no CPU time is wasted by the system waiting for the I/O task to be completed, and a running process keeps executing until either it voluntarily releases the CPU or when it blocks for an I/O operation."[1]
  
3.  Multi-processing - as the name would suggest, this refers to the concept of running multipe programs (or processes) at the same time (simulaneously). The system is able to both support multiple **_processors_** (hardware) and to allocate tasks to them. This must not be confused with multiprogramming. The difference between them is as such: a multi-processing system can run processes simultaneously because it has multiple **_processors_**. Most modern machines use this mechanism.
  
4.  Multi-threading - the ability of a CPU, or single core in a multiprocessor system, to execute multiple threads (or processes) concurrently. The threads must share resources, too. The goal of this mechanism is to optimise the use of a core or CPU, in a way similar to that of multiprogramming. "If a thread gets a lot of cache misses, the other threads can continue taking advantage of the unused computing resources, which may lead to faster overall execution as these resources would have been idle if only a single thread were executed."[2] However, the sharing of resources can result in threads actually running slower; for example if processes are dependent upon each other, the execution of one could delay the execution of the other.
  
  There are also three types of multi-processsing: block, interleaved and simultaneous multi-processing.
  
#Chapter 3

1.  A sequence of instructions that execute for a particular process.

2.  A process can be created by other processes (called **_SPAWNING_** a process). Child processes can also spawn children.

3.  "Preempting a process" is the act of interrupting the execution of a process from being carried out by a computer system, without requiring its cooperation, and with the intention of resuming the task at a later time. Such changes of the executed task are known as context switches.

4.  Swapping refers to replacing segments (or pages) of data in memory. Swapping is a useful technique that enables a computer to execute programs and manipulate data files larger than main memory. The operating system copies as much data as possible into main memory, and leaves the rest on the disk.

5.  The blocked/suspend state is where process that are awaiting some action are sent, to virtual memory. For example if a process sends a request to a server, and/or exceeds its quantum, it will be put in the blocked/suspended state to free the CPU for other processes. The ready/suspended state is one in which a process is waiting to use the CPU. The term "suspended" indicates that, while in these states, the process(es) are in virtual memory.

6.  When suspended, process is not currently available for execution; a process may or may not be waiting for an event. If not, it is said to be independent of the "blocked" state; the process may have been put into this state by some agent, eg. a parent process, in order to prevent it from running; a process can't leave this state unless expressly released by the agent.

7.  A PCB usually contains process identification data, process state data and process control data.

8.  Two modes are necessary in order to abstract some features of the operating from a user. This is done to proect the integrity of the system. In user mode, a user has less privileges; typically, only user programs are executed in this mode. More privileges and control over the operating system are accessible in the kernel mode. Typically system-level instructions are can be run here. For example, in kernel mode one should be able to access the processor directly, this is not possible in user mode.

9.  A trap can best be equated to a exception in software development; an error is generated in a running process, then the OS determines what actions to take next. What action the OS takes depends on what error generates. An interrupt is occurs when an external event _interrupts_ a processes execution. These external event are indepedent of said process.

10. I/O interrupts occur when peripheral hardware devices need the OS's attention. A memory fault is raised by computer hardware when a running program accesses a memory page that is mapped into the virtual address space, but not actually loaded into main memory.

11. A mode switch refers to the switching between user and kernel mode, and a a process switch is a switch between processes. In a process switch, the state of a process is stored to that execution can continue.
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
[1][https://gabrieletolomei.wordpress.com/miscellanea/operating-systems/multiprogramming-multiprocessing-multitasking-multithreading/](https://gabrieletolomei.wordpress.com/miscellanea/operating-systems/multiprogramming-multiprocessing-multitasking-multithreading/)

[2][https://en.wikipedia.org/wiki/Multithreading_(computer_architecture)](https://en.wikipedia.org/wiki/Multithreading_(computer_architecture))
