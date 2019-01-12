# test-01
>本文作者丁安娜，未经作者许可，不可转载！

**提示**:*本人只是一个还未入门的小白，写下此文章，只是为了记录学习历程*

Java下载地址：[Java官网](https://www.java.com/zh_CN/)

下面来记录今天所学知识点：

- 数组
   - 数组的语法
   - 数组的操纵
- 类
   - 类的概念
   - 类的创建
-------
- 数组
1. 语法:

两种创建方式:

(1). dataType[] arry = new dataType[arraySize];

(2).dataType[] arry = {value0, value1, ..., valuek};
   
2. 数组的操纵(一般用循环语句来处理数组元素):

代码示例:

```Java
public class TestArray {
   public static void main(String[] args) {
      double[] myList = {1.9, 2.9, 3.4, 3.5};
 
      // 打印所有数组元素
      for (int i = 0; i < myList.length; i++) {
         System.out.println(myList[i] + " ");
      }
      // 计算所有元素的总和
      double total = 0;
      for (int i = 0; i < myList.length; i++) {
         total += myList[i];
      }
      System.out.println("Total is " + total);
      // 查找最大元素
      double max = myList[0];
      for (int i = 1; i < myList.length; i++) {
         if (myList[i] > max) max = myList[i];
      }
      System.out.println("Max is " + max);
   }
}
```
- 类
1. 概念:

(1). 类是一个模板，它描述一类对象的行为和状态。

(2). 对象(与类作对比区别):对象是类的一个实例，有状态和行为。

2. 类的创建:

示例:

```Java
package student;

public class book {
	public String title;
	public String author;
	public String press;
	public String ISBN;
	public double price;

}
```
```Java
package student;

public class student {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		book b = new book();
		b.title = "xxx";
		b.author = "xxx";
		b.press = "xxx";
		b.ISBN = "xxx";
		b.price = 12.34;
	}

}
```
