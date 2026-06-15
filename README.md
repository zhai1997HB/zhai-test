# Demo Spring Boot Project

## 项目简介
这是一个基于 Spring Boot 3.2.0 的示例项目，使用 Java 17 开发。

## 技术栈
- Spring Boot 3.2.0
- Java 17
- Maven
- Spring Web
- Spring Actuator
- Lombok

## 项目结构
```
demo/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── demo/
│   │   │               ├── DemoApplication.java
│   │   │               └── controller/
│   │   │                   └── HelloController.java
│   │   └── resources/
│   │       └── application.yml
│   └── test/
│       └── java/
│           └── com/
│               └── example/
│                   └── demo/
│                       └── DemoApplicationTests.java
├── pom.xml
└── README.md
```

## 快速开始

### 前置条件
- JDK 17 或更高版本
- Maven 3.6+

### 运行项目
```bash
# 编译项目
mvn clean install

# 运行项目
mvn spring-boot:run
```

### 访问端点
项目启动后，可以访问以下端点：

- 健康检查: http://localhost:8080/actuator/health
- Hello API: http://localhost:8080/api/hello
- 服务状态: http://localhost:8080/api/health

## 开发指南

### 添加新功能
1. 在 `src/main/java/com/example/demo` 下创建新的包和类
2. 添加相应的测试类到 `src/test/java/com/example/demo`
3. 运行测试确保功能正常

### 运行测试
```bash
mvn test
```

### 打包
```bash
mvn clean package
```

## 许可证
MIT License
