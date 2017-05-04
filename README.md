## Retrofit2-FastJson-Converter

> 为 Retrofit2 提供的 FastJson 解析器（FastJsonConverter），弥补了官方缺少对 FastJson 支持的问题。

[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg)](https://www.apache.org/licenses/LICENSE-2.0)

### 何如使用

#### 一、添加依赖  

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

#### 二、使用

在 Retrofit.Builder 的 addConverterFactory 方法中传入 `FastJsonConverterFactory.create()` 即可。如下：

```java
Retrofit retrofit = new Retrofit.Builder()
      .baseUrl(baseUrl)
      .addConverterFactory(FastJsonConverterFactory.create())
      .client(client)
      .build();
```
### 开源许可

```
Copyright 2017 Baron Zhang

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```



