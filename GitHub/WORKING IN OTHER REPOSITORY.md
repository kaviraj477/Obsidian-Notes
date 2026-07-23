*WORKING IN SOMEONES REPOSITORY IN GIT AND NEED TO GET IT IN LOCAL:* [[GitHub]]

i) Git Bash here-->git clone "repository URL (of someone) "

ii) Close Git

iii) Open Git inside newly imported / cloned folder

iv) TO IMPORT IT IN ECLIPSE:        
    Eclipse IDE--> File--> import-->existing maven project--> cloned file path--> Finish
    
v) Open GitHub --> create new branch

vi)  FETCHING : *(to update any branch added/removed along master branch)*

1. METHOD#1:   *ECLIPSE IDE*
    Eclipse IDE -->Right click on that project-->team--> fetch from origin 

2. METHOD#2:  *GITBASH* 
    open that project folder-->git bash-->git fetch-->git checkout BranchName (we created in GitHub)-->close-->our branch name should updated or switched in eclipse
   
vii) open eclipse--> create new package in newly imported project-->create                  class--> create java program

vi) PUSHING TO ECLIPSE TO GITHUB:

1. METHOD#1: *via eclipse ide*
    after creating new program we should push that to remote:
    right click (project)-->team-->commit-->choose your progrom in unstaged changes-->hover and select add buuton -->commit message-->commit and push-->[^1]Login if asked-->
            
2. METHOD#2: *eclipse + gitbash*
    .....-->commit-->open project folder-->git bash-->git push 

3. METHOD#3:
   open project folder-->git bash--> git add . -->git commit -m "..."-->git push (or) git push origin branchName (ensure your branch name is visible in gitbash here)

vi) *PROCEDURE ON HOW TO LOGIN *

[^1]: GitHub Login Password
	
	1. User : This is your GitHub username.
	2. Password : Open a web browser, go to github.com, and log into your account (you can use your Gmail to log in here like normal).
	3. Click your profile picture in the top-right corner and select Settings.
	4. Scroll all the way down the left-hand menu and click on Developer settings (at the very bottom).
	5. On the left, click Personal access tokens, then select Tokens (classic).
	6. Click the Generate new token button (choose "Generate new token (classic)" if prompted).
	7. In the Note field, type something like "Eclipse IDE" so you remember what it is for.
	8. Look at the list of checkboxes under Scopes. Find the one named repo (Full control of private repositories) and check that box. This gives Eclipse the permission it needs to push your code.
	9. Scroll to the bottom and click Generate token.
	10. Click the blue link that says "Send a code via email".
	11. GitHub will now show you a long string of random characters. Copy this token immediately 
	12. Go back to Eclipse and paste that long token into the Password box.
	13. Check the box that says Store in Secure Store (this saves the token so Eclipse won't ask you for it every single time you push code).
	14. Click Log in. Your code will now successfully push to your GitHub repository!
