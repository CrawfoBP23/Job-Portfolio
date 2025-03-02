[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/6ISjSmU1)
# Homework 1 - Responding to Change

## Authors
1) Ivy Watson, wyb4kk, ivycw22
2) Arya Palla, wtk9wh, AryaPalla
3) Bailey Crawford, fej6xf, CrawfoBP23

## To Run

Run with filepath to the CSV file (program expects that first column is state names and second column is population) and the number of representatives desired, if no number is specified the program defaults to 435. 

## Contributions

List the primary contributions of each author. It is recommended to update this with your contributions after each coding session.:

### Ivy Watson

* Created DataObj class with constructors, getters, and setters to hold each row of data
* Made function to read in input from a CSV or Excel file & returned as ArrayList of DataObjs, throwing appropriate errors
* Takes file input from commandline, handles input errors and default values of representatives

### Arya Palla

* Created HamApportionment class with constructor that takes in initial ArrayList of type DataObj
* Implemented appropriate functions to calculate total population, allocate initial reps, and handle remaining reps for 
* each state
* Returns ArrayList with representatives parameter filled in for each state
* Implemented conditionals and default variable in main method for part C to handle when to use Huntington-Hill method

### Bailey Crawford

* Display results by iterating over the ArrayList of DataObj objects.
* Format the output to display each state's name and its corresponding number of representatives.
* Print the formatted results to the screen, following the format specified in the instructions.
* Implemented Huntington-Hill algorithm

## Issues

List any known issues (bugs, incorrect behavior, etc.) at the time of submission.
