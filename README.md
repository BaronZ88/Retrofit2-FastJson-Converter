# Retrofit2-FastJson-Converter

> 为 Retrofit2 提供的 FastJson 解析器（FastJsonConverter），弥补了官方缺少对 FastJson 支持的问题。

## 添加依赖

### Gradle 依赖方式:

Step 1. Add the JitPack repository to your build file

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
	
Step 2. Add the dependency

	dependencies {
	        compile 'com.github.BaronZ88:Retrofit2-FastJson-Converter:1.2'
	}
	

### Maven 依赖方式:

Step 1. Add the JitPack repository to your build file

	<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
    
Step 2. Add the dependency

	<dependency>
	    <groupId>com.github.BaronZ88</groupId>
	    <artifactId>Retrofit2-FastJson-Converter</artifactId>
	    <version>1.2</version>
	</dependency>

