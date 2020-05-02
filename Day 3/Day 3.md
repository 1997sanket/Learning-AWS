# Things covered
1. Basic Linux commands
2. Creating RDBMS on AWS and accessing it using our local PC

--- 

* **Basic linux commands**

ls	--> Lists directories/file in current directory
cd	--> Change directory
pwd	--> prints working directory
mkdir	--> Makes new directory
vi	--> Alternative to notepad of windows ( inserting data using 'i',  'Esc button' for back, ':w' for writing , ':q' for quitting, ':wq' for writing and quitting


Absolute path	--> Complete ancestory/path of a folder with root
Relative path	--> uses <dot> ( . -> same directory,  .. -> parent directory,  ../..  -> parent directory's parent directory)
 


Both have its advantages and disadvantages

Relative path is used for making our code more dynamic, for eg in file handling, we can use relative
path in our project folder, so that various team members can use the same code, without having the
need to edit for each memeber as each member can add project folder in different drives (C, D etc)

---

* **Creating RDBMS on AWS and accessing it using our local PC**

Created MySQl rdbms on AWS and accessed it on local PC
Added one inbound rule in security for port 3306 keeping source 'Anywhere'
stopped the service since it could be more costly.


**Note** : When not using stop the services, most importantly before going to sleep.


