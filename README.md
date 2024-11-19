# devOps
DevOps Practice
git :
welcome to devops

this is second class of devops
git config --user.name "name of user"
git config ---user.email "manilid"

git clone

check branch : git branch

change branch : git checkout branch

create and change branch : git checkout -b branch

saved to staging : git add <filename or *>

save to local repo : git commit <filename or *> -m "<commit-messeage>"

local to remote repo : git push

remote to local : git fetch or git pull

diff between git fetch and git pull : 
git fetch: download from remote to local but not saved in local ( merge == saved)
git pull : download and saved in local (download + merge)

git reset --soft HEAD~1 : revert changes but still keeps in staging area for review

git reset --hard HEAD~1 : resvert changes and deleted recently changes also 

git branch <branch_name>

git cherry-pick <commit-id> : it will apply that commit changes to current branch 

common questions:

what is diff between git pull and git fetch

what is branching stretegy your following in your project?
main: always ready to deploy branch and we are configure this branch with merge checks so that no one can directly change the code inside main branch with out PR.
release : before release we are creating a release branch form dev which is moved for production
features: when ever devoper need to fix somthing or add somthing he needs to create branch from dev branch , after completion of his changes he needs to create Pull request with dev/main branch.
            after PR , we need to get aproval from reviewers than only he can merge his changes to dev/main.

how to reset changes in git branch ?
we can follow 2 ways

    git reset --soft HEAD~1 : revert changes but still keeps in staging area for review

    git reset --hard HEAD~1 : resvert changes and deleted recently changes also 

if i want to apply one specifuc commit from another branch how can I do ?

by using git cherry pick we can apply specific commit to current branch

git cherry-pick <commit-ID>


MAVEN:
steps to install :
    if linux : yum install maven
    ubuntu: apt-get install maven
    windows: download package from https://maven.apache.org/download.cgi
    set env : , MAVEN_HOME = installation directory like C:\Program Files\Maven\apache-maven-3.9.5
    add path : %MAVEN_HOME%/bin
    verify installation using , mvn -v
-----------------------------------------------------------------------------------------------------------

maven is used for java projects >> .jar

Maven Life Cycle:
-----------------------------------------
mvn compile
mvn build
mvn test
mvn package
mvn verify
mvn install
mvn publish
----------------------------------
mvn POM.xml
-----------------------------------
Project object model file
 set of instructions for mvn build and run 
 and dependences and just like blue print of project 

mvn archetype:generate : templates
select one template: 2201
version of template: 


::JENKINS::
----------------------------------------------

download from : https://www.jenkins.io/download/thank-you-downloading-windows-installer-stable/
Environment variables:

JENKINS_HOME=<installation_path>
Path add = %JENKINS_HOME%/bin

pulgins: ( plugin and play type of working)

    each tool treat as plugin and install as plugins 