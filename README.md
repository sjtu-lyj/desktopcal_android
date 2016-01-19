# desktopcal_android

## 说明
1. 本app是的desktopcal 的android端 （官网地址 http://chs.desktopcal.com/）
2. 日历使用了 https://github.com/prolificinteractive/material-calendarview
3. 看板位置： https://www.leangoo.com/board/go/1024876#

## 使用方法
1. 请先安装使用desktopcal和坚果云（pc端和android端）
2. 将 C:\Users\(do your self)\AppData\Roaming\DesktopCal\Db 设为坚果云的同步文件夹。文件夹中应该有一个calendar.db文件(如果安装目录不一样，可以用everything或者listary来搜索calendar.db)
3. 安装本app。可以再android上用search everything来搜索一下calendar.db 的位置。app中使用的是静态地址。在我的小米4中为/storage/emulated/0/Android/data/nutstore.android/cache/objectcache/1/calendar.db。app中用的也是这个地址

## 原理
1. desktopcal的所有数据都是储存在calendar.db这个sqlite数据库中，可以用navicat工具直接打开它
2. 由于官方没有api，所以只能自己手工同步

## 问题处理
| 可能遇到的问题      | 解决方案      | 
| -------------       |:-------------:|
| windows不能及时同步到android端          | desktopcal在打开=的时候坚果云不能同步，只要把desktopcal关闭手工同步一下即可 | 
| 坚果云同步的位置和app中不一样，导致打不开 | 可以自行修改代码，编译，或者把问题反馈给我。我也会尽快实现自行查找db位置 |   

## question and answer
| question |  answer| 
| -------------       |:-------------:|
| 为什么没有登录界面| 我没有用户的密码，所以数据更新是用户自己的电脑实现的 | 

