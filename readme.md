semantic release

release


now - 1.0.0

"chore(readme): expected version to be 1.0.1"

##

"chore(readme) : expected version to be 1.0.2"   no space after scope () :

develop 

now - 1.0.1

(without pre-release: true)
"chore(readme): expected version to be 1.0.2"   WORKED
"feat(readme): expected version to be 1.1.0"    WORKED
"feat(readme): expected version to be 1.2.0"    WORKED

develop released 1.2.0 and through PR 1.2.0 is released to main hasn't released any version 

(with pre-release: true)
"chore(readme): expected version to be 1.2.0-develop.1"   got 1.2.1-develop.1
"chore(readme): expected version to be 1.2.1-develop.2"   WORKED

develop released 1.2.1-develop.2 and through PR 1.2.1 is released to main as "main":true

check next version in develop
"chore(readme): expected version to be 1.2.2-develop.1"   got 1.2.1-develop.3 as package.json is not updated with 1.2.1 (develop)
"chore(readme): expected version to be 1.2.1-develop.4"  WORKED

develop released 1.2.1-develop.4 and through PR 1.2.2 is released to main as "main":true and updated in package.json(master/main) but not in develop

check next version in develop
"chore(readme): expected version to be 1.2.1-develop.5"   WORKED

Updated develop with main released tag 1.2.2 and check next develop pre-release version

"chore(readme): expected version to be 1.2.3-develop.1"    got 1.2.1-develop.6 as package.json manually updated with 1.2.2 (develop)

synced main to develop
"chore(readme): expected version to be 1.2.3-develop.1"   WORKED



## scenario 2
develop has 1.2.3-develop.2" and feat commit generated 1.3.0
develop has again with feat
