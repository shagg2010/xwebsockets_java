-------------------
How To Run - Client
-------------------
1) Open Chrome
2) Open debugger tools, then Console tab
3) Copy WebSocketClient.js code to console window
4) Now, create new variable in Console using - var client = new WebSocketClient('ws', '127.0.0.1', 8081, '/xwebsockets_java/endpoint');
5) Now, on Console write and hit enter - client.connect();
6) Now, on Console write and hit enter - client.send('Hello Server!');
7) You should get response from WebSocket Sever
8) Now, on Console write and hit enter - client.disconnect();

--------------------------------------------------
How To Run - Server
--------------------------------------------------
1)  Add Tomcat 9 Server Configuration in IntelliJ
    1.1) Open Settings -> Plugins tab
    1.2) Search Tomcat, now install Smart Tomcat plugin
    1.3) Open Settings -> Tomcat Server -> Create new Config
        1.3.1) Download tomcat 9, and provide the location of sever (example: c:\apache\tomcat9\)
    1.4) Now go to Run -> Edit Configurations -> Smart Tomcat
        1.4.1) Click on '+' to create new config, and provide Server Port (use 8081 for this example) and use default admin port 8005
    1.5) Click on Play button for this Run Config in main IntelliJ Window to start the server