Git demo by teacher of BUET.
Initialize the project.  
Initialize project with git init.  




git init 
git add 
git commit -m "message"  
git status  
git log  







wsl  
ls  
ls -all  




cd .git  
ls  
logout  



git add-A ..........project er sobgulo file will be checked  
git add . -----------current directory er file gulo track rakhbe  
git add -u -------------age chilo emon file jegulo ke modify kora hoeche  
kebol tader kei  add korbe.  






jokhon cpp file create korlam and take compile korlam tokhon  
ekta .exe file create hoy ..but amr to .exe file ta commit  
korar dorkar nai  ...ei khetre amra ignore use korte pari.  


tokhon amra .gitignore file create kori  




akhon amra kono file e change korlam ....new kono commit korte chai na..  
commit ta ammend korbo just ..amader last comment ta edit hobe.  



git commit --amend -m "added some comments in hello.py"  
git log --oneline  




to keep the project in a repository  
git remote add origin https://github.com/shaDC24/Lecture-1-GIT-.git  
git push  
for setting the upstream  
git push --set-upstream origin main  
git push origin main  

amra chaile remove o koprte pari  
git remote rm main  
main is the name of the repository's branch  



git pull  
git fetch  
safer version of git pull is git fetch  





amara jokhon git checkout main die abr main branch e ashlam tokhon I lova cse,buet  
eta ar dekha jabe na.. ei jinish ta Feature-1 branch ei just add hoeche.  

abr main branch e kichu change korleo ta Feature-1 branch e jabe na.  







amra chaile branch deleete o korte pari.  
git branch -d <branch name>  
the above is thesafe delete  
git branch -D <branch name>  
the above is the force delete.  



Now i will mereg two branch  
as main is the main brach of my project and Feature-1 is just a added branch so i go to at first in the Feature branch  
1.git checkout Feature-1  
2.git merge master  
then merge conflict er jonno alert dibe.  
both rakhte chaile both accept dite hobe. 
3.git add -A  
4.git commit -m "merge conflict on hello.py"   
5.git checkout main  
6.git merge Feature-1  
there should be no conflict.  
7.feature-1 branch er kaj shesh.. now we can delete it.  
git branch -D Feature-1 
The command you ran only deletes the local branch.  
 If the branch still exists on the remote repository (e.g., GitHub, GitLab), it will still be visible there. To check whether the branch exists on the remote repository, you can use the following command:  
git branch -r   
If the branch still exists on the remote repository and you want to delete it from there as well, use this command:  
git push origin --delete Feature-1




kono untrack file thakle we can delete the file.
amra jodi commit na kore file ta deleete korte chai ..then  
git clean -f   
git clean -n  
the above command will show .. ki ki file deleete hote pare.  
git clean -d die amra je file remove hote pare tar diretiory dekhte pari  
git clean -di






ami ekta commit korlem... but oi commit ta amr dorkar nai
git revert HEAD  
then i will give a commit message  
git log --oneline  
die amra committed sob msg dekhte pabo  
git checkout ca9e639
ca9e639 is the name of the commit die amara abr ager commit e ferot jaite parbo.  

then   
git fetch  
git pull origin main  


amra jodi kono commit ke akdom delete korte chai then...  
git reset --hard 4f3c451  
4f3c451 is the hash value of the commit  
ei commit ta to erase hobei..porer commit  
gulo o erase hobe.  




git revert akdom erase kore na.. just new commit make kore  
git reset akdom erase kore fele   
kono tar jodi hiostory o na rakha jay tokhon amra resete --hard use kori.  



git diff ....ami ki ki change korchi ta dekhabe  ekta file e   
akhon ami jodi duite commit er moddhe difference dekhte chai  
git diff  e84e9e6 53de04d  
old then



git stash  
git stash list  
git stash pop  
git stash apply  
git stash drop  










