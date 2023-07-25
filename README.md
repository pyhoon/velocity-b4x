# velocity-b4x
A wrap of Apache Velocity Engine library for B4A and B4J (b4xlib)

# What is Velocity?​
Velocity is a Java-based template engine. It permits anyone to use a simple yet powerful template language to reference objects defined in Java code.

Source: https://velocity.apache.org/

## Download additional libraries:
[velocity-engine-core-2.3.jar](https://dlcdn.apache.org//velocity/engine/2.3/velocity-engine-core-2.3.jar)\
[commons-lang3-3.12.0.jar](https://repo1.maven.org/maven2/org/apache/commons/commons-lang3/3.12.0/commons-lang3-3.12.0.jar)\
[slf4j-api-2.0.7.jar](https://repo1.maven.org/maven2/org/slf4j/slf4j-api/2.0.7/slf4j-api-2.0.7.jar) (required if not using jServer)\
[slf4j-simple-2.0.7.jar](https://repo1.maven.org/maven2/org/slf4j/slf4j-simple/2.0.7/slf4j-simple-2.0.7.jar) (required if not using jServer)

## Change Logs:

v1.01 - Changed to b4xlib. Modified Initialize method.\
v1.02 - Added evaluate method. Added example project.\
v1.03 - Renamed Text method to ToString. Removed redundant references for slf4j libraries in manifest.txt which already existed in jServer.

## Velocity
Author: aeric\
Credit to: Daestrum\
Version: 1.03

### Methods:

***Initialize** (Directory As String)*\
Initializes the object. You can pass a default directory inside Objects directory

***put** (Key As Object, Value As Object)*\
Put Context with Key Value pair

***putMap** (m As Map)*\
Put Context by passing a Map

***merge***\
Merge Template with Context and pass to StringWriter

***mergeTemplate** (TemplateFile As String, Encoding As String)*\
Merge a Template with Context and pass to StringWriter

***evaluate** (Tag As String, TemplateString As String)*\
Evaluate TemplateString

### Properties:

***get** (Key As String) As Object [read only]*\
Get the Context by Key

***Template** As String [write only]*\
Load a Template file

***ToString** As Object [read only]*\
Return StringWriter as String
