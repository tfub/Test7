# Test7

## 实验内容：
### 1.读取手机联系人信息，并用ListView显示。显示界面布局如下所示。（给出读取联系人列表的实现）。


Contact.java
联系人实体类


phone_item.xml


activity_main.xml


ContactAdapter.java
自定义适配器


AndroidManifest.xml
权限声明


MainActivity.java


### 2.应用中有一个使用Sqllite保存的数据库db。里面有一个表contacts用于保存联系人的基本信息，这些信息包括姓名，联系电话，性别。要求你创建一个内容提供者，给其他app提供contacts中数据的查询。其他app能够查询contacts表中的所有信息，也可以查询单条联系人的信息。（实验报告给出你自定义的内容提供者的实现）

Contact.java
联系人实体类

DatabaseHelper.java
创建数据库db、创建表contacts，初始化contacts数据信息（共四条）

DatabaseHelper.java
自定义内容提供器，继承抽象类ContentProvider，实现方法。
GetType()方法根据传入的内容URI返回相应的MIME类型。
根据实验要求只对query()方法进行具体功能实现，查询所有信息和单条数据信息。

activity_task2.xml

AndroidManifest.xml
注册自定义内容提供器


Task2Activity.java
对按钮添加监听事件。




