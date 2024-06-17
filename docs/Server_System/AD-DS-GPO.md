---
layout: default
title: AD_DS-GPO
parent: Server_System
nav_order: 4
---

# Active Direcotiry Domain Server__Group Policy
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What is Group Policy? 
**Group Policy Objects** are features of Active Directory (domain network) to control the working environment of user accounts and computer accounts. It provide centralized management and configuration of operating systems, applications...

{: .note}
Event ID 1058 - Group Policy error

## Find the Group Policy

This Command line will show all GPOs 
```
Get-GPO -All | Select Id, Displayname
```

If need, update 
```
gpupdate /force
```
## Reset Defualt Group Policy  

If there is something wrong with default Group Policy Objects, reset default.  

```bash
dcgpofix /target:domain 

dcgpofix /target:dc

```

## Current GPOs  

We have two GPOs: (back up in C://gpo)
1. Printer 
2. Deny Student logon


