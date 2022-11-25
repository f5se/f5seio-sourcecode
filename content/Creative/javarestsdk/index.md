---
title: "F5 iControlRest Java SDK"
date: 2022-11-24T8:41:13+08:00
draft: false
hideLastModified: true
summaryImage: "SDK-Logo.jpeg"
keepImageRatio: yes
tags: ["f5", "api", "tools", "Java SDK"]
summary: "A Java SDK for F5 iControlRest."
showInMenu: false
---

# F5 iControlRest Java SDK

F5 iControlRest Java SDK, which support use Java Programming to operate with LTM REST API. The SDK contains the F5 Object to Java Object mapping, like: `VirtualServer`, `Pool`, `Node`, `RulesReference`, etc, there are more than 30 Java Objects which can used directly.

With the F5 iControlRest Java SDK, you can speed up your Auto Ops system development, iControlSOAP to iControlREST Transformation, etc.

Current supported API including:


```
	@iType(category = LTM, type = POST)
	public Pool createPool(String name, String loadBalancingMode, String monitor, String[] members);
	
	@iType(category = LTM, type = POST)
	public Pool createPool(String name, String loadBalancingMode, String monitor, String[] members, long transId);
	
	@iType(category = LTM, type = POST)
	public Pool createPool(String payload);
	
	@iType(category = LTM, type = POST)
	public Pool createPool(String payload, long transId);
	
	@iType(category = LTM, type = DELETE)
	public Object deletePool(String name);
	
	@iType(category = LTM, type = DELETE)
	public Object deletePool(String name, long transId);
	
	@iType(category = LTM, type = GET)
	public SnatPoolReference listAllSnatPools();
	
	@iType(category = LTM, type = GET)
	public SnatPool getSnatPoolByName(String name);
	
	@iType(category = LTM, type = POST)
	public SnatPool createSnatPool(String name, String[] members);
	
	@iType(category = LTM, type = POST)
	public SnatPool createSnatPool(String name, String[] members, long transId);
	
	@iType(category = LTM, type = POST)
	public SnatPool createSnatPool(String payload);
	
	@iType(category = LTM, type = POST)
	public SnatPool createSnatPool(String payload, long transId);
	
	@iType(category = LTM, type = DELETE)
	public Object deleteSnatPool(String name);
	
	@iType(category = LTM, type = DELETE)
	public Object deleteSnatPool(String name, long transId);
	
	@iType(category = LTM, type = POST, description = "fastl4 vs, without persist")
	public VirtualServer createVirtualServer(String name, String destination, String pool);
	
	@iType(category = LTM, type = POST, description = "fastl4 vs, without persist")
	public VirtualServer createVirtualServer(String name, String destination, String pool, long transId);
	
	@iType(category = LTM, type = POST, description = "fastl4 vs, with persist")
	public VirtualServer createVirtualServer(String name, String destination, String pool, String persist);
	
	@iType(category = LTM, type = POST, description = "fastl4 vs, with persist")
	public VirtualServer createVirtualServer(String name, String destination, String pool, String persist, long transId);
	
	@iType(category = LTM, type = POST, description = "create vs via post body")
	public VirtualServer createVirtualServer(String payload);
	
	@iType(category = LTM, type = POST, description = "create vs via post body")
	public VirtualServer createVirtualServer(String payload, long transId);
	
	@iType(category = LTM, type = DELETE)
	public Object deleteVirtualServer(String name);
	
	@iType(category = LTM, type = DELETE)
	public Object deleteVirtualServer(String name, long transId);
	
	@iType(category = LTM, type = GET, description = "List All Virtual Servers")
	public VirtualServersReference listAllVirtualServers() ;
	
	@iType(category = LTM, type = GET)
	public VirtualServersReference listAllVirtualServersExpandSubcollections();
	
	@iType(category = LTM, type = GET)
	public VirtualServer getVirtualServerByName(String vsName);
	
	@iType(category = LTM, type = GET)
	public VirtualServer getVirtualServerByNameExpandSubcollections(String vsName);
	
	@iType(category = LTM, type = GET)
	public NodesReference listAllNodes();
	
	@iType(category = LTM, type = GET)
	public Node getNodeByName(String nodeName);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeDiable(String nodeName);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeEnable(String nodeName);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeOffline(String nodeName);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeUp(String nodeName);
	
	@iType(category = LTM, type = PATCH)
        public Object nodeDiable(String[] nodeNames);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeEnable(String[] nodeNames);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeOffline(String[] nodeNames);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeUp(String[] nodeNames);
	
	@iType(category = LTM, type = PATCH)
        public Object nodeDiable(String nodeName, long transId);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeEnable(String nodeName, long transId);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeOffline(String nodeName, long transId);
	
	@iType(category = LTM, type = PATCH)
	public Object nodeUp(String nodeName, long transId);
	
	@iType(category = LTM, type = GET)
	public PoolsReference listAllPools();
	
	@iType(category = LTM, type = GET)
	public PoolsReference listAllPoolsExpandSubcollections();
	
	@iType(category = LTM, type = GET)
	public Pool getPoolByName(String poolName);
	
	@iType(category = LTM, type = GET)
	public Pool getPoolByNameExpandSubcollections(String poolName);
	
	@iType(category = LTM, type = GET)
	public MembersReference listAllMembers(String poolName);
	
	@iType(category = LTM, type = GET)
	public Member getMemberByName(String poolName, String memberName);
	
	@iType(category = LTM, type = PATCH)
	public Object memberDisable(String poolName, String memberName);
	
	@iType(category = LTM, type = PATCH)
	public Object memberEnable(String poolName, String memberName);
	
	@iType(category = LTM, type = PATCH)
        public Object memberOffline(String poolName, String memberName);
	
	@iType(category = LTM, type = PATCH)
	public Object memberUp(String poolName, String memberName);
	
	@iType(category = LTM, type = PATCH)
        public Object memberDisable(String poolName, String[] memberNames);
	
	@iType(category = LTM, type = PATCH)
	public Object memberEnable(String poolName, String[] memberNames);
	
	@iType(category = LTM, type = PATCH)
       public Object memberOffline(String poolName, String[] memberNames);
	
	@iType(category = LTM, type = PATCH)
	public Object memberUp(String poolName, String[] memberNames);
	
	@iType(category = LTM, type = PATCH)
        public Object memberDisable(String poolName, String memberName, long transId);
	
	@iType(category = LTM, type = PATCH)
	public Object memberEnable(String poolName, String memberName, long transId);
	
	@iType(category = LTM, type = PATCH)
        public Object memberOffline(String poolName, String memberName, long transId);
	
	@iType(category = LTM, type = PATCH)
	public Object memberUp(String poolName, String memberName, long transId);
	
	@iType(category = LTM, type = POST)
	public Transaction transactionStart();
	
	@iType(category = LTM, type = GET)
	public Transaction transactionStatus(long transId);
	
	@iType(category = LTM, type = PATCH, description = "remove transaction from internal DB")
	public Object transactionRevoke(long transId);
	
	@iType(category = LTM, type = PATCH)
	public Object transactionCommit(long transId);
	
	@iType(category = LTM, type = GET)
	public TransactionReference listAllTransaction();
	
	@iType(category = LTM, type = POST)
	public BashResponse bashScripts(String bash);
```

More details refer to https://github.com/cloudadc/f5-rest-service/.
