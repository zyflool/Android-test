# 2019 Android组机试题

## 思考题

### 编程示例

```java
public calss main{
    public static void main(String[] args){
        String name="John";
        int number = 130;
		System.out.println(test(name)+":"+ number);
    }
    
    String test(String name){
        return name;
    }
}
```

输出结果：

```
John:130

```

可能会用到的：

for循环

```
public calss main{
    public static void main(String[] args){
        int n=0;
		for(int i =0;i<5;i++){
			n=n+i;
		}
		System.out.println(n);
    }
}

```

输出结果：

```
10
```

### 一、找出数组/切片(array/slice)中第二小的数

例如 1,2,3,4,5,6 2第二小

```java
public calss main{
    public static void main(String[] args){
        
		System.out.println(second());
    }
    static int second(int[] array){
      //your code
    }
}
```



### 二、斐波那契数列

在[数学](https://zh.wikipedia.org/wiki/數學)上，**斐波那契数列**是以[递归](https://zh.wikipedia.org/wiki/递归)的方法来定义：
> $$
\> F_0 = 0
\> $$
\>
\> $$
\> F_1 = 1
\> $$
\>
\> $$
\> F_n = F_{n-1} + F_{n-2} (n>=2)
\> $$
\>
\> 用文字来说，就是斐波那契数列由0和1开始，之后的斐波那契系数就是由之前的两数相加而得出。首几个斐波那契系数是：
\>
\> 0，1，1，2，3，5，8，13，21，34，55，89，144，233……
\>
\> **特别指出**：[0](https://zh.wikipedia.org/wiki/0)不是第一项，而是第零项。

请写出程序，输入n，返回第n项是？

```java
public calss main{
    public static void main(String[] args){
        
		System.out.println(fibonacc());
    }
    static int Fibonacc(int n){
      //your code
    }
}
```



### 三、编写一个程序，判断字符串b是否在字符串a内、

```java
public calss main{
    public static void main(String[] args){
        String a="String";
        String b="ing";
		System.out.println(find(a,b));
    }
    static String find(String a, String b){
      //your code
    }
}
```



 

### 四、回文数判断
判断一个整数是否是回文数。回文数是指正序（从左向右）和倒序（从右向左）读都是一样的整数。 例如121，123321，12521....

```java
boolean isPalindrome(int n){
    
    //your code
    
    
    
    
    // return true or false
}
```





### 五、全排列
给定 {1, 2, 3, , , n}，其全排列为 n! 个，这是最基础的高中组合数学知识，现给出一个数组，请你输出他的全排列例如，{1,2,3} 
123 132 231 213 321 312



```java
void fullpermutation(int[] array){
    //your code 
    
    // use "System.out.println()" 输出所有结果
}
```

## 面向对象编程思想题

### 6. 读程序题

- 读下列代码回答问题，下列`kotlin`代码中用到了 `kotlin`的基本输出和`继承、接口`的相关知识 

```kotlin

object Muxi {
    @JvmStatic
    fun main(args: Array<String>) {
        val student = Student()
        student.say()
        student.study()
    }


}

internal class Student : Person(), Study {

    override fun say() {
        super.say()
        println("I'm a student!")
    }


    override fun study() {
        println("I'm studying!")
    }
}

internal open class Person {
    var string = "I'm a person!"

    internal open fun say() {
        println(string)
    }
}

internal interface Study {
    fun study()
}

```

1. 请写出该程序的输出。
2. 分析并指出这个程序中父类和接口的作用
3. 结合这个程序，说说继承和接口的区别

