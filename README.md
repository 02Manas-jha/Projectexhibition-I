# Bank Queue Simulation Project

## Overview

Queues are an integral part of everyday life, evident in places like supermarket checkout stations, help desk call centers, manufacturing assembly lines, wireless communication networks, and multitasking computers. Queuing theory provides a rich and useful set of mathematical models for analyzing and designing service processes where there is contention for shared resources. This project explores both the theory and application of fundamental and advanced models in this field.

## Project Description

This project focuses on simulating a queueing system in a bank setting using a numerical dataset. We will use Python libraries such as NumPy, Pandas, and SimPy (a process-based simulation framework). The simulation will illustrate how a queueing system operates in a bank with the following conditions:

- The bank has two tellers.
- Customers arrive at the bank about every 3 minutes on average, following a Poisson process. This arrival rate is assumed but should ideally be modeled from actual data for accurate results.
- Customers wait in a single line for an available teller, creating an M/M/2 queueing system.
- The average service time is 1.2 minutes for the first teller and 1.5 minutes for the second teller, both following an exponential distribution.
- When both tellers are idle, customers choose either one with equal probabilities.
- If a customer enters the bank and sees four people waiting, they leave with a probability of 50%.
- If a customer enters the bank and sees five or more people waiting, they leave with a probability of 60%.

## Key Concepts

### Fundamental Models
- **Single- and Multiple Server Markov Queues**: These models deal with systems having one or more servers where arrivals and service times follow Markov processes.
- **Bulk Arrival and Bulk Service Processes**: These models consider scenarios where multiple entities arrive or are served at the same time.
- **Priority Queues**: These models handle systems where entities have different levels of priority for service.

### Applications
While the emphasis of this project is on communication networks and computer operations, examples from transportation, manufacturing, and the service industry are also relevant.

## Simulation Tools

### Libraries Used
- **NumPy**: For numerical operations and handling arrays.
- **Pandas**: For data manipulation and analysis.
- **SimPy**: For creating the process-based simulation of the queueing system.

## Getting Started

### Prerequisites
- Python 3.10
- Libraries: NumPy, Pandas, SimPy

### Installation
To install the necessary libraries, use the following commands:
```bash
pip install numpy
pip install pandas
pip install simpy
```

### Running the Simulation
1. Clone the repository.
2. Navigate to the project directory.
3. Run the simulation script:
   ```bash
   python bank_queue_simulation.py
   ```

### Expected Output
The simulation will provide insights into:
- Average wait time for customers.
- Average number of customers in the queue.
- Probability of customers leaving due to long wait times.

## Conclusion

This project demonstrates how queuing theory can be applied to simulate and analyze a bank's customer service process. By understanding and optimizing these models, we can enhance service efficiency and customer satisfaction in various real-world applications.

## References

- "Introduction to Queueing Theory" by Robert B. Cooper
- "Queueing Systems" by Leonard Kleinrock
- [SimPy Documentation](https://simpy.readthedocs.io/en/latest/)

#ToDos
- Using simpy for stimulations and visualizastions.
