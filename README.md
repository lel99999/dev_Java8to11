# dev_Java8to11
Java 8 to 11 Review, Workspace and Notes

![Java 8 vs Java 11](https://github.com/lel99999/dev_Java8to11/blob/main/java-8-vs-java-11.png) <br/>

#### Install Java 8, 11. RHEL 7
```
$sudo yum install -y java-1.8.0-openjdk-devel 

$sudo yum install -y java-11-openjdk-devel
```

#### Switching Java Versions with Alternatives
```
$sudo alternatives --config java

There are 2 programs which provide 'java'.
Selection      Command
-----------------------------------------------
*+ 1           java-1.8.0-openjdk.x86_64 (/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.191.b12-8.el8.x86_64/jre/bin/java)
   2           java-11-openjdk.x86_64 (/usr/lib/jvm/java-11-openjdk-11.0.1.13-4.el8.x86_64/bin/java)

Enter to keep the current selection[+], or type selection number: 2
```
This will switch the system java binary to JDK 11. We do the same for javac since java and javac are independently managed. There is no need to switch anything else as every other JDK binary will switch either with the java or the javac binary:
```
$ sudo alternatives --config javac
There are 2 programs which provide 'javac'.
Selection      Command
-----------------------------------------------
*+ 1           java-1.8.0-openjdk.x86_64 (/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.191.b12-8.el8.x86_64/jre/bin/javac)
   2           java-11-openjdk.x86_64 (/usr/lib/jvm/java-11-openjdk-11.0.1.13-4.el8.x86_64/bin/javac)

Enter to keep the current selection[+], or type selection number: 2
```

#### Notes
