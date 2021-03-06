# SDK和API的区别





作者：简道云
链接：https://www.zhihu.com/question/21691705/answer/770586138
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。



**讲个小故事：**

> 研发人员A开发了软件A，研发人员B正在研发软件B。  
> 有一天，研发人员B想要调用软件A的部分功能来用，但是他又不想从头看一遍软件A的源码和功能实现过程，怎么办呢？  
> 研发人员A想了一个好主意：**我把软件A里你需要的功能打包好，写成一个函数。你按照我说的流程，把这个函数放在软件B里，就能直接用我的功能了！**
> 其中，API就是研发人员A说的那个函数。

![img](https://pica.zhimg.com/50/v2-4160a3b3d7361a1d75fa0174f8e3e83e_720w.jpg?source=1940ef5c)![img](https://pica.zhimg.com/80/v2-4160a3b3d7361a1d75fa0174f8e3e83e_1440w.jpg?source=1940ef5c)

这就是API的诞生。

**日常生活中，我们有很多类似API的场景，比如：**

> 电脑需要调用手机里面的信息，这时候你会拿一根数据线将电脑手机连接起来，电脑和手机上连接数据线的接口就相当于“API接口”。如图所示：

![img](https://pica.zhimg.com/50/v2-c3e0af3bc3c7ec6a163a2e8b5b5d6695_720w.jpg?source=1940ef5c)![img](https://pica.zhimg.com/80/v2-c3e0af3bc3c7ec6a163a2e8b5b5d6695_1440w.jpg?source=1940ef5c)

**那SDK又是什么？**

SDK 就是 Software Development Kit 的缩写，翻译过来——软件开发工具包。这是一个覆盖面相当广泛的名词，可以这么说：辅助开发某一类软件的相关文档、范例和工具的集合都可以叫做SDK。

SDK被开发出来是为了减少程序员工作量的。

比如——

有公司开发出某种软件的某一功能，把它封装成SDK（比如数据分析SDK就是能够实现数据分析功能的SDK），出售给其他公司做开发用，其他公司如果想要给软件开发出某种功能，但又不想从头开始搞开发，直接付钱省事。



**现在可以谈谈API和SDK的区别了。**

总的来说，两者没有值得比较的区别，因为是具有关联性的两种东西。

你可以把SDK想象成一个虚拟的程序包，在这个程序包中有一份做好的软件功能，这份程序包几乎是全封闭的，只有一个小小接口可以联通外界，这个接口就是API。

比如——

我们现在要在企业ERP系统中增加某个功能（比如自动备份、数据分析、云存储等），但又不想耗费大量时间、也没那么多研发亲自去做这个功能。这时我们可以选择使用这个“SDK”软件包，把ERP系统连接上API接口，就可以使用SDK软件包里的功能。



- **举个实例辅助理解：**

【中铁大桥科研院】有一个自研的信息平台，用于管理业务数据。

但他们曾面临一个问题——尽管有信息平台，却因为系统的独立性，数据的上传和备份，需要依靠人工在excel里来回操作，效率很低。

由于系统的开发周期长、成本高，桥科院将目光聚焦到现成的功能软件上。

后来通过API将简道云直接插入公司数据库，数据可自动上传至信息平台上并统一展示；再通过webhook把数据推送到服务器，实现自动备份。

![img](https://pic2.zhimg.com/50/v2-e412823d1380e1174b97ab614f818159_720w.jpg?source=1940ef5c)![img](https://pic2.zhimg.com/80/v2-e412823d1380e1174b97ab614f818159_1440w.jpg?source=1940ef5c)API将信息平台与简道云相连

在这一过程中，简道云扮演的角色就是SDK，而简道云配备API接口，可以对接外部系统，让桥科院不用开发直接实现了数据自动上传、备份的功能。



**最后，贴近生活讲讲两者的关系：**

有一杯密封饮料，它的名字叫做“SDK”。

饮料上插着吸管，吸管的名字叫“API”。

把你叫做“XX系统”。

如果你想喝到SDK里的饮料（让系统拥有SDK中的功能），你必须通过API这根吸管来实现（通过API连接你的系统和SDK工具包），否则你就喝不到饮料。

**所以：**

SDK＝放着你想要的软件功能的软件包

API＝SDK上唯一的接口