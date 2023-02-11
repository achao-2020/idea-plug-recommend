# 整理好用的idea插件

## 一、整理的思路

  基于springboot开发的后端项目中，从数据库设计之后，实体类到控制层的接口生成，再到实际开发的便捷插件，单元测试，整理出来以下几款能够增加开发效率的插件。

## 二、mybatis代码生成器

    `mybatisX`能够根据数据库表快速生成service， entity，mapper。

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-22-48-49-image.png)

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-22-49-08-image.png)

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-22-49-39-image.png)

## 三、快速接口调用

    使用`Restfull Fast Request`插件，定义好controller的接口之后，只需要在代码行左侧，既可以快速进行接口测试，可以不必使用其他接口文档生成的第三方调用工具，方便快捷。同时可以配置多种调用环境。

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-22-55-05-image.png)

## 四、热部署插件

    `Jrebel and XRebel` 可以便开发边进行编译，不用二次启动便可以及时测试更改的功能（快速生效，使用idea rebuild功能，快捷键ctrl + shift +F9）。务必使用截图版本，才能”免费（pojie）使用”。

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-22-58-13-image.png)

## 五、生成全部属性getter,setter

    在控制层，数据传输层，服务层，实体层中进场要进行pojo的转换，这个时候，需要对某个类的全部属性进行赋值（有些字段没有对应上就无法使用copy util），这个时候为了不遗漏字段，需要对每个字段进行setter，有这样一款插件，可以生成全部的setter方法——`GenerateAllSetter`，在需要的实体上使用Alt + Enter快捷键，弹出生成菜单。见下面截图：

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-23-04-47-image.png)

## 六、驼峰转换

    开发过程中对SET_ORG常量的定义，和数据库(set_org)，变量(setOrg)的命名方法有所不同，这个使用`CamelCase`插件，可以快速转换。选中变量，使用快捷键Shift + Alt + U，可以在不同格式中进行转换。

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-23-08-34-image.png)

## 七、翻译插件

    `A8Translate`可以对选中的单词翻译，快捷键Alt + 8;`Translate `可以对java doc注释进行整句翻译。

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-23-17-00-image.png)

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-23-15-35-image.png)

## 八、代码规约

    老生常谈的插件，可以提高开发者代码的规范。避免出现不好的习惯导致功能上的漏洞。

`Alibaba Java Coding Guidelines`

`SonarLint`

## 九、单元测试插件

    每次写完功能，需要编写单元测试用例，保证功能系统的稳定性。`SquareTest`可以快捷生成多个测试用例（基于Mokito），开发者只需要关注测试用例的参数构建。需要注意的是，基于controller的测试用例，并没有完好的模板，作者自己编写了个模板（并不完整）；参考如下：

![](C:\Users\Xpeng\AppData\Roaming\marktext\images\2023-02-11-23-23-17-image.png)

controller单元测试生成模板

[controller测试模板](整理好用的idea插件.md)
