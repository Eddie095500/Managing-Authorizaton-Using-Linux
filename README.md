# Managing-Authorization

<h2>Objective</h2>

Review and edit user, group and other permissions on project files using Linux commands in a Bash shell.

<h2>Necessary Permission Changes</h2>

- Remove write permissions for other on file **project_k.txt**.
- Remove read permissions for group on file **project_m.txt**.
- Remove write permissions from user and group on file **.project_x.txt**.
- Add read permissions to group on file **.project_x.txt**.
- Remove executable permissions from group on directory **/home/researcher2/projects/drafts**.

<h2>Steps Taken</h2>

- Navigate to projects directory using `cd projects`.
- List non-hidden files and directories using `ls`.
- Reviewed permissions for non-hidden files and directories found in the **/home/researcher2/projects** directory using `ls- l`.

![1](https://github.com/DigitalWatchmen/Managing-Authorization/assets/164795269/fd8bbdf0-22cb-41a1-bd9e-51ddb60a7869)

- Reviewed permissions for hidden files and directories found in the **/home/researcher2/projects** directory using `ls -la`.

![2](https://github.com/DigitalWatchmen/Managing-Authorization/assets/164795269/24cedcb1-3354-4a78-9ea7-c2f7806f7b54)

- Removed write permissions from other on file **project_k.txt** using `chmod o-w project_k.txt`.
- Verified updated permissions on file **project_k.txt** using `ls -l project_k.txt`.

![3](https://github.com/DigitalWatchmen/Managing-Authorization/assets/164795269/a37a5313-dacb-48b5-9665-7796a7d0ae2e)

- Removed read permissions from group on file **project_m.txt** using `chmod g-r project_m.txt`.
- Verified updated permissions on file **project_k.txt** using `ls -l project_m.txt`.

![4](https://github.com/DigitalWatchmen/Managing-Authorization/assets/164795269/d6ba8517-8489-476d-af54-b56bc8c2e871)

- Removed write permissions from user and group & added read permissions to group on file **.project_x.txt** using `chmod u-w,g-w,g+r .project_x.txt`.
- Verified updated permissions on file **.project_x.txt** using `ls -la .project_x.txt`.

![5](https://github.com/DigitalWatchmen/Managing-Authorization/assets/164795269/63b57393-5051-41dd-bdb9-63975cb8f464)

- Reviewed permissions of directory **/home/researcher2/projects/drafts** using `ls -ld drafts`.
- Removed executable permissions from group on directory **/home/researcher2/projects/drafts** using `chmod g-x drafts`.
- Verified updated permissions of directory **/home/researcher2/projects/drafts** using `ls -ld drafts`.

![6](https://github.com/DigitalWatchmen/Managing-Authorization/assets/164795269/29a20915-bb21-4b9f-ac04-2f0cda8e3df2)
