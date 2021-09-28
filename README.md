# jdk


## 현재버전 확인
```
❯ java -version
openjdk version "11.0.10" 2021-01-19
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.10+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.10+9, mixed mode)
```

## 설치되어있는 JDK리스트 확인
```
❯ /usr/libexec/java_home -V
Matching Java Virtual Machines (2):
    11.0.10, x86_64:    "AdoptOpenJDK 11"    /Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home
    1.8.0_252, x86_64:    "AdoptOpenJDK 8"    /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home

/Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home

```

## JDK 버전 변경
```
// 1.8 버전으로 변경
❯ export JAVA_HOME=$(/usr/libexec/java_home -v 1.8)

// 11 버전으로 변경
❯ export JAVA_HOME=$(/usr/libexec/java_home -v 11)

```
## 변경 여부 확인
```
❯ java -version
openjdk version "1.8.0_252"
OpenJDK Runtime Environment (AdoptOpenJDK)(build 1.8.0_252-b09)
OpenJDK 64-Bit Server VM (AdoptOpenJDK)(build 25.252-b09, mixed mode)

❯ echo $JAVA_HOME
/Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home

```
