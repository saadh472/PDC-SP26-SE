# Parallel and Distributed Computing Coursework

A chapter-based collection of Python concurrency and distributed computing exercises. Each chapter includes source examples, study notes, and recorded output.

This is a coursework fork of the shared PDC course repository. The code includes learning examples and textbook-based exercises. [Course repository](https://github.com/RameenAnwar/PDC-SP26-SE)

## Explore the coursework

| Chapter | Topics |
| --- | --- |
| [Chapter 1](Saad%20Hussain%2023FA-051-SE/Chapter%201/README.md) | Python foundations and serial, threaded, and process-based execution |
| [Chapter 2](Saad%20Hussain%2023FA-051-SE/Chapter%202/README.md) | Threads, locks, semaphores, events, conditions, barriers, and queues |
| [Chapter 3](Saad%20Hussain%2023FA-051-SE/Chapter%203/README.md) | Process pools, process synchronization, pipes, and queues |
| [Chapter 4](Saad%20Hussain%2023FA-051-SE/Chapter%204/README.md) | MPI communicators, collective operations, and virtual topology |
| [Chapter 5](Saad%20Hussain%2023FA-051-SE/Chapter%205/README.md) | Asyncio, futures, and thread or process executors |
| [Chapter 6](Saad%20Hussain%2023FA-051-SE/Chapter%206/README.md) | Sockets, Pyro4 remote objects, and Celery task queues |

Open a chapter's README for its file list, working directory, expected output, and additional setup requirements.

## Start with the standard-library examples

Install Python 3 and clone the repository.

```sh
git clone https://github.com/saadh472/PDC-SP26-SE.git
cd PDC-SP26-SE
```

Open the coursework folder, then run these examples from the indicated chapter's `Code` directory.

**Chapter 1**

```sh
python classes.py
```

**Chapter 3**

```sh
python process_pool.py
```

The classes example demonstrates attributes and inheritance. The process-pool example maps a square function across four worker processes. Both use Python's standard library.

Some examples retain older Python APIs or intentionally demonstrate blocking, timing, or synchronization behavior. Read the chapter notes before running them. Timing results depend on the operating system, interpreter, and available CPU cores.

## Additional environments

| Chapter | Additional requirements |
| --- | --- |
| 4 | An MPI runtime, such as Microsoft MPI, MPICH, or Open MPI, plus `mpi4py` and `numpy`. Launch MPI examples with the process count specified in the chapter notes. |
| 6 · Sockets | Separate server and client processes. Start the server first. |
| 6 · Pyro4 | `Pyro4`, a running Pyro name server, and the corresponding example server. |
| 6 · Celery | `celery`, an AMQP broker such as RabbitMQ, and a task worker. |

The chapter READMEs contain the example-specific commands. Run distributed exercises in a local learning environment with sample data.

## References

The related textbook is *Python Parallel Programming Cookbook – Second Edition* by Giancarlo Zaccone, published by Packt. Its examples and publisher documentation are available in the reference repository. [Publisher's code repository](https://github.com/PacktPublishing/Python-Parallel-Programming-Cookbook-Second-Edition)
