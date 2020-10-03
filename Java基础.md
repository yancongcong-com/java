# JAVA基础

## 入门

快捷输入：psvm + tab  sout 

- ### 注释

  1. 单行注释：

     ```java
     //我是注释
     ```

  2. 多行注释：

     ```java
     /*
     我是多行注释
     */
     ```

  3. 文档注释

     ```shell
     修改注释样式
     Editor下 Commenst
     ```

- ## 标识符

   	1. 关键字
      	2. 标识符注意点
       - 所有的标识符必须以字母(A-Za-z)$或_开始
       - 首字母之后任何字符
       - 不能使用关键字
       - 标识符大小写敏感

## 数据类型 

  - 强类型语言

    - 要求变量的使用要求严格符合规定，所有变量定义后才能使用

  - 弱类型语言

    - 变量类型随着变量的值改变而改变

  - Java的数据类型分为两大类

    - 基本类型（primitive  type）

       1. 整型

          - byte占一个字节范围-128~127

          - short占两个字节范围-32768~32767

          - int占四个字节范围-2^31~2^31-1

          - long占8个字节范围

            ```java
            long num = 20L;
            ```

       2. 浮点型

          - float占四个字节

            ```java
            float mun = 29.1F;
            ```

          - double占八个字节

            > ```java
            > //不能用浮点数进行比较
            > float f = 0.1f;
            > double d = 1.0/10;
            > System.out.println(f==d);
            > ```

       3. 字符类型

          - char占两个字节

            ```java
            int()
            /*
            GBK：国标码 汉字两个字节 简体中文
            BIG5:繁体中文
            utf-8统一编码，汉字三个字节
            */
            //转义字符
            // \t
            // \n
            ```

        	4. boolean类型

          - 占一位true和false

            ```java
            boolean flag = true;
            if(flag){}
            ```

      > 什么是字节  8bit=1B(byte)   8位=1字节

    - 引用类型（reference type）

      1. 类

         ```java
         String  name = "yancongcong"
         ```

      2. 接口

      3. 组

## 类型转换

  1. 优先级

  2. **转换类型**

     - 强制转换类型		(类型)变量名
     - 自动转换类型        自动

  3. | 低   |       |      |      |       | 高     |
     | ---- | ----- | ---- | ---- | ----- | ------ |
     | byte | short | int  | long | float | double |

     > 运算中，不同类型的数据先转换为同一类型，然后进行运算

  ```java
  /*
  1. 不能对布尔值进行转化
  2. 不能把对象类型转换成不相干的类型
  3. 在把高容量转换成低容量的类型，强制转换
  4. 转换可能出现内存溢出，影响精度
  */
  ```

## 变量

  > 变量名----变量类型----作用域

  ```java
  type varName [=value] [{,varName[=value]}];
  ```

  - 作用域

    - 局部变量

      > 位于方法中，只可在本方法中使用

    - 实例变量

      > 位于类中，需要实例化才可使用(默认int为0，Boolean为false,其他为null)

    - 类变量

      > 位于类中，添加static。全局调用

## 常量

- 定义

  ```java
  final double name = 'yancongcong';
  ```

## 变量的命名规范

1. 所有变量，方法，类名：见名知意
2. 类成员变量：首字母小写和驼峰原则
3. 局部变量：首字母小写和驼峰原则
4. 常量：大写字母和下划线
5. 类名：首字母大写和驼峰原则
6. 方法名：首字母小写和驼峰原则

## 运算符

- 算术运算符：+，-，*，/，%，++，--（幂运算 Math.pow(x,y)）

- 赋值运算符：=

- 关系运算符：>,<,>=,<=,==,!=instanceof

- 逻辑运算符：&&(与)，||(或)，!(非)

  - 逻辑与运算：两个变量都为真，结果才为true

  - 逻辑或运算：两个变量有一个真，结果为true

  - 逻辑非运算：真为假，假为真

  - 短路：当与运算有一个为假，后续不在执行

    ```java
    int mun = 2;
    boolean d = (mun>4)&&(mun++>2);
    System.out.println(d);
    System.out.println(mun);
    ```

- 位运算符：&,|,^,~,>>,<<,>>>

  - \>>右移

- 条件运算符：？：

  - 三元运算符

  ```java
          int score = 20;
          String type = score > 60 ?"及格":"不及格";
          System.out.println(type);
  ```

  - > +号连接

    ```java
    //注意
    System.out.println("" + a + b);
    System.out.println(a + b + "");
    ```

- 扩展赋值运算符：+=，-=，*=，/=

## 包机制

- 一般利用公司域名作为包名倒置

  ## Javadoc

- 参数信息
  - @author作者名
  - @version版本号
  - @since 指明需要最早的JDK版本
  - @param参数名
  - @return返回值情况
  - @throws异常抛出情况
- Javadoc

```dockerfile

```



  

  

  

  



































