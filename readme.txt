Read me:

How to run ‘Epidemic_simulator.py’:

1.	Through command prompt:
•	Go to the directory where python is installed through command prompt and execute following command:
•	Type command : python epidemic_simulator.py -bcrhj --delay=3 --nsim=1 --Beta=0.5 --Gama=0.3 airport.txt routes.txt

Note: Before running the above command, you must have following files present in directory.
a.	Simulator code file: epidemic_simulator.py
b.	Dataset files: airport.txt and routes.txt
c.	To analyze means to generate graph image of comparison of performance of strategies: analyze.py

1.	After completion of execution of simulation, the respective output files will get generate in folder.
2.	Now to generate graph image of comparison of performance of strategies, run only analyze.py.
Command: python analyze.py
3.	This analyze.py doesn’t required any arguments.

Note: Run analyze.py only after complete execution of main simulator code.

Arguments:
--bcrhj
If you want to run simulator for all strategies in single run, then give argument like above.
Here you can run simulator for 1 strategy to all five strategies in one run (simulation).
If you want to run simulator for specific strategy:
1.	For betweenness centrality strategy or algorithm, write only --b
2.	For clustering strategy or algorithm, write only --c
3.	For random  strategy or algorithm, write only --r
4.	For hub shutdown strategy or algorithm, write only --h
5.	For Jaccard coefficient strategy or algorithm, write only --j

--delay : This argument indicates the delay in simulation. In the above command delay=3 indicate delay of 3 days in simulation process.

--nsim: This argument indicates the number of simulations means for how many simulations you want to run simulator.

--Beta : This argument is optional. It indicates the probability of node’s state changing from susceptible to infected 

--Gama : This argument is optional. It indicates the probability of node’s state changing from infected to recovered.

airport.txt: This argument is the text file containing the airport data generated from original dataset.

Routes.txt: This argument is the text file containing the flights and air route data generated from original dataset.
