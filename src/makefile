# Name: Terrance Parks
# Course:   CIS 145 Introduction to DevOps
# CRN:      45595
# Date: 2/15/2019
# Assignment: Make - Write a Makefile to Compile C Code

# This executes the ServerCountThree executable, creating it if necessary
# this run when you type "make test" at the command line
# if an error occurs the command line will tell you that target failed
# otherwise the result of the program's execution is shown

# MACROS
BUILD_DIR = ../build
DATA_DIR = ../data
EXE_FILE = ../build/ServerCountThrees
OBJ_FILES = ServerCountThrees.o readInt32BitLE.o
DAtA_FILE = threesData.bin
RUN_TEST = ./ServerCountThrees

# rebuild everthing from scratch and launch the executable ServerCountThrees
# if an error occurs the command line will tell you that target failed
all : clean test

# build the ServerCountThree executatable
# if an error occurs the command line will tell you that target failed
# otherwise the result of the program's execution is shown
exe : $(EXE_FILE)

# rule for builiding he ServerCountThree Executable
# if an error occurs the command line will tell you that target failed
# otherwise the result of the program's execution is shown

$(EXE_FILE) :	$(OBJ_FILES)
	mkdir $(BUILD_DIR)
	cp  $(DATA_DIR)/threesData.bin $(BUILD_DIR)/threesData.bin
	gcc -o $(EXE_FILE) $(OBJ_FILES) -I.
	chmod ugo+x $(EXE_FILE)


	

# compile and run the ServerCountThrees
# if an error occurs the command line will tell you that target failed
# otherwise the result of the program's execution is shown
test : exe
	cd $(BUILD_DIR); \
	$(RUN_TEST) 

# remove all generated files
# if an error occurs the command line will tell you that target failed
# otherwise the result of the program's execution is shown
clean :
	- echo 'Removing generated files'
	- rm *.o
	- rm -r $(BUILD_DIR)


