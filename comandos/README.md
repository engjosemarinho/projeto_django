engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda
$ git init
Initialized empty Git repository in C:/Curso_Python/Projeto Agenda/.git/

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)
$ git add .

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)
$ git commit -m "Primeiro Commit"
[main (root-commit) 7ad3b5c] Primeiro Commit
 8 files changed, 337 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 comandos/README.md
 create mode 100644 manage.py
 create mode 100644 project/__init__.py
 create mode 100644 project/asgi.py
 create mode 100644 project/settings.py
 create mode 100644 project/urls.py
 create mode 100644 project/wsgi.py

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)
$ ssh-keygen -t rsa -C "eng.josemarinho@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/engjo/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /c/Users/engjo/.ssh/id_rsa
Your public key has been saved in /c/Users/engjo/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:7+Ko52loGxQyS9L9d1oxm5sVIzqu6SF4JVPdKXG6vqE eng.josemarinho@gmail.com
The key's randomart image is:
+---[RSA 3072]----+
|        . .      |
| . .   . = .     |
|. = o . + * o    |
| o + +   + * o   |
|  . + o S = .    |
|   o + + * +     |
|  . +.. = +      |
|   .oooB.+       |
|   .oBE.o..      |
+----[SHA256]-----+

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)
$ notepad ~/.ssh/josemarinho.pub 

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)
$ ssh -T git@github.com
git@github.com: Permission denied (publickey).

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)
$ eval $(ssh-agent)
Agent pid 1298

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$ ssh-add ~/.ssh/josemarinho
Identity added: /c/Users/engjo/.ssh/josemarinho (engjo@pc_marinho_vmw)

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$ ssh -T git@github.com
Hi engjosemarinho! You've successfully authenticated, but GitHub does not provide shell access.

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$ git remote add origin git@github.com:engjosemarinho/projeto_django.git

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$ git add .

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$ git commit -m "Segundo Commit"
On branch main
nothing to commit, working tree clean

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$ git push origin main -u
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (11/11), 3.67 KiB | 751.00 KiB/s, done.
Total 11 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To github.com:engjosemarinho/projeto_django.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

engjo@pc_marinho_vmw MINGW64 /c/Curso_Python/Projeto Agenda (main)        
$