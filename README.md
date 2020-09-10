```A fork from subTee, who seems to have removed the original short-lived public repo. Not my work. If you're reading this subTee and want me to take it down, I will. Didn't mean to host some private code of yours.```

# GhostLoader
GhostLoader - AppDomainManager - Injection - 攻壳机动队



GhostLoader Steps :)


```
1. Create C:\Tools
2. Copy Some .NET, any .NET binary to C:\Tools
3. In this example, we use FileHistory.exe, but any .NET app will do.
4. Ensure FileHistory.exe.config is in the same path
5. Execute C:\Tools\FileHistory.exe

Does your tool/product detect/observe the Image Load Event?

The purpose of this example is to demonstrate a way to circumvent, tools that catch/prevent ImageLoad events.

```

This should evade [Sysmon Event ID 7](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon#events)

```
Event ID 7: Image loaded
The image loaded event logs when a module is loaded in a specific process. This event is disabled by default and needs to be 
configured with the –l option. It indicates the process in which the module is loaded, hashes and signature information. The
signature is created asynchronously for performance reasons and indicates if the file was removed after loading. This event
should be configured carefully, as monitoring all image load events will generate a large number of events.
```
