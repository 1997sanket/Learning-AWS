# Using Linux to code and deploy c++ programs in GitHub

Hello people, today I'm going to show you how to use a Linux OS to code and deploy C++ on git.
We are going to use a very basic code, the infamous *Hello, World* code, haha.
---
## Steps to follow

	       1. Any Linux OS, preferablly Ubuntu.
 
	       2. Make sure you have GitHub installed on your OS. If install using the command **sudo apt install git-all**

	       3. After this, clone your Git repository, just write **git clone <address>**, this address you will get from your GitHub repo.

	       4. Now open the inbuilt text editor and write your code. Type **vi YourFileName.cpp**, inside this press **i** and then write your code and to 			save and exit first press **Esc button** to get out of editing modeand then type **:wq**.

	       5. Now type g++ **YourFileName.cpp -o YourOutputName**, and press enter. Thats it your 2 files are ready.

	       6. Now to check and run once type **./YourOutputName**

	       7. Now your files are ready and you just have to push it in GitHub.

	       8. Now type **git add -A** to add your file to your project.

	       9. Before commiting you need to tell Git who you are to do this type **git config --global user.email <your email>** 
		  and ***git config --global user.name "<full name>"
	    
               10. Now you can commit by using **git commit -m "<Descriptive message"**

	       11. Now type **git push**

