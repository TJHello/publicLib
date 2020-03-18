# PublicLib(公用库)
---
#### 将一些需要用到的aar或者jar包转换成mave的方式来进行远程集成 

### 使用方法

#### 1. 添加私有仓库

```groovy

buildscript {
     repositories {
        ...
         maven { url 'https://raw.githubusercontent.com/TJHello/publicLib/master'}
     }
}

allprojects {
     repositories {
        ...
        maven { url 'https://raw.githubusercontent.com/TJHello/publicLib/master'}
     }
}

```

#### 2. 添加对应的库

```groovy

dependencies {
	implementation 'com.TJHello.publicLib:Yomob:1.8.5' //Yomob广告集成需要的所有包
	implementation 'com.TJHello.publicLib:MI:2.5.0'//MI广告集成需要的所有包
	implementation 'com.TJHello.publicLib:GDTSDK:4.110.980'//GDT广告集成需要的所有包
	implementation 'com.TJHello:ADEasy:0002'//ADEasy
	//...
}

```
