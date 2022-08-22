# ScyllaExercises
ScyllaDB Exercise projects for upskill knowledge 

Tasks to complete for first exercise 
1 - Create a 3 nodes cluster, with one datacenter 
each of the nodes in a different rack , dc:north, racks north1, north2, north3

2 - Create a keyspace with 3 tables, one of the tables using STCS, another LCS, another TWCS.

3 - Insert 10,000 records in each of the tables, using loop and cqlsh.

4 - In the TWCS table, when creating the table and inserting data use a time-window of 30 minutes and the data to expire with 1 hour TTL.
5 - Add a DC with 3 more nodes , each of the nodes in a different rack, dc: south, racks south1, south2, south3

6 - Install Scylla Manager

7 - Run repair using Scylla manager

8 - Decommission the old DC, keeping only the new created DC

9 - Add a node, decommission a node

10 - Then kill one of the nodes, destroy one of the containers (kill the seed node)

11 - Replace procedure to replace this node we've killed

Prerequisites
1) Linux
2) Docker
3) Docker-compose

First step was creating 3 separate nodes with docker run command for following output 
goodwinbg@scyllatraining:~$ docker run --name BrianExercise1 -d scylladb/scylla
a8d47166c0754feb8873d3f560606fee438b3a8382eb198348d90762ad3a9dca
goodwinbg@scyllatraining:~$ docker run --name BrianExercise2 -d scylladb/scylla
a3dd8d62b4aa9d9b4a289d0858c468453cccb23e132fbd09036afc2e6289931c
goodwinbg@scyllatraining:~$ docker run --name BrianExercise3 -d scylladb/scylla
79b4c4f9f8d8e154eb4d97e8178a636cce907a64f99ee6ae593e759610e23ee0
