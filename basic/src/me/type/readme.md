# 数据类型练习
## int
## double
## boolean

# 基本数据类型总结

- 4 类 8 种基本数据类型。4 整数型，2 浮点型，1 布尔型，1 字符型

| 类型       | 存储 | 取值范围                                                     | 默认值          | 包装类    |
| ---------- | ---- | ------------------------------------------------------------ | --------------- | --------- |
| **整数型** |      |                                                              |                 |           |
| byte       | 8    | 最大存储数据量是 255，最小 -2<sup>7</sup>，最大 2<sup>7</sup>-1，<br />[-128~127] | (byte) 0        | Byte      |
| short      | 16   | 最大数据存储量是 65536，[-2<sup>15</sup>,2<sup>15</sup>-1]，<br />[-32768,32767]，±3万 | (short) 0       | Short     |
| int        | 32   | 最大数据存储容量是 2<sup>31</sup>-1，<br />[-2<sup>31</sup>,2<sup>31</sup>-1]，±21亿，[ -2147483648, 2147483647] | 0               | Integer   |
| long       | 64   | 最大数据存储容量是 2<sup>64</sup>-1，<br />[-2<sup>63</sup>,2<sup>63</sup>-1]， ±922亿亿（±（922+16个零）） | 0L              | Long      |
| **浮点型** |      |                                                              |                 |           |
| float      | 32   | 数据范围在 3.4e-45~1.4e38，直接赋值时必须在数字后加上 f 或 F | 0.0f            | Float     |
| double     | 64   | 数据范围在 4.9e-324~1.8e308，赋值时可以加 d 或 D 也可以不加  | 0.0d            | Double    |
| **布尔型** |      |                                                              |                 |           |
| boolean    | 1    | true / flase                                                 | false           | Boolean   |
| **字符型** |      |                                                              |                 |           |
| char       | 16   | 存储 Unicode 码，用单引号赋值                                | '\u0000' (null) | Character |

- 引用数据类型
  - 类（class）、接口（interface）、数组
- 自动装箱和拆箱
  - 基本数据类型和它对应的封装类型之间可以相互转换。自动拆装箱是 `jdk5.0` 提供的新特特性，它可以自动实现类型的转换
  - **装箱**：从**基本数据类型**到**封装类型**叫做装箱
  - **拆箱**：从**封装类型**到**基本数据类型**叫拆箱

```java
// jdk 1.5
public class TestDemo {
    public static void main(String[] args) {
        Integer m =10;
        int i = m;
    }
}
```

　　上面的代码在 jdk1.4 以后的版本都不会报错，它实现了自动拆装箱的功能，如果是 jdk1.4，就得这样写了

```java
// jdk 1.4
public class TestDemo {
    public static void main(String[] args) {
        Integer b = new Integer(210);
        int c = b.intValue();
    }
}
```

# 数据类型转换
## String转int
## String转Double
# String
## String的常用函数
## StringBuffer
# Date
## SimpleDateFormat
