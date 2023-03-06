# What is Git and how it works

## What is it Git 

Git is a popular distributed version control system. With Git, developers can track changes to their code over time, collaborate with other developers, and easily revert to previous versions if necessary. Git allows developers to work on the same codebase simultaneously, with each developer having their own copy of the code on their local machine. Changes made by each developer can then be merged into a shared repository, allowing the entire team to stay up-to-date with the latest changes.

## How to make repository in Git

1. Open the terminal

2. Enter the command "git init" to initialize the repository. This will create a new repository in the current directory.

3. Add any files you want to include in the repository to the staging area using the command git add _filename_

4. Commit the files to the repository using the command "git commit -m 'Initial commit'" This will create the first version of your repository with the files you added in the previous step.

## Most usefull Git commands 

One of the most useful commands in Git is git status. This command shows the current state of your Git repository and helps you keep track of changes made to your files. It displays information such as which files have been modified, which files are staged for commit, and which files are not being tracked by Git.

# Other usefull commands

* **git add**: adds changes to the staging area

* **git commit**: commits changes to the repository

* **git push**: pushes changes to a remote repository

* **git pull**: pulls changes from a remote repository

* **git branch**: creates branches

* **git checkout**: switches between branches or restores files

* **git merge**: merges changes from one branch to another

* **git log**: displays the commit history

* **git diff**: shows differences between files or commits


* **git stash** - временно сохраняет текущие изменения, чтобы можно было переключиться на другую ветку или сделать другую работу, а затем вернуться к ним позже.


* **git reset** - отменяет изменения до указанного коммита.


* **git revert** - создает новый коммит, который отменяет изменения, внесенные указанным коммитом.


* **git tag** - создает тег для указанного коммита, который может использоваться для обозначения версий или моментов релиза.


* **git add**-p: эта команда позволяет вам выбрать, какие изменения вы хотите включить в коммит. Она также помогает вам просматривать изменения в коде и разбивать их на более мелкие куски.


* **git log** --oneline: эта команда выводит историю коммитов в однострочном формате, что упрощает ее чтение и понимание.


* **git checkout -b**: эта команда позволяет вам создать новую ветку и переключиться на нее одной командой.


* **git rebase**: эта команда позволяет вам перенести изменения из одной ветки в другую. Это может быть полезно, если вы хотите обновить свою ветку до последней версии мастера.


* **git commit --amend**: если вы заметили ошибку в последнем коммите, вы можете использовать эту команду, чтобы изменить его без создания нового коммита.


* **git push --force**: если вы сделали изменения в локальном репозитории, которые конфликтуют с удаленным репозиторием, вы можете использовать эту команду, чтобы принудительно заменить удаленный репозиторий своими локальными изменениями. Однако, будьте осторожны при использовании этой команды, так как она может привести к потере данных и проблемам в коллаборации.


## **как посмотреть значение предпоследнего коммита в ветке в git?**

Чтобы посмотреть значение предпоследнего коммита в текущей ветке в Git, вы можете использовать команду:


* **git log -n 2 --pretty=format:"%H"**
Эта команда выводит список двух последних коммитов в текущей ветке, где каждый коммит отображается в формате SHA-1 хеш-кода (который является уникальным идентификатором коммита). 
Затем вы можете **скопировать SHA-1 хеш-код предпоследнего коммита** (второй из списка) и использовать его для дальнейших действий, например, чтобы отобразить детали этого коммита с помощью команды **git show <SHA-1 хеш-код>**.


Если вы находитесь в другой ветке и хотите просмотреть _**предпоследний коммит в этой ветке**_, то перед выполнением команды git log необходимо переключиться на нужную ветку с помощью команды git checkout <имя ветки>


* **git checkout имя_branch2^** - посмотреть предпоследний коммит в ветке, например branch2, находясь в главной ветке


* **git log --pretty=oneline --all --graph** или просто **git log --oneline --all --graph** - посмотреть в графическом режиме в одну линию, не зависимо от того на какой ветке они сделаны

# Conclusion

## Knowing these commands and how to use them effectively can greatly improve your productivity and efficiency when working with Git.



### Learning these commands and their usage will help you effectively manage your Git repositories.




