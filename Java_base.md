
## 变量
1. 浮点数不能表示精确的值，如货币。
2. 成员变量（实例变量）不初始化默认为0。
3. 成员变量可以声明在使用前或者使用后。
4. 多个线程同时修改一个类的静态变量，可能破坏数据的一致性，需要采取适当的同步措施，如同步机制、原子类或 volatile 关键字。
5. `name instanceof String`：name是否位String类型。
## 命名
1. 静态变量一般采用驼峰命名法。
1. 常量一般采用全大写字母命名法，用final修饰，作用同#define。
1. 类名一般采用驼峰命名法，以大写字母开头。
## 修饰符
1. 默认访问修饰符（default修饰符或不使用修饰符），只能被同一个包的其他类访问。
1. protect修饰符：①同一个包内可以访问，②不同包的子类可以访问继承来的protect方法。
1. 父类中声明为 public 的方法在子类中也必须为 public。
1. 父类中声明为 protected 的方法在子类中要么声明为 protected，要么声明为 public，不能声明为 private。
1. 父类中声明为 private 的方法，不能够被子类继承。
1. static关键字声明的静态方法不能使用类的非静态变量。
1. 父类中的 final 方法可以被子类继承，但是不能被子类重写。
1. final 类不能被继承，没有类能够继承 final 类的任何特性。
1. abstract修饰符定义的类为抽象类，抽象类不能用来实例化对象，声明抽象类的唯一目的是为了将来对该类进行扩充。。
1. 一个类不能同时被 abstract 和 final 修饰。
1. 如果一个类包含抽象方法，那么该类一定要声明为抽象类，否则将出现编译错误。
1. 抽象类可以包含抽象方法和非抽象方法。
1. 抽象方法是一种没有任何实现的方法，该方法的具体实现由子类提供。
1. 抽象方法不能被声明成 final 和 static。
1. 任何继承抽象类的子类必须实现父类的所有抽象方法，除非该子类也是抽象类。
1. 抽象方法的声明以分号结尾，例如：`public abstract sample();`。
1. synchronized 关键字声明的方法同一时间只能被一个线程访问。
## JavaEE
1. switch语句中，如果 case 语句块中没有 break 语句时，匹配成功后，从当前 case 开始，不论能否匹配，后续所有 case 的语句都会执行。
1. 用`String str = "Runoob";`创建的字符串存储在公共池中。
1. 用`String str2=new String("Runoob");`创建的字符串对象存储在堆上。
1. String 类是不可改变的，如果需要对字符串做很多修改，那么应该选择使用 StringBuffer & StringBuilder 类。
1. `System.out.println();`的用法同python的`print`函数。
1. `System.out.printf();`的用法同C语言的`printf`函数。
1. `System.out.format();`的用法同C语言的`sprintf`函数。
1. StringBuilder 类和 StringBuffer 之间的最大不同在于 StringBuilder 的方法不是线程安全的（不能同步访问）。
1. 由于 StringBuilder 相较于 StringBuffer 有速度优势，所以多数情况下建议使用 StringBuilder 类。
1. `public static void main(String[] args)`的`arga`是在命令行输入的字符串数组，以不可见字符隔开。
1. `protected void finalize() throws java.lang.Throwable {}`函数相当于析构函数，在对象被销毁时调用。
## JavaIO
1. `BufferedReader`对象可以用以输入字符。
    ```java
    char c;
    // 使用 System.in 创建 BufferedReader
    BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
    System.out.println("输入字符, 按下 'q' 键退出。");
    // 读取字符
    do {
        c = (char) br.read();
    } while (c != 'q');
    ```
    ```java
    String str;
    BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
    do {
        str = br.readLine();
        System.out.println(str);
    } while (!str.equals("end"));
    ```
1. `Scanner`duxi
$f(x,y)$