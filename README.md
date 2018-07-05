# 数据库连接组件说明

	版本: V 1.0.7.0
    作者: daodaoliang
    时间: 2016年7月25日18:54:41

### 0. 组件结构说明

![项目架构](./scripts/pro_arch.png)

### 1. 组件使用说明

#### 1.1 编译组件库

* 获取源码;
* 在QtCreator中打开NDBPool.pro, 不要选择影子构建，开始编译构建;
* 同级目录中会出现bin文件夹,里面就是编译好的组件库, 注意看版本信息;
* 在外部项目使用时直接把编译好的库和inc文件夹下的文件打包使用即可;
* 在内部项目使用时,请直接引用NDBPool_inc.pri即可,同时需要手动把编译好的库拷贝到主程序执行目录,或者编写辅助脚本在运行前拷贝;

#### 1.2 运行测试用例

* 编译并运行 example 子项目即可，不要勾选在终端运行;

### 3. 组件路线图

* ~~数据库链接的动态分配和动态回收;~~
* ~~数据库链接在分配后的长时间未使用时动态回收;~~

### 4. changelog

* V 1.0.1.0 按照[公孙二狗](http://qtdebug.com/DB-ConnectionPool.html)的思路编写初版;
* V 1.0.2.0 增加数据库链接的动态分配;
* V 1.0.3.0 增加数据库连接的动态释放;
* V 1.0.4.0 优化处于等待状态下的连接池的状态维护;
* V 1.0.5.0 优化处于待释放状态下的连接池的状态维护,优化对外的使用接口
* V 1.0.6.0 优化对外的使用接口
* V 1.0.7.0 打补丁修改一些BUG



