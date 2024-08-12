---
pageClass: courses-page
---

# Courses

Here are some of the notable courses I have taken in NUS. Projects and Assignment codes may be hidden for privacy purpose. 

**CS2100 (Computer Organisation)**
- Learnt the fundamentals of Computer Device such as circuit design, ALU, memory hierarchy and input/output. Some hands-on assignment on writing Assembly code in MIPS.

**CS2102 (Database Systems)**
- Learnt the fundamentals of relational Database. Learnt the fundamentals of SQL such as designing query (aggregates, view, CTE), triggers and database normalization. 

**CS2103 (Software Engineering)**
- Learnt the fundamental of Software Enginering. Learnt different SDLC model (Waterfall, Brownfield, Agile), Software Engineering principle (SOLID, design patterns) and documentation (UML, markdown). 
- Worked in a team of 5 to work on improving a project following Brownfield SDLC model. From a simple task manager, we evolve it into a Java team management tools that allow grouping of different member in companies into different groups and to assign tasks to groups or individuals. The code is available [here](https://github.com/zicotjia/tp)

**CS2105 (Introduction to Computer Networks)**
- Learnt the fundamental concepts in Networking. Go through the OSI 7 layers of Networking minus layer 5-6 (Physical, Data Link, Network, Transport, Application). For assignments. create a simple server client that sends data through TCP or UDP, implement a server that has simple reliability protocol (Given a high-level design as a state machine within the assignment) to be able to handle corrupt/invalid packet from a client. Assignment codes are written in Python 3.

**CS2106 (Introduction to Operating Systems)**
- Learnt the fundamental of Operating Systems (Mostly Unix/Linux). Learnt about the kernel architectures, memory virtualization, process scheduling, synchronisation, memory allocation and file system (ext2 and FAT32) and etc.

**CS2109 (Introduction to AI and Machine Learning)**
- Learnt the fundamental of classical and mordern AI.

**CS2030S (Programming Methodology II)**
- Learnt in depth on OOP and Java with some introduction to functional programming. Learnt about Java features such as wildcard, generics and Lambda and also how to write code following OOP paradigm. For Labs, create our own Maybe class that is suppose to work like the Optional class in Java standard library, create a shop programme and model customer, cashier, inventory interactions in Java.

**CS2040S (Data Structures and Algorithms)**
- Learnt the design and implementation of fundamental data structures (binary trees, heap, hashmap, graph) and algorithms (binary search, quicksort/quicksearch, DFS/BFS, Dijkstra, Kruskal, Floyd-Warshall, etc). For assignments, we work on implementing the Scapegoat tree data structure and design multiple algorithms and data structures for cases such as text prediction, maze solver, etc.
- Work as a tutorial assistant for this module. Preparing tutorial question for all class to use for one of the tutorial class. Taught a class of 16 students, grade their assignments/labs and provide feedback.

**CS3210 (Parallel Computing)**
- Learnt the fundamental of Parallel Computing. Learnt about the types of parallelism (Data Parallelism & Task Parallelism), parallel computation model (Task Pool, Pipeline, Fork Join, Message Passing), parallel architecture and algorithm (Bitonic Sort, Reduction). 
- There are 3 Assignments. 

First one is designing and implementing a simple world simulation (presented as a 2d grid where state of grid change per iteration based on state of neighbour) in C/C++ that attempt to maximise parallelism using OpenMP. Designed a model where a new grid is created per iteration. This allow fearless use of OpenMP to do calcuation of the new state per iteration as there is no data race (All modification is done in the duplicate grid).

Second one is on creating an algorithm to detect problematic pattern in a string consisting of 2 letter long words separated by space from a collection of problematic words in a database. The algorithm should use CUDA invocation to achieve high paralelization and exploit cache locality. Created an CUDA kernel where each CUDA thread is assigned a sequential portion of of the string to check. A CUDA kernel is invocated for each problematic word in database.

Last one is on scheduling tasks between multiple machines using OpenMPI and gather the result of the tasks into one machine. The aim to to achieve high parallelization by ensuring that machines stay idle for as little time as possible. Implemented a master worker model where one machine is assigned master which will schedule the task to all other worker models and also gather all the task results. 

**CS3211 (Parallel and Concurrent Programming)**
- Learnt about the design and implementation of concurrent systems where a set of processes collaborate by communication and synchronisation. Learnt about different concurrent systems model (Shared memory, Message Passing, etc), reasoning correctness or properties of a conccurency systems and parallel programs. Learnt about features of modern language (C++20/23, Go, Rust) to support writing concurrent codes.
- There are 3 assignments

First one is implementing an order/stock matching engine in C++23 that can handle buy, sell, cancel orders of different companies stock. Designed a system where orders are separated by the companies (i.e: store Google stock in one data structure, Amazon stock in another data structure). This allow threads processing different stock type to work in parallel due to them accesing different data structure. Use a linkedList with hand-to-hand locking between elements to store orders, allowing multiple threads to access the orders concurrently.

Second one is similar to the first assignment but to be written in Go and using only goroutine and channels to design a concurrent system. Use similar data structure such as assignment one but use a standard slice to hold the orders instead. Create a goroutine that is responsible for each data structure instance (Google orders will have its own goroutine) and have a goroutine be responsible for creation of new data structure and creation of that data structure handler goroutine. Have a fetcher goroutine that takes order from a connection and pass it to the data structure goroutine to do matching. This ensure no goroutine share any memory space,

Third one is a task scheduler systems in Rust that handle compute heavy task or I/O. Use the Tokio library to leverage asynchronous programming to be able to yield thread doing blocking I/0. Wrap all incoming task as a Tokio task, utilising the Tokio runtime to concurrently do multiple tasks and also allow await on blocking task to minimise idle threads.

**CS3217 (Software Engineering on Modern Application Platforms)**
- Learnt more advanced software engineering principles and designing modern application. Go through more rigorous analysis of software engineering project and work on self proposed project that require more complicated design architecture and reason the effectiveness and advantage of your design architecture. Work with another student to create a bartering system in Swift where users are able to make barter request and transaction. Create a custom state machine to handle the state of a transaction.

**CS3223 (Database Systems Implementation)**
- Learnt in-depth of the concepts and implementation issues related to database management systems. Learn about the underlying data structure that is used to store data/index (B+ trees vs Hash), caching & buffer manager database indexing, Relational Operator (Join, Selection, projection) algorithm, query optimiser, concurrency control and crash recovery (Aries).

- One assignment is to implement two different buffer manager policy within postgreSQL source code. One is an LRU policy and the other is a custom second chance-like policy.

**CS3241 (CS3241)**
- Learnt about the fundamental of Computer Graphics concepts and OpenGL. Learnt the entire rendering pipeline, homogenous matrix and matrix transformation, projection of object from world spcae to screen space,  illumination (Phong lighting, Ray tracing), texture mapping, rasterization, etc. 

- There are 4 labs

First one is to create a 2d windows where 2d circle of random size can be spawned on clicking any point in the window. Circles have collision and the window can be resized to different size while also ensuring all circles position are moved if they are outside the new window space,

Second one is to create multiple cars that are orbiting a spherical object. Camera should be able to move around the spherical object and zoom in and out of the object while staying locked to the centre of the spherical object

Third one is to do texture mapping on already provided objects. There is a glass table where we have to implement reflection using texture mapping. This is done by positioning a second camera below to capture the view of that camera, store it in a texture object, then map the texture on the top surface of the table

Last one is to implement Ray Tracing and do Phong shading on an already provided objects given an already provided light source. Light coefficient of all surfaces points are assigned through Ray Tracing which is used in the Phong shading.

Executables and demo video for the finished assignments can be found [here](https://drive.google.com/drive/folders/1tBYsgui6sMI_tQB_AKUQtuFUgBVpOu9_?usp=sharing)

**CS4225 (Big Data Systems for Data Science)**
- Learnt about tools to handle Big Data (Hadoop, Spark) and Data Streaming (Spark Streaming, Flink) and some of their underlying mechanism. Learnt about different nonSQL database type (Key-Value Store, Document Store, Graph, Column oriented) and their specific use cases. Also learnt how Spark and Flink achieve fault tolerance through writing backup into disk and doing checkpointing. 

- There are two assignment, one on hadoop and another on spark.

The first assignment is on reading a continuous stream of text message with metadata stored as a JSON object then update a dataset that contains count of appearance of every words by Singaporean texter and another one for United state user.

The second assignment it on using Spark to extract raw data from .csv file and transform into various dataframes to train a machine learning model to predict weather.

<style lang="stylus">

.courses-page
  background-color #FFF5E1

</style>