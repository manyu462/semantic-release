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
"chore(readme): expected version to be 1.2.2-develop.1"   
