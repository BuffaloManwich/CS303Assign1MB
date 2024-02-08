# CS303Assignment1Pt1MB
# This is an assignment to build array functions that replicate some of the functionality of vectors.
# The main program will read the inputs from the file "A1input.txt" into an integer array. Each line from file is a single array.
#
# This will require a user screen to choose the operation from a list. It will require a read array option, and manipulate array menu. The manipulate menu will have "add int", "del int", "search for int", and "change index val".
#
# Creating new arrays will not allow for variable size entry ie newArray[i+1], and arrays cannot be passed by reference. In order to accomplish the assignment without that functionality, I will need to exploit the fact that the integers in the file number 10 or less. I will also exploit the fact that none of the inputs are zero, and initialize the array to size [15] with zero values as default empty.
#
# The try/catch block for part 2 has been built into the stoi() function and file opening process. The interruptive nature of throwing and catching the errors make it difficult to incorporate elsewhere in the program. Guardrails are in place to prevent problematic inputs.
#
# The int* feature is central to the operating of the program. Unfortunately, this only allows one array to be held for access. Each loading of a new array overwrites the previous array.
# For this reason I have restricted writing access to 14 of the 15 available entries. There are many loops and a couple of try/catch blocks to prevent issues.
#
# The way to use the program is simple. Open in Visual Studio and Run.
# A menu will show in terminal. Use the numeric options for navigation. Start with option "1". Then modify/print as wanted. Option "4" exits the program.
# 
# NOTE: Integer array is not loaded automatically!
# Must use option "1) Read new int array from file" before entering the print or modify options.
# Without reading in an array, the print and modify may behave unpredictably or crash the program.
# 
# 
# 
# All functions currently work as intended on Visual Studio locally. Edge cases and possible errors have been addressed/prevented as best as I can predict/anticipate.
# 