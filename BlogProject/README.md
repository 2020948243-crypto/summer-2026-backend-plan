# SpringBoot博客后端项目

## 技术栈
- Java 21
- SpringBoot 3.2.x
- MyBatis-Plus
- MySQL 8.0+
- Redis 7.0+
- SpringSecurity
- JWT
- Knife4j

## 项目结构
```
src/
├── main/
│   ├── java/
│   │   └── com/example/blog/
│   │       ├── controller/
│   │       ├── service/
│   │       ├── mapper/
│   │       ├── entity/
│   │       ├── dto/
│   │       ├── config/
│   │       ├── security/
│   │       └── BlogApplication.java
│   └── resources/
│       ├── application.yml
│       └── schema.sql
└── pom.xml
```

## 功能列表
- [ ] 用户注册/登录
- [ ] JWT鉴权
- [ ] 文章CRUD
- [ ] 文章分页
- [ ] 分类管理
- [ ] 标签管理
- [ ] 评论功能
- [ ] 点赞功能
- [ ] 权限控制

## 部署说明
```bash
# 构建项目
mvn clean package

# 运行项目
java -jar target/blog-0.0.1-SNAPSHOT.jar
```

## 接口文档
访问 http://localhost:8080/doc.html 查看接口文档