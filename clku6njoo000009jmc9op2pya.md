---
title: "Day- 3: Basic Linux Commands"
datePublished: Wed Aug 02 2023 20:30:54 GMT+0000 (Coordinated Universal Time)
cuid: clku6njoo000009jmc9op2pya
slug: day-3-basic-linux-commands
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/4Mw7nkQDByk/upload/92136a5e5c3e4d28fb0aa48bdfa40e59.jpeg
tags: linux-for-beginners, linux-basics, linux-commands, 90daysofdevops, 90daysofdevops-devops-projectdevelopment-nonitbackground-github-docker-cloudplatforms-ec2-aws-elasticbeanstalk-lambdafunctions-devopspipelines-terraform-jenkins-docker-devsecops-scm-git-gitlab-bitbucket-buildtools-griddle-maven-ant-msbuild-monitoringtools-prometheus-grafana-ansible-ai-chatgpt-valueaddition-realworldproblems

---

In this article, we will explore various file and directory manipulation tasks in a Linux-based terminal.

* *Viewing File Contents:* To view what's written in a file (fruits.txt)
    

```bash
[~]$ cat fruits.txt
```

*Changing Access Permissions:* To change the access permissions of files (for example, make the file executable only for the owner)

```bash
[~]$ chmod u+rwx,g-rwx,o-rwx filename # Replace 'filename' with the actual file name
[~]$ chmod 700 filename # Replace 'filename' with the actual file name
```

| <mark>Bit</mark> | <mark>Purpose</mark> | <mark>Octal Value</mark> |
| --- | --- | --- |
| r | Read | 4 |
| w | Write | 2 |
| x | Execute | 1 |

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">while using octal code like <strong>xyz</strong>, where <strong>x</strong> gives permission for the <strong>user</strong> or <strong>owner</strong>, <strong>y</strong> talks about <strong>group</strong> &amp; <strong>z</strong> tells about <strong>others</strong>.</div>
</div>

Examples for more clarity:

* Full access for Owner, add read, remove execute for group and no access for others
    

```bash
[~]$ chmod u+rwx,g+r-x,o-rwx test-file  
```

* Provide full access to Owners, group and others
    

```bash
[~]$ chmod 777 test-file  
```

* Provide Read and execute access to Owners,groups and others
    

```bash
[~]$ chmod 555 test-file  
```

* Read and Write access for Owner and Group, No access for others.
    

```bash
[~]$ chmod 660 test-file  
```

* Full access for Owner, read and execute for group and no access for others.
    

```bash
[~]$ chmod 750 test-file
```

---

* *Checking Command History:* To check which commands you have run till now
    

```bash
[~]$ history
```

* *Removing a Directory/Folder:* To remove a directory/folder (for example, remove a directory named 'my\_folder')
    

```bash
[~]$ rm -r my_folder
```

* *Creating and Viewing fruits.txt:*
    

```bash
[~]$ echo "Apple Mango Banana Cherry Kiwi Orange Guava" > fruits.txt
[~]$ cat fruits.txt
```

* *Adding Content to devops.txt:* Add content in devops.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava:
    

```bash
[~]$ echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > devops.txt
```

* *Showing Top Three Fruits:*
    

```bash
[~]$ head -n 3 devops.txt
```

* *Showing Bottom Three Fruits*
    

```bash
[~]$ tail -n 3 devops.txt
```

* *Creating and Viewing Colors.txt*
    

```bash
[~]$ echo -e "Red\nPink\nWhite\nBlack\nBlue\nOrange\nPurple\nGrey" > Colors.txt

[~]$ cat Colors.txt
```

* *Adding Content to Colors.txt:* Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey:
    

```bash
[~]$ echo -e "Red\nPink\nWhite\nBlack\nBlue\nOrange\nPurple\nGrey" > Colors.txt
```

* *Finding Differences Between Files:* To find the difference between fruits.txt and Colors.txt file
    

```bash
[~]$ diff fruits.txt Colors.txt
```

> "Choose a job you love, and you will never have to work a day in your life." - <mark>Confucius</mark>

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">Happy learning!!!</div>
</div>

%[https://hashnode.com/post/clkso3bpx000009k275r554xg] 

%[https://hashnode.com/post/clktnsqy3001y09mo4o9abzdq]