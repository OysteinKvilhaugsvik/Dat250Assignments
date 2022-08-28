## Heroku Report

**Installation Problems and Validation**

I had no problems with the installations, but Mavan was the only tool i was missing. 
We have used Eclipse in several other courses so it works fine. I plan on using VScode which i have used before and should work fine.

**Technical Problems**

During the setup of the Heroku app i ran into problems with the ```mvn clean install``` command. The error massage said that "Java_Home is undefined".
I should probably have set the path of the JDK as an environment variable while i installed maven. However, setting Java_Home did not seem to solve the problem. 
After some googling i found that in the file mvn.bat in the maven folder you can set Java_Home like this which solved the problem.
```
@REM ==== START VALIDATION ====
set JAVA_HOME=C:\Users\oyste\jdk-18_windows-x64_bin\jdk-18.0.2.1\bin
if not "%JAVA_HOME%"=="" goto OkJHome
```

This seemed to solve the problem and everything else worked.
Link to [Heroku App] (https://lit-lake-78049.herokuapp.com/)
