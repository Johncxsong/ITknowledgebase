---
layout: default
title: New PC - adding domain network
parent: Server_System
nav_order: 2
---

# New PC - adding domain network
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Add New Computer in Domain Network  
1. Connect staff wifi 
2. Open Powershell 
3. `Rename-Computer -NewName [name]` to restart  
4. `Add-computer -DomainName [domain name]` to connect

{: .warning}
DNS in the new computer must point to Server IP [it sould be automatically set up]