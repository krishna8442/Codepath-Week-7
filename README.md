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
   
   GIFWALKTHROUGH:

