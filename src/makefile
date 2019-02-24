# Name: Terrance Parks
# Course: CS178 Build Automation for DevOps and QA
# CRN: 45595
# Date: 2/3/2019
# Assignment: Make - Write a Makefile to Compile C Code

# This rule tells make how to build Count3s from countThrees.c and
# readInt32BitLE.c

Count3s:	countThrees.c readInt32BitLE.c
	gcc -o Count3s countThrees.c readInt32BitLE.c


# This executes the Count3s executable, creating it if necessary
# this run when you type "make runCount3s" at the command line
# if an error occurs the command line will tell you that target failed
# otherwise the result of the program's execution is shown


runCount3s:
	./Count3s

