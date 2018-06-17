# Java异常处理

在Java中,异常分为受检查的异常,与运行时异常. 两者都在异常类层次结构中.
下面的图展示了Java异常类的继承关系.

![](http://img.my.csdn.net/uploads/201310/29/1383051170_4167.jpeg)

粉红色的是受检查的异常(checked exceptions),其必须被 try{}catch语句块所捕获,或者在方法签名里通过throws子句声明.受检查的异常必须在编译时被捕捉处理,命名为 CHecked Exception 是因为Java编译器要进行检查,Java虚拟机也要进行检查,以确保这个规则得到遵守.
绿色的异常是运行时异常(runtime exceptions),需要程序员自己分析代码决定是否捕获和处理,比如 空指针,被0除...
而声明为Error的，则属于严重错误,需要根据业务信息进行特殊处理,Error不需要捕捉。