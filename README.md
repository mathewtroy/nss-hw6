# :label: Homework from the subject Design of Software Systems  (NSS)

**Code**: B6B36NSS \
**Name**: Design of Software Systems/ Návrh softwarových systémů \
**Faculty**: Faculty of Electrical Engineering/ Fakulta elektrotechnická \
**Department**: 13136 - Department of Computer Science/ Katedra počítačů 

## :label: Assignment
<details><summary> Show more </summary>

**1) Vytvorte readme podle markdown dokumentace:**
https://docs.gitlab.com/ee/development/documentation/styleguide/ <br>

**Obsah readme:** (každý bod je kapitola)
- nazev aplikace (nikoli napsane textem :) )
- list autorů
- list technologii
- popis
- nazev instalace
- copyright



**2) Vytvorte 2 větve (test1, test2) z master větve a vypište seznam všech větví** <br>
Look at list all branches <br> `git branch -a`

PS D:\study\2023-2024-leto\nss\hw\06\git> git branch -a <br>

  main                              
  test1                             
  remotes/origin/HEAD -> origin/main
  remotes/origin/main               
  remotes/origin/master             
  remotes/origin/test1              
  remotes/origin/test2    

**3) Na test1 vytvorte test.txt s textem:**
huraa NSS :) a dostaňte commit na repo gitlabu (at není jen lokalne). 
Zaroven ukazte ze mate vse commitnute lokalne. <br> 

**4) Na test2 ziskejte dany commit** (metodu necham na vas) <br>

Switch to branch test2 <br>
`git checkout test2`

Looking for hash of the commits from branch test1 <br>
`git log test1`

Copy commit from branch test1 <br>
`git cherry-pick 24968b53c91f4b42d3176332e7d3219d3ca8abba`

**5) Vypiste commity pomoc git log** <br>
`git log`

**6) Na test2 pridejte test2.txt** ale chcete aby v historii byl \
pouze 1 commit se zpravou která byla v minulem commitu (je vic spravnych reseni) <br>

Add to index <br>
`git add test2.txt`

Commit <br>
`git commit -m "added test.txt"`

Run interactive rebase <br>
`git rebase -i HEAD~2`

First line should have pick, second should have squash <br>
`pick 77777b7 added test.txt`
`squash a1b2c3d some other commit message`

Then use this for completing rebase
`git rebase --continue`

**7) Na test2 smazte poslední commit** 

Soft reset <br>
`git reset --soft HEAD~1`

Use push send <br>
`git push --force`

**Best practise:** <br> 

**Co commitovat** <br>
-zdrojaky, soubory zdroje dat... 

**Co necommitovat**
- hesla, api klice... \
- .idea.. 
- systém files \
- temporary files\
- davame do .gitignore\

</details>


# :label: Application Name

*Place your application name here using a large-sized font.*

## :label: List of Authors

*List the names and roles of the people who have contributed to this application.*

## :label: List of Technologies

*Enumerate the technologies, languages, frameworks, and tools used in the development of this application.*

## :label: Description

*Provide a detailed description of what the application does, its features, and its use cases.*

## :label: Installation Name

*Detail the step-by-step instructions on how to install and set up your application.*

## :label: Copyright

*Include the copyright information, licensing details, and any legal information associated with the application.*



## :label: Contacts

**Teacher:** Jiří Šebek <br>
**Author:** Aleksandr Kross  <br>
:email: **[If you have questions text me](mailto:krossale@fel.czut.cz)**
