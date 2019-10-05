##### 按步骤进行:
1. 按照需求更改generator.xml配置文件
	需要配置的东西有：
	1.1 connectionURL 和 userId 和 password配置连接数据库信息
	1.2 自定义各种包名和位置，涉及到javaModelGenerator 和 sqlMapGenerator 和 javaClientGenerator
	1.3 利用<table>标签定义自己想映射的数据库表
2. 根据targetProject所指定的主目录名和targetPackage所指定的包名创建文件夹（这里src已经创建好了，里面有三个test.xx创建文件夹的例子）
3. 在这一堆东西所在文件夹运行命令：java -jar mybatis-generator-core-1.3.0.jar -configfile generator.xml -overwrite
