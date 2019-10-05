##### 按步骤进行:

- 按照需求更改generator.xml配置文件：
  - 更改connectionURL, userId, password配置数据库连接
  - 自定义包名和位置，涉及到javaModelGenerator 和 sqlMapGenerator 和 javaClientGenerator
  - 利用<table>标签定义将要映射的数据库表
- 根据targetProject指定的主目录名和targetPackage指定的包名创建文件夹（这里src已经创建好了，里面有三个test.xx创建文件夹的例子）
- 在文件夹根目录运行命令：```java -jar mybatis-generator-core-1.3.0.jar -configfile generator.xml -overwrite```
