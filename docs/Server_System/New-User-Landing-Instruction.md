---
layout: default
title: New User Entry Landing
parent: Server_System
nav_order: 1
---

# New User Entry Landing Instruction for IT admin
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Identity at Internet

### Add New Student
Login Server > Active Directory Users and Computers > REALMS folder > Students > Create a new user > Enter the Info  
Properties (right click user) > Member of...Tab(1.student onsite/ 2. student distant)
- General tab (descriptions: studentID number in the back card) 
- Account tab (unlock account)  

### Add Auditor Student
Login Server > Active Directory Users and Computers > Contacts folder > Create a new user > Properties  
- Member of tab (1. auditor onsite/ 2. auditor distant)  

### Sync with Azure 
```bash
Start-ADSyncSyncCycle -PolicyType Delta
```

### Micosoft 365 Admin Center 
Users(left tool bar) > Active users > Search the user > License and apps  
Multi-factor authentication (top bar) > search user > enable  

{: .note}
Microsoft 365 Business Standard--> onsite student (need purchase)  
Business Basic--> prospective student (free)  
Business Premium & Phone--> Staff  


## Identity at Physical Building

[Click Here to Login](https://my2n.com/){: .btn-green }  

Main building > Devices (left toolbar) > Back door >  Click three dots > Open configuration > Login > Directory > Create new user > Put name and ID (access enable for entry and exit rules).  


### Add Description in Student File
{: .no_toc }
Login Server > Active Directory Users and Computers > REALMS folder > Students > Properties > General tab > Description (student ID in the back last 6 digit NO.)  

### Internet Connection
{: .no_toc }
Staff/ Students / Guest  

## Others
### Printing Sync
Login `172.16.30.16:9191` > Options > User/Group sync > sync options  

### SharePoint back up  
SharePoint > Department > IT > Documentation > Door Lock System > ID cards  






