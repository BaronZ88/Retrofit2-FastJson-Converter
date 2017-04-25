# Retrofit2-FastJson-Converter

> 为 Retrofit2 提供的 FastJson 解析器（FastJsonConverter），弥补了官方缺少对 FastJson 支持的问题。

## 何如使用

### 一、添加依赖  

**Gradle 方式依赖:**

Step 1. Add the JitPack repository to your build file

```groovy
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```
	
Step 2. Add the dependency

```groovy
dependencies {
	compile 'com.github.BaronZ88:Retrofit2-FastJson-Converter:1.2'
}
```
	

**Maven 方式依赖:**

Step 1. Add the JitPack repository to your build file

```xml
<repositories>
	<repository>
	    <id>jitpack.io</id>
	    <url>https://jitpack.io</url>
	</repository>
</repositories>
```
    
Step 2. Add the dependency

```xml
<dependency>
	<groupId>com.github.BaronZ88</groupId>
	<artifactId>Retrofit2-FastJson-Converter</artifactId>
	<version>1.2</version>
</dependency>
```

### 二、使用

在 Retrofit.Builder 的 addConverterFactory 方法中传入 `FastJsonConverterFactory.create()` 即可。如下：

```java
Retrofit retrofit = new Retrofit.Builder()
      .baseUrl(baseUrl)
      .addConverterFactory(FastJsonConverterFactory.create())
      .client(client)
      .build();
```




