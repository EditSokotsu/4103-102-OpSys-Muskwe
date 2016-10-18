#Multi*

1.  Multitasking refers to an operating system's ability to run multiple processes concurrently, over a certain quantum, ("concurrently" because these processes aren't run in parallel). Processes are executed in an "interleaving" manner, meaning a single process does not need to finish before another is executed. Resources, such as the CPU and main memory, are shared by the OS amongst all processes, via a number of strategies. The concept of multitasking is similar to the Lehman's intuitive idea of what "multitasking" is: doing homework, while listing to music, chewing gum and texting is multitasking; multiple processes (homework, music, ect) are all being done concurrently (one would have to switch oneself between each process, just like processes are switched on and of the CPU). 

2.  Multiprogramming - Multiprogramming is also the ability of an operating system to execute more than one program on a single processor machine. One/multiple programs are loaded into main memory, ready for execution. This is meant to improve the system by increasing the the use of the CPU, i.e. the aim of multiprocessing is to keep the CPU as busy as possible.

  "suppose the currently running process is performing an I/O task (which, by definition, does not need the CPU to be accomplished). Then, the OS may interrupt that process and give the control to one of the other in-main-memory programs that are ready to execute (i.e. process context switching). In this way, no CPU time is wasted by the system waiting for the I/O task to be completed, and a running process keeps executing until either it voluntarily releases the CPU or when it blocks for an I/O operation."[1]
  
3.  Multi-processing - as the name would suggest, this refers to the concept of running multipe programs (or processes) at the same time (simulaneously). This must not be confused with multiprogramming. The difference between them is as such: a muli-processing system can run processes simultaneously because it has multiple **_processors_**. 
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  [1][https://gabrieletolomei.wordpress.com/miscellanea/operating-systems/multiprogramming-multiprocessing-multitasking-multithreading/](https://www.google.com)
