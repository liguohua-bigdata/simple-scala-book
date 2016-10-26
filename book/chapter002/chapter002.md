####1.Scala的类型系统
在一个语言当中，类型系统的重要性不言而喻。它可以表示:  
1. 语音支持的数据  
2. 语言支持的操作  
在Scala中一切都是对象，下图说明了scala的类型系统  
![](images/classhierarchy.img_assist_custom.png)   
---
>
说明：  
1.在scale中root class是scala.Any，代表着一切类型.它是Scala所有类的父类，所有类都是他直接或间接的子类。在这个类中定义的方法成为，
  所有类的共同的方法，在任何类型的对象中都能够调用。这个类中定义了以下几个方法。
 >>
 final def ==(that: Any): Boolean
 final def !=(that: Any): Boolean
 def equals(that: Any): Boolean
 def hashCode: Int
 def toString: String
 
2.scala.Any有两个子类scala.AnyVal，scala.AnyRef分别代表一切数值类型和一切引用类型.   
>>2.1 scala.AnyVal有Byte、Short、Char、Int、Long、Float、Double、Boolean和Unit9个具体类型,前8个都对应到Java的基本类型.  
>>2.2 scala.AnyRef实际上是Java的java.lang.Object类别名。所以我们自定义类型都是该类的子类。  

>3.scala.Nothing是所有类的子类  




