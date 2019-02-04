# Data Pipelines
The purpose of any software application is to receive some inputs, process them and share present the output to a user or to another application. 

Data pipelines are that category of applications that process this data in a sequential manner. A stage in the pipeline receives data, process it and passes it on to the next stage. After processing a given input it is ready for the next input. The execution block that does the processing may differ depending on the use case, but the data keeps moving through these blocks in a predetermined order. A majority of software applications typically fall into this category. 

## Typical Challenges
1. All the possible configurations are not known in advance at the time of design. 
2. Tight coupling: Developers tend to ignore the future adaptability of the design and may create a very tight coupling between the blocks. It becomes extremely difficult to remove a single block without disturbing others. 
3. Execution bottlenecks, use of mutexes and other synchronization primitives slowly creep into each module and eventually result in deadlocks as the application grows. 

