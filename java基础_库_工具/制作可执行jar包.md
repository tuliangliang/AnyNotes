### 制作可执行jar包

* 使用maven快捷方式quickstart方式创建项目，并借助maven打包命令mvn package打成jar包
* pom.xml添加maven-shade-plugin插件可以把所需依赖一并打进jar包


### 遇到的坑
- [直接运行jar包找不到主类和没有主清单属性的解决](https://blog.csdn.net/qq_27483535/article/details/52830421)
- [使用maven的maven-shade-plugi插件时需要注意的一个问题](https://blog.csdn.net/thc1987/article/details/44176481)
- 超级大坑：使用idea快捷键创建java项目时会在<build></build>中包含一层<pluginManagement>，请删除，否则打包无法添加主类。