## The main points of Chapter One
## What is concurrency?
At the simplest and most basic level, concurrency is about two or more separated activities happened at the same time. 
Concurrency in computer systems:
**Task switching**:Computers have only one processors can only perform one task at a time, but it can switch between tasks many times per second. By doing a bit of one task and then a bit of another and so on, it appears that the tasks are happening concurrently.
Hardware concurrency: multi-core processors are capable of genuinely running more than one task in parallel. 

<font color=Blue> this is a<font>
## Approaches to Concurrency:

(Concurrency with multiple processes), Downsides one: The communication between these processes is often either complicated to set up or slow, or both, because operating systems typically provide a lot of protection between processes to avoid one process accidentally modifying data belonging to another process.
Downside two: There’s an inherent overhead in running multiple processes: it takes time to start a process, the operating system must devote internal resources to managing the process, and so forth.
Upside one: The added protection operating systems typically provide between processes and the higher-level communication mechanisms mean that it can be easier to write safe concurrent code with processes rather than threads.
Upside two: Run the separate processes on distinct machines connected over a network.(Though this increases the communication cost, on a carefully designed system it can be a costeffective way of increasing the available parallelism and improving performance)
(Concurrency with multiple threads)Downsides: Lack of protection, data competition
Upsides: Shared address space(flexibility of shared memory), smaller overhead with launching and communication between multiple threads.
Why use Concurrency?
1.Using concurrency for separation of concerns, for separation of concerns is almost always a good idea when writing software. 2.Using concurrency for performance, task and data parallelism.
Data parallelism v.s. Task parallelism: For one algorithm has a lot of data to process, then we can divide the data up among multiple processors running the same algorithm. For one bunch of data, we want to know its average value, maximum value, minimum value, for we can have different processors each look at the same data set and compute different answers.


