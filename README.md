# AudioRecorder
A Small JAR utility


A Small JAR File which will help you to create the Audio File. Just use the JAVALOADER tag by Mark to Call the Jar file and call the method to save the Recording. By Default it will be saved as: [filename].wav

The usage of this Tag is quite Easy. Just Call the javaLoader by this and call the method as:
[code]
&lt;cfscript&gt;
filePaths = ArrayNew(1);
filePaths[1] = expandPath(&quot;JavaRecorder.jar&quot;); // Path where your JavaLoader.jar you have placed
loaderObj =createObject(&quot;component&quot;,&quot;javaloader.JavaLoader&quot;).init(filePaths);
staticClassObj = loaderObj.create(&quot;com.recorder.AudioRecorder&quot;); 
   result = staticClassObj.record('C:\wwwroot\recording'); 
&lt;/cfscript&gt;
[/code]

[recording] is the name of the file. It will be stored in the wwwroot folder. if things are not clear, Email me i will guide you 

Just Provide Path in the record method and then bang it will save the file, currently the time is 3 minutes. This is still in Beta Version. I need your suggestions Guys to add more functionality, Please write here to let me know to add more functionality.

Drop me an Email on: webmaster@steadysoft.in 

Last Update:
Added Some example code to show the user how to record the file and where it will be recorded

Requirements:
Coldfusion version which supports javaloader
