# Java-
避免遗漏忘记，在此记录 
位运算符 &
首先首先互相比较的数换成二进制然后上下排放比较每一个相对着的数字如果都为1，则第三行相对的数就是1，否则为0
比较完后再将二进制换成10二进制，如果有必要的话。



使用idea创建src的java文件时自带一个Main.java文件，该文件输出一句"Hello World"，这是为什么呢？原来Hello World 中文意思是『你好,世界』。因为《The C Programme Language》中使用它做为第一个演示程序，非常著名，所以后来的程序员在学习编程或进行设备调试时延续了这一习惯。

        java文件的本质是什么？

        java文件本质其实就是文本文件，我们可以用任何文本编辑器对它进行编译（不信的话可以试试选择打开方式，只要是使用文本编辑器它的内容都不会改变），只要最后它的扩展名为.java就可以使用java虚拟机jvm对其进行编译和运行。

        main方法是程序的入口，可是main方法为什么要写成：public static void main(String [] args){}？

        首先 main是java程序的入口，java程序通过java虚拟机JVM调用，属于外部调用，所以需要使用public修饰，否则虚拟机无法调用。

        在java中，没有static的变量或函数，如果想被调用的话，是要先新建一个对象才可以。而main函数作为程序的入口，需要在其它函数实例化之前就启动，这也就是为什么要加一个static。main函数好比一个门，要探索其它函数要先从门进入程序。static提供了这样一个特性，无需建立对象，就可以启动。

        使用void的原因是当main方法出现返回值时JVM无法进行上抛，如果有返回值难道抛给操作系统么?

        String[]args中args是数组的名字，并不是固定的，不信可以自己试试，它是声明了一个可从控制台接受的数据的类型为String数组，所以main方法中其实除了这个arg意外其他都必须是固定格式
