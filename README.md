# YHAutoCoding![](http://pfile.cn/px0r3c)
利用运行时原理一句话实现对象所有成员变量的归档解档!!
###使用方式
#### 一、使用 pod 安装
```
	在 Podfile 文件中添加:

		pod 'YHAutoCoding'
	
	执行 pod install 命令

```
#### 二、手动集成
1、往 Xcode 中拖入文件夹 YHAutoCoding

2、在需要归档解档的类中引入头文件

```
#import "YHAutoCoding.h"
```
3、在类中实现如下方法即可

```
/** 一句话实现对象自动归档解档 */
yh_autoCoding

/** 添加忽略归档的变量 */
- (NSArray *)ignoredMemberNames {
    return @[@"_zs_balance"];
}
```
			
![icon](http://pfile.cn/vdowo2-l)
