# l-eec-lab-2-posix---concurrent-execution-solved
**TO GET THIS SOLUTION VISIT:** [L.EEC Lab 2-POSIX – Concurrent execution Solved](https://www.ankitcodinghub.com/product/l-eec-lab-2-posix-concurrent-execution-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95096&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;L.EEC Lab 2-POSIX - Concurrent execution Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Introduction

</div>
</div>
<div class="layoutArea">
<div class="column">
In modern operating systems, the code that runs in the CPU can either be running in a special privilege/protected mode (normally reserved for OS system calls or device drivers) or in the so-called user-space, where user programs execute within

</div>
</div>
<div class="layoutArea">
<div class="column">
processes, which are self-contained components with a proper interface with the

</div>
</div>
<div class="layoutArea">
<div class="column">
OS. The OS supports

</div>
</div>
<div class="layoutArea">
<div class="column">
creating, scheduling, terminating processes, and enables

</div>
</div>
<div class="layoutArea">
<div class="column">
the communication/signaling with and between the processes.

</div>
</div>
<div class="layoutArea">
<div class="column">
Curiosity: The printf function manages the interface between a process and a special serial communication channel (aka standard output). When launching a

</div>
</div>
<div class="layoutArea">
<div class="column">
process this channel is bound to the terminal/console, printing the serialized data.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
If you develop a monolithic (not concurrent) piece of code, you are good with running it in a single process or thread. However, if you are waiting for an external event (e.g. using scanf) that triggers a time-intensive task, one has to choose between blocking on the external event (wait on scanf) or executing the task and risk missing input

</div>
</div>
<div class="layoutArea">
<div class="column">
events.

</div>
</div>
<div class="layoutArea">
<div class="column">
In the following weeks we will cover the handling of concurrent task execution

</div>
</div>
<div class="layoutArea">
<div class="column">
in your program with both multi-processing and multi-threading. We will also cover the synchronization of these tasks, sharing memory and handling race-conditions

</div>
</div>
<div class="layoutArea">
<div class="column">
when accessing shared resources (mutual exclusion).

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
This laboratory work will be divided into 3 parts with the following objectives:

</div>
</div>
<div class="layoutArea">
<div class="column">
Computing Systems

</div>
</div>
<div class="layoutArea">
<div class="column">
Part A – OS processes.

</div>
</div>
<div class="layoutArea">
<div class="column">
Part B – Process threads.

</div>
</div>
<div class="layoutArea">
<div class="column">
Part C – Condition variables and other synchronization methods.

</div>
</div>
<div class="layoutArea">
<div class="column">
At the end there will be an individual assessment through the development of a

</div>
</div>
<div class="layoutArea">
<div class="column">
small program.

</div>
</div>
<div class="layoutArea">
<div class="column">
Complementary readings:

<ul>
<li>● &nbsp;Processes API (OSTEP Ch. 5)</li>
<li>● &nbsp;Threads API (OSTEP Ch. 27 -until Sec. 27.3)</li>
<li>● &nbsp;Locked Data Structures (OSTEP Ch. 29)</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column"></div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
Part A – OS Processes

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
A Process within the Operating System is an instance of a running program that includes the respective code and all the associated memory. In a multi-process OS, a process runs along with other processes, competing for CPU time slots, as well as

</div>
</div>
<div class="layoutArea">
<div class="column">
for other hardware resources, especially I/O.

</div>
</div>
<div class="layoutArea">
<div class="column">
One approach (there are others) to programmatically launch a new process

</div>
</div>
<div class="layoutArea">
<div class="column">
is to clone a running process that we will call the parent process. This is achieved using the POSIX function fork. The clone process is called the child process. All the parent process memory is replicated (using memcpy) and the child process

</div>
</div>
<div class="layoutArea">
<div class="column">
becomes autonomous, i.e., both parent and child processes are managed

</div>
</div>
<div class="layoutArea">
<div class="column">
independently by the OS and its scheduling.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Use the top command to identify the currently running processes, along with their CPU usage share. The program also measures the execution time of each process from two angles: 1) the system clock that does not stop and 2) the process clock that

</div>
</div>
<div class="layoutArea">
<div class="column">
counts the time the process is in the running state.

</div>
</div>
<div class="layoutArea">
<div class="column">
The following code instantiates a number of processes – there is a defined macro to

</div>
</div>
<div class="layoutArea">
<div class="column">
control the number of processes.

</div>
</div>
<div class="layoutArea">
<div class="column">
Tweak HOW_MANY_FORKS and try to guess the number of CPU cores on your machine/VM. Mind that Intel CPUs with Hyper-threading (SMT) enabled virtually duplicate the number of cores. In a Unix-like OS (Linux, MacOS, BSD, Solaris), the top command (terminal) shows a rank of the running processes, normally exhibiting

</div>
</div>
<div class="layoutArea">
<div class="column">
the top CPU demanding processes, along with their PID (process ID) and name.

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Tutorial Program Atp1 (full code @Atp1.c)

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Exercise 1: Modify the function heavy_load, so it is busy-waits for a certain amount of time (fixed), say 15 seconds, counted using the CPU process clock. The process clock differs from the real-time clock, in which it only counts time when the process

</div>
</div>
<div class="layoutArea">
<div class="column">
is executing.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
The use of process forking involves creating a new memory space – the process memory is in fact duplicated upon forking (memcpy). Hence, it is not possible to share a variable in memory amongst different processes even when cloned from the same

</div>
</div>
<div class="layoutArea">
<div class="column">
program. Memory isolation is enforced by design at OS level.

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
The following snippet (Atp2) illustrates memory isolation. It also uses the function wait to synchronize the parent process at the end of the child. Examine the code

</div>
</div>
<div class="layoutArea">
<div class="column">
and try to predict the results on each printf.

</div>
</div>
<div class="layoutArea">
<div class="column">
Tutorial Program Atp2 (full code @Atp2.c)

</div>
</div>
<div class="layoutArea">
<div class="column">
Exercise 2: Modify the previous code so the parent launches two different Childs

</div>
</div>
<div class="layoutArea">
<div class="column">
and waits (synchronizes) for them before returning.

</div>
</div>
<div class="layoutArea">
<div class="column">
Multitasking

</div>
</div>
<div class="layoutArea">
<div class="column">
Page 3 | 13

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Computing Systems

</div>
</div>
<div class="layoutArea">
<div class="column">
L.EEC

</div>
</div>
<div class="layoutArea">
<div class="column">
2021/2022

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
There are two main arguments that encourage multitasking a process and splitting the execution of a monolithic program: 1) Having multiple execution contexts enables blocking routines (e.g. waiting on a scanf or some I/O message) to coexist without blocking each other; and 2) speed up the overall execution by exploring multicore

</div>
</div>
<div class="layoutArea">
<div class="column">
infrastructures and code parallelization.

</div>
</div>
<div class="layoutArea">
<div class="column">
In both scenarios, there will be a moment when processes need to synchronize and communicate data from one side to the other. Inter-process communication (IPC) is a vast topic that ranges from simple process signaling to complex network-oriented communication and component distribution models. A list of IPC techniques can be

</div>
</div>
<div class="layoutArea">
<div class="column">
found

</div>
</div>
<div class="layoutArea">
<div class="column">
A simple mechanism to retrieve data from a child process to the parent process

</div>
</div>
<div class="layoutArea">
<div class="column">
uses the exit status code. When quitting processes, the program may report a

</div>
</div>
<div class="layoutArea">
<div class="column">
signal code to the OS. This signal normally briefs the OS with an error code that

</div>
</div>
<div class="layoutArea">
<div class="column">
indicates the cause conveying the end of the process. In C language the

</div>
</div>
<div class="layoutArea">
<div class="column">
programmer may use the return statement in the main function or the exit

</div>
</div>
<div class="layoutArea">
<div class="column">
function with the proper code (exit – issues program termination directly from any

</div>
</div>
<div class="layoutArea">
<div class="column">
function).

</div>
</div>
<div class="layoutArea">
<div class="column">
Curiosity: The following shell command “gcc -o code code.c &amp;&amp; ./code” runs a

</div>
</div>
<div class="layoutArea">
<div class="column">
program after a successful compilation process, i.e executes if gcc returns code 0

</div>
</div>
<div class="layoutArea">
<div class="column">
(no error).

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
here.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
In Atp3.c you may find a monolithic code example that executes a batch of jobs,

</div>
</div>
<div class="layoutArea">
<div class="column">
compiles the result for each job and prints out the result at the end. Analyze the

</div>
</div>
<div class="layoutArea">
<div class="column">
code to understand the use of the struct handler that follows the whole process.

</div>
</div>
<div class="layoutArea">
<div class="column">
The structure stores the input values, the pending status and the result.

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Exercise 3: Implement the function dispatch_jobs_v1. This alternate function

</div>
</div>
<div class="layoutArea">
<div class="column">
shall produce the same result, but instead of a monolithic approach, each job runs

</div>
</div>
<div class="layoutArea">
<div class="column">
on a dedicated process. Carry out your tests along with a top observation.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Exercise 4: The previous approach has one catch! In a scenario with 1000 jobs

</div>
</div>
<div class="layoutArea">
<div class="column">
you’ll trigger 1000 processes, all competing for the CPU.

</div>
</div>
<div class="layoutArea">
<div class="column">
Implement the function dispatch_jobs_v2, similarly to v1, but instead of

</div>
</div>
<div class="layoutArea">
<div class="column">
launching all processes at once, it limits

</div>
</div>
<div class="layoutArea">
<div class="column">
(workers) – see SIMULTANEOUS_WORKERS_MAX. Try to avoid empty slots –

</div>
</div>
<div class="layoutArea">
<div class="column">
the number of simultaneous processes

</div>
</div>
<div class="layoutArea">
<div class="column">
example: If you trigger A and B processes, A faster than B, and you synchronize

</div>
</div>
<div class="layoutArea">
<div class="column">
both before launching C and D, then you’ll be wasting computing power.

</div>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
Part B – Process Threads

Tutorial Program Btp1 (full code @Btp1.c)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Process threads can be seen as sections of a program that execute independently within the scope of a process. Threads execution may differ, based on the OS architecture, but in general they are components of the process, sharing execution

</div>
</div>
<div class="layoutArea">
<div class="column">
code data and memory (particularly the process data segment and heap).

</div>
</div>
<div class="layoutArea">
<div class="column">
The following snippet (Btp1) depicts the instantiation of two threads with the same

</div>
</div>
<div class="layoutArea">
<div class="column">
code base, followed by a synchronization at the end of each thread.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
One of the most relevant aspects that differentiate thread-based and process-based approaches for multitasking is memory access. We have seen with processes that

</div>
</div>
<div class="layoutArea">
<div class="column">
communication between processes requires additional OS components. When using threads, their process memory space is shared, which facilitates data sharing. Though, keep in mind that open access to memory comes with the risk of failure/security and specially data integrity. Memory isolation and protection is valued

</div>
</div>
<div class="layoutArea">
<div class="column">
for certain applications.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
The following snippet (Btp2) highlights how threads can seamlessly update global

</div>
</div>
<div class="layoutArea">
<div class="column">
and static variables.

</div>
</div>
<div class="layoutArea">
<div class="column">
Note: static variables behave as permanent variables within the scope of a function. Static and global variables sit on the data segment of the process. In this example the static variable s refers to the same memory position in both threads. You may see static variables as being persistent across multiple calls of a function. In the case of a thread’s execution body, it is the same variable across different threads, whereas

</div>
</div>
<div class="layoutArea">
<div class="column">
local variables will still be given different memory positions on each thread’s stack.

</div>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
Tutorial Program Btp2 (full code @Btp2.c)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Memory isolation between processes means that each process gets its private memory space. Forking a process requires an operation of allocating memory for that process (managed at OS level), cloning the current process memory, and binding to several system resources. And all this takes time. It may seem fast to a

</div>
</div>
<div class="layoutArea">
<div class="column">
naked eye, but sure is not at computing level.

</div>
</div>
<div class="layoutArea">
<div class="column">
The following snippet (Btp3) proposes the execution of an empty task (start and

</div>
</div>
<div class="layoutArea">
<div class="column">
finish) multiple times, running with processes and threads for comparison. You may

</div>
</div>
<div class="layoutArea">
<div class="column">
witness the performance penalty of creating and destroying a process.

</div>
</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="section">
<div class="layoutArea">
<div class="column">
Mutexes

</div>
</div>
<div class="layoutArea">
<div class="column">
In scenarios where multiple threads access shared data or common resources simultaneously it is common to enclose the access within a critical section. In this section we need to guarantee that any operation executes without preemption, i.e no other thread will access the region while one thread is performing. Mutexes behave

</div>
</div>
<div class="layoutArea">
<div class="column">
as binary flags that when locked prevent other threads from entering the associated critical section. Lock and unlock operations are atomic, guaranteed at kernel or

</div>
</div>
<div class="layoutArea">
<div class="column">
processor level.

</div>
</div>
</div>
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
For certain data types and usage models there are programming techniques that circumvent the requirement for a strict mutex to enter the critical region. This often requires a deep understanding of the concurrent model, the OS scheduling behavior and compiler instructions regarding atomicity. A simple example would be a thread that only reads data inside that region, which may be dispensed of checking the mutex in certain conditions. In fact, this is not a golden rule though. The use of mutexes or other atomic structures such as semaphores guarantee a safe access to

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
critical sections.

</div>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Here’s a list of basic primitives to handle a mutex in a multithreading environment:

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
pthread_mutex_init pthread_mutex_lock pthread_mutex_unlock pthread_mutex_destroy

Tutorial Program Btp4 (full code @Btp4.c)

</div>
</div>
<div class="layoutArea">
<div class="column">
The following snippet (Btp4) instantiates three threads that concurrently print data to the terminal on specific lines. The result is a mess because the access is unguarded.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Exercise 5: Improve the code in Btp4 to guard the access to the shared resource –

</div>
</div>
<div class="layoutArea">
<div class="column">
the terminal.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
We have seen an example of unguarded access to a shared resource. The following snippet (Btp5) depicts the use of two threads in a producer-consumer model over a shared data model – a circular FIFO buffer. There is one thread that periodically pushes values to a circular FIFO buffer, while another thread periodically pops values

</div>
</div>
<div class="layoutArea">
<div class="column">
from that buffer. The producer thread is running faster (smaller period) than the consumer, leading to occasional (but certain) “Buffer Full” messages. You may

</div>
</div>
<div class="layoutArea">
<div class="column">
ignore these messages for now.

</div>
</div>
<div class="layoutArea">
<div class="column">
With two threads accessing a critical region (the buffer), the buffering structure may become inconsistent. This race-condition requires mutual-exclusion protection

</div>
</div>
<div class="layoutArea">
<div class="column">
(mutexes).

</div>
</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="section">
<div class="layoutArea">
<div class="column">
Buffer

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Critical Section

Producer-thread Consumer-thread

Tutorial Program Btp5 (full code @Btp5.c)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Exercise 6: Improve the code in Btp5 to protect the calls to the buffer with a mutex.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Deadlocks

</div>
</div>
<div class="layoutArea">
<div class="column">
The use of multiple mutexes comes with a risk. When two threads are waiting (to lock) on different mutexes and the unlock of each is inside the critical region of the other mutex, then they enter a state of deadlock, where none can unlock and move

</div>
</div>
<div class="layoutArea">
<div class="column">
on. Btp6 depicts one such scenario.

</div>
</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="layoutArea">
<div class="column">
Tutorial Program Btp6 (full code @Btp6.c)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Exercise 7: Improve the code in Btp6 to avoid deadlocks.

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Page 10 | 13

</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="layoutArea">
<div class="column">
Computing Systems

</div>
</div>
<div class="layoutArea">
<div class="column">
Conditional Variables

</div>
</div>
<div class="layoutArea">
<div class="column">
Part C –Threads Synchronization

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
In Btp5 we have seen two threads making use of the Producer-Consumer model.

</div>
</div>
<div class="layoutArea">
<div class="column">
The producer updates the buffer and the consumer should get the value in the

</div>
</div>
<div class="layoutArea">
<div class="column">
buffer after the update. But both threads are unsynchronized and the buffer

</div>
</div>
<div class="layoutArea">
<div class="column">
handling on both sides constitutes a critical section. The consumer is unaware of

</div>
</div>
<div class="layoutArea">
<div class="column">
when the producer updates the buffer and it keeps polling the queue size to get

</div>
</div>
<div class="layoutArea">
<div class="column">
new data.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
This communication/synchronization model is inherently inefficient – the Consumer

</div>
</div>
<div class="layoutArea">
<div class="column">
thread will either busy-wait (CPU intensive loop) constantly checking for updates, or

</div>
</div>
<div class="layoutArea">
<div class="column">
it will only poll from time to time, lowering the CPU demand and potentially

</div>
</div>
<div class="layoutArea">
<div class="column">
increasing the latency between the producing event and the consuming event. To

</div>
</div>
<div class="layoutArea">
<div class="column">
improve this situation, a synchronization mechanism is needed to let the consumer

</div>
</div>
<div class="layoutArea">
<div class="column">
know when there is fresh data in the buffer.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
We have seen that mutexes synchronize threads when accessing a critical region.

</div>
</div>
<div class="layoutArea">
<div class="column">
In this case, if the Consumer-thread keeps a mutex locked while waiting for an

</div>
</div>
<div class="layoutArea">
<div class="column">
update, the producer will not be able to push an update because the mutex is

</div>
</div>
<div class="layoutArea">
<div class="column">
locked. Mutexes cannot be locked in one thread and unlocked in another one! Each

</div>
</div>
<div class="layoutArea">
<div class="column">
thread that uses a mutex must lock and unlock it, and only when using the

</div>
</div>
<div class="layoutArea">
<div class="column">
respective critical section. Thus, we need another solution.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Conditional Variables provide a solution for this thread synchronization problem.

</div>
</div>
<div class="layoutArea">
<div class="column">
One can see a conditional variable as a flag inside the critical section. The

</div>
</div>
<div class="layoutArea">
<div class="column">
Consumer thread locks the mutex of the critical section and waits on that flag (in

</div>
</div>
<div class="layoutArea">
<div class="column">
this case, for that flag to be set by the Producer). While waiting, it must temporarily

</div>
</div>
<div class="layoutArea">
<div class="column">
release the mutex, so that whoever sets the flag (the Producer in this case) can

</div>
</div>
<div class="layoutArea">
<div class="column">
enter the critical section, perform its function (updating the buffer in this case) and

</div>
</div>
<div class="layoutArea">
<div class="column">
signal the condition variable.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Once the Producer signals the conditional variable, the Consumer thread

</div>
</div>
<div class="layoutArea">
<div class="column">
immediately1 leaves the waiting state and locks the given mutex again, knowing

</div>
</div>
<div class="layoutArea">
<div class="column">
that the Producer left the critical section after an update. The consumer is now

</div>
</div>
<div class="layoutArea">
<div class="column">
inside the critical section and ready to fetch the new data. This releasing and

</div>
</div>
<div class="layoutArea">
<div class="column">
reacquiring the mutex while waiting is done automatically inside the respective

</div>
</div>
<div class="layoutArea">
<div class="column">
system call (see the next section).

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Conditional variables inside critical sections behave as notification mechanisms

</div>
</div>
<div class="layoutArea">
<div class="column">
(like signaling channels).

</div>
</div>
<div class="layoutArea">
<div class="column">
1 Not exactly “immediately” because the producer will have to leave the lock after flagging the update. Page 11 | 13

</div>
</div>
</div>
<div class="page" title="Page 12">
<div class="layoutArea">
<div class="column">
Computing Systems

</div>
</div>
<div class="layoutArea">
<div class="column">
L.EEC

</div>
</div>
<div class="layoutArea">
<div class="column">
2021/2022

</div>
</div>
<div class="layoutArea">
<div class="column">
Buffer

</div>
</div>
<div class="layoutArea">
<div class="column">
Cond. Var

Critical Section

</div>
</div>
<div class="layoutArea">
<div class="column">
Producer-thread

Libpthread API

</div>
<div class="column">
Consumer-thread

</div>
</div>
<div class="layoutArea">
<div class="column">
● pthread_cond_tc=PTHREAD_COND_INITIALIZER;

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>pthread_mutex_t m = PTHREAD_MUTEX_INITIALIZER;
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
o Macros with generic initialization code.

</div>
</div>
<div class="layoutArea">
<div class="column">
● pthread_cond_wait ( pthread_cond_t *restrict cond,

</div>
</div>
<div class="layoutArea">
<div class="column">
pthread_mutex_t *restrict mutex )

</div>
</div>
<div class="layoutArea">
<div class="column">
o A thread must hold the mutex, when calling pthread_cond_wait().

</div>
</div>
<div class="layoutArea">
<div class="column">
o pthread_cond_wait() automatically releases the lock while waiting.

flag.

● pthread_cond_signal(pthread_cond_t *cond)

o Wakes up one thread waiting on the condition variable, if any.

● pthread_cond_broadcast(pthread_cond_t *cond)

o Wakes up all threads waiting on the condition variable, if any.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
o When the condition variable cond is signaled, pthread_cond_wait()

</div>
</div>
<div class="layoutArea">
<div class="column">
automatically reacquires the lock so that the thread is holding it upon

</div>
</div>
<div class="layoutArea">
<div class="column">
returning. However, it is not guaranteed that the condition associated

</div>
</div>
<div class="layoutArea">
<div class="column">
to the signaling, i.e., the flag, is still satisfied – other threads may have

</div>
</div>
<div class="layoutArea">
<div class="column">
preempted this thread after return and taken an action that resets the

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Page 12 | 13

</div>
</div>
</div>
<div class="page" title="Page 13">
<div class="layoutArea">
<div class="column">
Computing Systems

</div>
</div>
<div class="layoutArea">
<div class="column">
L.EEC

</div>
</div>
<div class="layoutArea">
<div class="column">
2021/2022

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Exercise 8: In Btp5 the access to the shared resource (buffer) was guarded with a

</div>
</div>
<div class="layoutArea">
<div class="column">
mutex. But both threads are running freely in independent loops – unsynchronized. Add a conditional variable to the code, so that the consumer polls the queue status

</div>
</div>
<div class="layoutArea">
<div class="column">
only when notified. Be aware that:

</div>
</div>
<div class="layoutArea">
<div class="column">
● When the producer signals the conditional variable, the consumer may not

</div>
</div>
<div class="layoutArea">
<div class="column">
be listening (i.e., waiting within pthread_cond_wait()). As an example, if the

</div>
</div>
<div class="layoutArea">
<div class="column">
consumer is notified and then takes too much time processing the buffer

</div>
</div>
<div class="layoutArea">
<div class="column">
until returning to waiting again, the producer may generate one or multiple

</div>
</div>
<div class="layoutArea">
<div class="column">
signal notifications in the meanwhile, that will be overwritten, thus lost.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Exercise 9: Implement a variation of the previous with one producer and two/three

</div>
</div>
<div class="layoutArea">
<div class="column">
consumer threads. Each consumer thread will pop from the buffer and print the

</div>
</div>
<div class="layoutArea">
<div class="column">
result (along with its thread ID).

</div>
</div>
<div class="layoutArea">
<div class="column">
● Observe how the consumer threads alternate, indicating the existence of a

</div>
</div>
<div class="layoutArea">
<div class="column">
thread waiting queue in the conditional variable.

</div>
</div>
<div class="layoutArea">
<div class="column">
● Repeat with a broadcast signaling.

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Exercise 10: Implement the following scenario, as depicted in the following

</div>
</div>
<div class="layoutArea">
<div class="column">
illustration.

</div>
</div>
<div class="layoutArea">
<div class="column">
Producer-thread

</div>
<div class="column">
Relay-thread

</div>
<div class="column">
Consumer-thread CLI-thread

</div>
</div>
<div class="layoutArea">
<div class="column">
Buffer1

</div>
<div class="column">
Buffer2

</div>
</div>
<div class="layoutArea">
<div class="column">
Suspend flag

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
● Producer-thread periodically pushes a value (random) to Buffer1.

</div>
</div>
<div class="layoutArea">
<div class="column">
● Relay-thread consumes from Buffer1 and produces to Buffer2. Use a

</div>
</div>
<div class="layoutArea">
<div class="column">
conditional var to sync with the production events.

</div>
</div>
<div class="layoutArea">
<div class="column">
● Consumer thread consumes from Buffer 2 (in sync with Relay-thread

</div>
</div>
<div class="layoutArea">
<div class="column">
production) and prints the output to the screen.

</div>
</div>
<div class="layoutArea">
<div class="column">
● CLI-thread reads from stdin to toggle a flag that suspends the Consumer-

</div>
</div>
<div class="layoutArea">
<div class="column">
thread’s activity.

</div>
</div>
<div class="layoutArea">
<div class="column">
● While suspended, both buffers will get filled up and the Producer-thread

</div>
</div>
<div class="layoutArea">
<div class="column">
eventually gets a full buffer indication. When that happens, the thread should

</div>
</div>
<div class="layoutArea">
<div class="column">
wait for buffer availability. That means the Producer-thread will proceed with

</div>
</div>
<div class="layoutArea">
<div class="column">
its data production loop as soon as Buffer1 becomes available again. This

</div>
</div>
<div class="layoutArea">
<div class="column">
procedure needs to be propagated for Buffer2, so that when Consumer-

</div>
</div>
<div class="layoutArea">
<div class="column">
thread resumes activity, Relay-thread can relay from Buffer 1 to Buffer2, thus

</div>
</div>
<div class="layoutArea">
<div class="column">
waking Producer-thread that can now push data to Buffer1.

</div>
</div>
<div class="layoutArea">
<div class="column">
● Another point to consider is that Relay-thread must only pop from Buffer1 if it

</div>
</div>
<div class="layoutArea">
<div class="column">
is certain that it fits in Buffer2 (not full).

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Page 13 | 13

</div>
</div>
</div>
