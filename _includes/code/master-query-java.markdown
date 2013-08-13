

```java
Random randomizer = new Random();
MasterServer master = new MasterServer(MasterServer.GOLDSRC_MASTER_SERVER);   
Vector<InetSocketAddress> servers = master.getServers();
InetSocketAddress randomServer = servers.elementAt(
  randomizer.nextInt(servers.size())
);
GoldSrcServer server = new GoldSrcServer(randomServer.getAddress(),
  randomServer.getPort()
);
```