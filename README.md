# PyProjects

Repository for my python projects
***
***1. Body Mass Index Calculator***

Made a BMI Calculator using python.
User provides *weight* and *height* and the code returns the calculated Body Mass Index (BMI)
> - Concepts used: Inputs, Control flow, Exception handling (try-except-finally)
> - Formula used for BMI calculation: **weight (in kgs) / (height)<sup>2</sup> (in metres)**

***2. Automatic File Explorer Sorter***

We all know how tedious of a work is decluttering your dump folder.
This python script automates it for you.

*Modules*
> - Modules used: OS and Shutil: `import os, shutil`
> - OS module allows user to interact with the operating system
> - Shutil module allows user to conduct some high level operations on file or collection of files, like removing or copying or moving files

*How does it work*
> - After importing the modules
> - User has to enter the folder path location in a variable named "path" it will be location of the folder where he wants the sorting to take place
> - Making use of the `os.listdir(path)` to list out the names of the files present in the location
> - User will pass the names of the folders he wants to sort the files into a for loop, the loop will check if the folder exists, if not then then it will create one
> - The code I've written is hard coded to sort `.ipynb` books to 'Python Files', `.xlsx` files to 'Excel Files' and `.jpg` files to 'Image Files' so for flexiblity you would need to add more elif statements to accomodate the files you want to sort
> - The 2nd for loop has an if-else within that what sort of extension the file has and checks whether the file is already sorted, if the file matches the extension and isn't already present in the folder it will be moved to the respective folder
