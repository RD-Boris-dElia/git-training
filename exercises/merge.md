# Merge some code

Or the beginning of the problems

For this exercise, we will need to work in pairs to simulate potential real problems (merge conflicts). Let's call them John and Lisa for this exercise.

Merge conflicts occur when competing changes are made to the same line of a file, or when one person edits a file and another person deletes the same file.

## First case

Let's imagine a simple example where John is working on improving feature1 from your application :

1. Change the line 'GET and FILTER data from the DB' to 'GET and FILTER data from the DB then format the data for the client'.
2. commit
3. push

In the meantime, Lisa is fixing a bug on the same feature :

1. Change the line 'GET and FILTER data from the DB' to 'GET and FILTER data from the DB but without bugs please'.
2. commit
3. push

If both pushes happen on the same branch, you will have what's called a merge conflict. A merge conflict is best resolved manually on your local environment. 

Here's how the conflict looks :
```
# This is my first feature

<<<<<<< HEAD
GET and FILTER data from the DB but without bugs please
=======
GET and FILTER data from the DB then format the data for the client
>>>>>>> 1fe434371b9dc1171d091fe75e2bc3b89f134252

```
======= is the conflict separator between the 2 bits of code that caused the conflict

<<<<<<< is the entrypoint of the conflict with the source (HEAD) of the first part of the code then the conflicting code from that source.

\>>>>>>> is the exit of the conflict with the hash from the commit introducing the conflict. 

The easiest way to resolve the conflict is to use your IDE. Your result should look like this :
```
# This is my first feature

GET and FILTER data from the DB but without bugs please then format the data for the client
```
