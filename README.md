## Project 7 - WordPress Pentesting

1.(Required) WordPress <= 4.2 - DOM  Cross-Site Scripting (XSS)

Summary: 

  Vulnerability types: XSS

  Tested in version: = 4.2.21
        
   Fixed in version: 4.3

GIFWALKTHROUGH:(![dom xss vulnerability](https://user-images.githubusercontent.com/17356647/46977771-a5302a80-d092-11e8-92fc-be91a98563c4.gif)
)

Steps to recreate: 

  Go to Appearances and Editor.
  Edit the Twenty Fifteen theme.
  Insert ''<SCRIPT>alert('XSS')</SCRIPT>'' in Comment.php
  Make a new post and Click on View Post.
  
 Affected source code:
  
2.(Required) WordPress <= 4.2 -  Cross-Site Scripting (XSS)

Summary:

Vulnerability types: XSS

  Tested in version: = 4.2.21
        
   Fixed in version: 4.3
   
   GIFWALKTHROUGH:![xss vulnerability](https://user-images.githubusercontent.com/17356647/46978126-a3b33200-d093-11e8-9b5b-e9a5c82c6ee8.gif)
   
   Steps to recreate:
   
   Click on Add a new post
   
   Enter the string "<IMG SRC="#" ONERROR="alert('XSS')"/>" in the title and write some random stuff in body of the post.
   
   Publish and view the post.
   
  Affected source code: 
   
 3.(Required) WordPress <= 4.2 -  User Validation and Enumeration Vulnerability
 Summary:

  Vulnerability types: XSS

  Tested in version: = 4.2.21
        
   Fixed in version: 4.3
   
   GIFWALKTHROUGH:![vulnerabiliy 3](https://user-images.githubusercontent.com/17356647/46978263-1e7c4d00-d094-11e8-8029-8ea3d67f1a31.gif)
   
 Steps to recreate:
 
 Go to Kali Linux
 
 When you try to log in using some random username, it says no username found.
 
 Try username as admin and some random passoword. It says password is wrong.
 
 So that's a leak of username.
 
 Make a file called newfile.txt with words shown in the gif image ie. password, admin,12345,admin,hacker123,Hacker@123,hack_password
 
 Go to Kali Linux and enter the following command " wpscan --url http://wpdistillery.vm  -- wordlist (location of your wordslist file) --username admin" and run the command.
 
 It wil enumerate the users and displays the username and passwords .
 
Affected source code: 

   
   


