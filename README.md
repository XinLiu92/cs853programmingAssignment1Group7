# cs853programmingAssignment1Group7

UNH cs853 Information Retrieval (Fall 2018) programming assignment1
Gourp 7: Xin Liu, Kunpeng Xie, Yibo Xu


cs853 Prog assignment1 installation

Group 7: Xin Liu, Kunpeng Xie, Yibo Xu



Required Tool:

1. Maven3.5.4: To automatic loading up required dependencies, download from:https://maven.apache.org/download.cgi
2. Git: Version control, download from https://git-scm.com/downloads
3. Intellij IDEA: download from https://www.jetbrains.com/idea/download/#section=mac



Installation:

1. Maven installation guide https://maven.apache.org/install.html
2. Git installation:https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
3. Intellij installation: https://www.jetbrains.com/help/idea/install-and-set-up-product.html



Add trec car tool to the project:

1. Navigate to the directory of trec car tool java version which is ~/trec-car-tools-java-master
2. Use maven command to package the trec car tool to jar file and maven will put it in maven local repository
       mvn clean install
   *If you got a message like mvn: command not found. Under Linux, you need to set JAVA_HOME and M2_HOME directory in .bash_profile, if there is no such file, just create one. run the following command 
   
       sudo vi ~/.bash_profile
   Add the following to the file:
       //replace the JAVA_HOME and M2_HOME based on your own
       JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_121.jdk/Contents/Home
       export JAVA_HOME
        
       M2_HOME=/Users/kangkang/Documents/maven/apache-maven-3.3.9
       export M2_HOME
        
       PATH=${PATH}:${JAVA_HOME}/bin:${M2_HOME}/bin
       export PATH
   save and exit the file and run the following command:
       source ~/.bash_profile
   Now you can go the ~/trec-car-tools-java-master to run the command.

1. Clone the programming assignment by https://github.com/XinLiu92/cs853programmingAssignment1Group7.git to your local. 
2. Open the cloned repository in Intellij, and reimport maven dependencies.
   Windows type in ctrl+shift+a to find action, type in "reimport", you will find "reimport all maven projects", then select it and press enter. Mac will type in cmd+shift +a instead. 
   All of the necessary dependencies are included in pom.xml
3. Make sure you pass two arguments to the program, the first one is index directory, second one is the data file directory
4. Rebuild the project and run Main.java
5. By changing the boolean variable defualtScore under Main.java to false, you can swich the score function to the one we need to change in assignment spec.
6. Then run the program to get the result.
