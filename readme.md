**Clone of https://github.com/SignalR/java-client. Removed Android support, but added Maven functionality.**

# ASP.NET SignalR for Java
ASP.NET SignalR is a new library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications. What is "real-time web" functionality? It's the ability to have your server-side code push content to the connected clients as it happens, in real-time.

## What can it be used for?
Pushing data from the server to the client (not just browser clients) has always been a tough problem. SignalR makes 
it dead easy and handles all the heavy lifting for you.

This library can be used from both regular Java or Android applications.

## Documentation
See the [documentation](http://asp.net/signalr)
	
## LICENSE
[Apache 2.0 License](https://github.com/SignalR/SignalR/blob/master/LICENSE.md)

## Contributing

See the [contribution  guidelines](https://github.com/SignalR/SignalR/blob/master/CONTRIBUTING.md)

## Build with gradle
Use `./gradlew jar` to (re-)create the JAR file in `signalr-client-sdk/build/libs`. I did store the binaries here in GitHub -- cry your pardon -- as I did not want to recreate them every time via Maven.  
In your `.pom`, add this block to `repositories`:

```
<repository>
    <id>git-bcersows</id>
    <name>bcersows' SignalR GitHub based repo</name>
    <url>https://raw.githubusercontent.com/bcersows/java-client/master/</url>
</repository>
```

These belong into the `dependencies`:

```
<dependency>
    <groupId>com.google.code.gson</groupId>
    <artifactId>gson</artifactId>
    <version>2.8.1</version>
</dependency>
<dependency>
    <groupId>bcersows</groupId>
    <artifactId>signalr</artifactId>
    <version>1.0.0</version>
    <scope>provided</scope>
</dependency>
<dependency>
    <groupId>org.java-websocket</groupId>
    <artifactId>Java-WebSocket</artifactId>
    <version>1.3.4</version>
</dependency>
```

I do realize that the naming of the repository is not the best. Not gonna change it, though.
