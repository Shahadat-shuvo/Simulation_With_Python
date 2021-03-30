# Simulation_With_Python


## Introduction

A queue is a line of people or things to be handled in a sequential order. It is a sequence of objects that are waiting to be processed. Queuing theory is the study of queues for managing process and objects. Simulation has been applied successfully for modeling small and large complex systems and understanding queuing behavior. Analysis of the models helps to increases the performance of the system.Simulation helps in understanding the behaviour of a queuing system and also obtain certain very useful parameters. 

## Queing onceptions

A Queue has to be maintained well to synchronize between the average waiting time and the idle time of server. A queuing model in which input, computation,transmission, storage and output are discrete in time field, is called discrete queuing model. Inreal life, a queue can be imagined as though to be of some people waiting in bank, usage of Atm machines or cash counter phenomenon.

## About this Project

In this project we are trying to simulate a single server banking system. We use Poisson and Exponential distribution for some random variables to generate interarrival time and service time respectively.

NOw, we have to consider a single server for simulate the bank system.

We have to initaial inter arrival time and service time first.

Consider poission as inter arrival time and exponential as service time generate 20 random values.

The generate arrival time, time service end, time service begin,waiting time,time spend in system & idle time step by step.

The value generating equations are given in the code section.

The single channel queuing model can be fitted in situations where the following seven conditions are fulfilled:

The number of arrivals per unit of time is described by poisson distribution. The mean arrival rate is denoted by λ.

The service time has exponential distribution. The average service rate is denoted by μ.

Arrivals are from infinite population.

The queue discipline is FIFO, that is, the customers are served on a first come first serve basis.

There is only a single service station.

The mean arrival rate is less than the mean service rate .

The waiting space available for customers in the queue is infinite.

## Quick Links
1. https://towardsdatascience.com/simulating-a-queuing-system-in-python-8a7d1151d485
2. Probability distribution. (https://www.datacamp.com/community/tutorials/probability-distributions-python?fbclid=IwAR1Van10TbSh-pfjCA_zS5F3AXI8fmWGrSgNZ0QdUwm-NwZG6Aacqd-qHOg)
3. A short research. (https://morioh.com/p/2a0717880c2d)

## Team Members

* Md Shahadat Islam. 
* Md Ashraf Udin.
* Thirtha Das.
* Ishrat Ishita.


**Lets first try and visualize the system


<img src="downloads/banking_simulate.png" alt="photo not available" width="70%" height="70%">

1. ***State Variables:*** describe the system at a particular time
2. ***Simulation Clock:*** Keeps track of time
3. ***Statistical Counters:*** Variables for storing statistical info about performance parameters
4. ***Initialization Routine:*** A subprogram or class that initializes the model at time 0
5. ***Timing Routine:*** A subprogram or a class that determines the next event
6. ***Event Routine:*** A subprogram or a class that updates the system when a particular event occurs

## Timing Routine

The timing routine decides which event occurs next by comparing the scheduled time of events and advances the simulation clock to the respective event. Initially, the departure events are scheduled to occur at time infinity(since there are no customers), which guarantees that the first event will be an arrival event.

<img src="C:/UsersShuvo/Pictures/Screenshots/time_routine.png" alt="photo not available" width="70%" height="70%">
