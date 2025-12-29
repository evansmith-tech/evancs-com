---
layout: default
title: Reading List
---

### Books & Core Foundational Texts

* [Designing Data-Intensive Applications]()
    - Essential for understanding the trade-offs between B-Trees and LSM-Trees, which dictates how hardware I/O patterns (random vs. sequential) affect application performance.
* [Database Internals]()
    - Provides a low-level blueprint for storage engines, specifically how to structure on-disk binary formats and page layouts for efficient retrieval.
* [Transaction Processing: Concepts and Techniques]()
    - The "bible" for learning how to ensure data integrity (ACID) during hardware or power failures, which is the primary responsibility of a storage layer.
* [Readings in Database Systems (The "Red Book")]()
    - A historical perspective on why certain storage architectures won over others, offering insight into the long term evolution of data persistence.
* [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/)
    - Specifically the persistence and virtualization section, it demystifies how the OS interacts with storage controllers/drivers/etc, and how virtualized devices work. 
* [The Design and Implementation of the FreeBSD Operating System]()
    - A masterclass in Unix File System (UFS) architecture that teaches the complexities of metadata management and inode allocation.
* [The Art of Computer Systems Performance Analysis]()
    - Equips you with the statistical rigor needed to distinguish between a genuine storage bottleneck and transient system noise during benchmarking.

---

### Papers & Digital Resources

* [Dremel Paper](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36632.pdf)
    - Databases are the primary consumers of storage, so understanding how they query data helps engineers optimize the underlying physical layout for columnar access.
	- Fun paper. Databases tend to be the major consumer of storage in cloud, and also their good papers tend to be (in my opinion), a decent window into how storage, networking, user expectations, and databases concepts comingle with each other. I think its good to have an idea of what the database customer is trying to solve, especially when you rarely get a chance to use the product you yourself create.
* [CMU Database Group Youtube](https://www.youtube.com/@CMUDatabaseGroup/videos)
    - High-quality lectures on modern storage trends like NVMe-optimization and persistent memory integration.
* [FIO Output Explained](https://tobert.github.io/post/2014-04-17-fio-output-explained.html)
    - A practical guide to interpreting the industry-standard tool for storage benchmarking, ensuring you understand latency percentiles over simple averages.
* [I/O Plumbing Tests with FIO](https://blog.purestorage.com/purely-technical/io-plumbing-tests-with-fio/)
    - Focuses on the "plumbing" of the Linux I/O stack, helping engineers identify whether performance issues reside in the application, the kernel, or the hardware.
* [Storage Performance Basics for Deep Learning](https://developer.nvidia.com/blog/storage-performance-basics-for-deep-learning/)
    - Explores the modern shift toward high-throughput, low-latency storage requirements driven by GPU-heavy workloads and massive datasets.

---
