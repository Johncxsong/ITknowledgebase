---
layout: default
title: Windows-Updating from Command Line
parent: Server_System
nav_order: 3
---

# Windows-Updating from Command Line
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Weekly Update CLI  

```Bash
Install-WindowsUpdate -ForceDownload -ForceInstall -Verbose -AcceptAll
```


## Resolving updates if it does not update

### 1. stop servers
```Bash
net stop bits 
net stop wuauserv
```

### 2. delete updates files 
`windows > softwareDistribution > delete everything`

### 3. restart server 
```Bash
net start bits 

net start wuauserv
```