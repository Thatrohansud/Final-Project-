# Final-Project-
This is for unit 2 
 For my unit 2 final I wanted to create a pizza delivering SDV. This SDV will use all concepts we learned about in Unit 2 uncluding the utilization of a list to track where the SDV went, Image Proscessing to Detect Objects, For Loops and Forever Loops used to repeat the SDV's code when reacting to an object, the use of conditionals through if-then statements, if else statements, and if-else-elseif statements in addition to Booleans and Variables in relation to tracking the SDV on the 2D list. Here is an in depth explanation of how all of this works in the programs with screenshots: 

Step 1: I utilized the SDV's vision sensor to track if there is an object or not. Below is the maze the SDV will be navigating. The start is where ths SDV is standing and the end is the red checkered block. The code states that if the front image tracking sensor is not near an object (in this case a red wall) it will drive forward 200 meeters. This uses the basic if-then conditional



![image](https://github.com/user-attachments/assets/e51ce5fe-a0b7-4626-80f1-82e44ef54391)
![image](https://github.com/user-attachments/assets/56601702-aeea-42a6-97f5-0cd37c134737)

Next: What happens when the SDV is in front of an object. The below code states how if the front sensor is near an object (using vision sensor) it will detect that and turn 90 degrees. This is where the first loops are used. I coded the program so that it keeps on turning 90 degrees until the front sensor does not detect an object then drives forward. An additional forever loop is put over the entire code so that the SDV keeps on repeating this proscess. This also uses conditionals such as if-then, if-else, and if-else-elseif (elif in python)


![image](https://github.com/user-attachments/assets/4cd6fd91-de1d-4ef1-bfed-95d06d598f66)

Now you may think this code is enough for the SDV to navigate the maze and deliver the Pizza. While the SDV can navigate the maze by avoiding objects it will be directionlessly moving throughout and eventually get stuck as seen below. This is where we use lists, variables, and booleans. 



![image](https://github.com/user-attachments/assets/886cb64b-9565-4a11-8f9a-c3a620d98085)



First we utilize lists and variables, I have created a 2d list to represent the maze with the 0's being blocks in the maze and the 1's being the path the SDV should take to complete and 2 being the destination. The row and column variables indicate the placement of the SDV in regardance to the 2d list. They are the lenght of the list in rows and columns which are numerically 8 but in code 0 is counted as a number so their value will be 7 (you can't explicitly see that in the program)


![image](https://github.com/user-attachments/assets/d4bdfb19-32e8-4080-b6c3-7276c61255ec)

Now using the 2D list we have creaed we have tied in booleans. The boolean named onpath is set to true when the SDV is on a block which corresponds with the letter 1 on the 2d list. And the boolean is set to false when it corresponds to anything else. Now combined with the vision sensors code for reacting to objects and the SDV's internal sense of direction it can navigate the maze all the way to the checkered red block where it keeps on spinning in circles. 

![image](https://github.com/user-attachments/assets/19e0ed82-bd56-4b41-8127-064fbb4b33e1)

The final edit we will make to the code is we will terminate the code using the stop driving block when the block (finishing block) correlating to the list which is noted as 2 is driven on. Now the code works normally: 

![image](https://github.com/user-attachments/assets/bb49164a-8a7c-450f-a470-fdf23da2a485)



Now moving on to Final Project Unit 3: 

For this I will be expanding the student registration activity for 3.2.4. Currently my code looks like this. The code implements a basic student course registration system across three Python files: course.py, student.py, and course_registration.py. In course.py, various courses (e.g., "Algebra I", "Earth Science") are defined as objects, while student.py features a Student class that assigns unique IDs, stores names and courses in lists, and provides methods like get_first_name, get_last_name, and add_course, utilizing Python slices (e.g., [0] for first name, [-1] for last name) to parse names. The course_registration.py script creates three students—"Jill Smith", "Bill Edwards", and "Timmy Jones"—assigns them courses, stores them in a list, and prints their details using iteration and direct list indexing (e.g., student_list[2]). Key concepts include classes, objects, initialization, string representation, methods, lists, loops, imports, static variables, and python slice (learned outside of class). Everything covered in lesson 3 before 3.2.5 is here. I am going to make a simulation (similar to the rock paper sszicors game) could simulate student enrollment over a semester by also using randint function to iterate between lists. 

![image](https://github.com/user-attachments/assets/6f5b04af-37e7-44ad-933a-232aeb2faa2b)
![image](https://github.com/user-attachments/assets/08d360df-5721-4ced-9ec5-3a74199eb8f9)
![image](https://github.com/user-attachments/assets/c7c6a6e1-82c0-4ca4-b123-e87064563a30)





