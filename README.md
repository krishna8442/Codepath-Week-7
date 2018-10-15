## Project 7 - WordPress Pentesting

1.(Required) WordPress <= 4.2 - DOM  Cross-Site Scripting (XSS)

Summary: 

  Vulnerability types: XSS

  Tested in version: = 4.2.21
        
   Fixed in version: 4.3

GIFWALKTHROUGH:(![dom xss vulnerability](https://user-images.githubusercontent.com/17356647/46977771-a5302a80-d092-11e8-92fc-be91a98563c4.gif)
)

Steps to recreate: Comment on wordpress post with the following string:

  Go to Appearances and Editor.
  Edit the Twenty Fifteen theme.
  Insert ''<SCRIPT>alert('XSS')</SCRIPT>'' in Comment.php
  Make a new post and Click on View Post.
  
2.(Required) WordPress <= 4.2 -  Cross-Site Scripting (XSS)

Summary:

Vulnerability types: XSS

  Tested in version: = 4.2.21
        
   Fixed in version: 4.3
   
   GIFWALKTHROUGH:![xss vulnerability](https://user-images.githubusercontent.com/17356647/46978126-a3b33200-d093-11e8-9b5b-e9a5c82c6ee8.gif)
   
   Steps to recreate: Comment on wordpress post with the following string:
   
   Click on Add a new post
   
   Enter the string "<IMG SRC="#" ONERROR="alert('XSS')"/>" in the title and write some random stuff in body of the post.
   
   Publish and view the post.
   
 3.(Required) WordPress <= 4.2 -  User-Enumeration.
 Summary:

  Vulnerability types: XSS

  Tested in version: = 4.2.21
        
   Fixed in version: 4.3
   
   GIFWALKTHROUGH:
   
   


