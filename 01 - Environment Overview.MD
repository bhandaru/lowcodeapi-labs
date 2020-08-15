# Environment Overview.   
  
<div align="center">## OCP Architecture</div>

![](/images/common-environment-ocp-architecture.png)  

You will be interacting with an OpenShift environment that is running on a public cloud. The environment consists of the following systems:  
```   
    1 master node(s)  
    1 infrastructure node(s)  
    20 "application" nodes  
    An NFS server  
```
The infrastructure node is providing several services:  
```
    The OpenShift Docker registry  
    The OpenShift router  
    Etherpad  
```

Additionally, a predefined number of user accounts have been provisioned.

Before continuing, please visit visit the Etherpad at the following URL:

```
http://etherpad-ocp-workshop.apps.osevg.openshiftworkshop.com/p/workshop
```

Decide on a user account among one of the available users or use the one that has been assigned to you by the instructor. Find that user account and type your name next to it. This will be your user account for the duration of these exercises. For example:

```
userXY=Luke Skywalker
```

If you already see a name next to a user account, it means that someone else has already claimed it.

You will see various code and command blocks throughout these exercises. Some of the command blocks can be copy/pasted directly. Others will require modification of the command before execution. If you see a command block with a red border (see below), the command will require modification. Typically this is a substitution of your username or user number:
```
some command for userXY
```

<p align="center">
  <a href="/README.md">Previous Exercise</a> &nbsp;|
  &nbsp;<a href="/README.md">Table of Contents</a> &nbsp;|
  &nbsp;<a href="/02%20-%20Installing%20Client.MD">Next Exercise</a>
</p>
