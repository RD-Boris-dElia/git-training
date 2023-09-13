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

