# Operators and Functions
## 1. Built-in Operators(内建运算符)
### 1.1 Operators Precedences(运算符优先顺序)
#### 1.1.1 元素选择(element selector, dot)
```
语法:
    bracket_op([]);
    dot(.)
举例：
    A[B];
    A.identifier
```
#### 1.1.2 一元前缀运算符(unary prefix operators)
```
语法:
    unary(+);
    unary(-);
    unary(~)
举例：
    -A
```
#### 1.1.3 一元后缀(unary suffix)
```
语法:
    IS [NOT] (NULL|TRUE|FALSE)
举例：
    A IS NULL
```
#### 1.1.4 位异或(bitwise xor)
```
语法:
    bitwise xor(^)
举例：
    A ^ B
```
#### 1.1.5 乘法类运算符(multiplicative operators)
```
语法:
    star(*);
    divide(/);
    mod(%);
    div(DIV)
举例：
    A * B
```
#### 1.1.6 加法类运算符(additive operators)
```
语法:
    plus(+)；
    minus(-)
举例：
    A + B
```
#### 1.1.7 字符串连接(string concatenate)
```
语法:
    string concatenate(||)
举例：
    A || B
```
#### 1.1.8 位与(bitwise and)
```
语法:
    bitwise and(&)
举例：
    A & B
```
#### 1.1.9 位或(bitwise or)
```
语法:
    bitwise or(|)
举例：
    A | B
```
### 1.2 Relational Operators(关系运算符)
### 1.3 Arithmetic Operators(算数运算符)
### 1.4 Logical Operators(逻辑运算符)
### 1.5 String Operators(字符串运算符)
### 1.6 Complex Type Constructors(复杂类型构造符)
### 1.7 Operators on Complex Types(复杂类型操作符)
## 2. Built-in Functions(内建函数)
### 2.1 Mathematical Functions(数学函数)

### 2.2 Collection Functions(集合函数)
### 2.3 Type Conversion Functions(类型转换函数)
### 2.4 Date Functions(日期函数)
#### 2.4.1 UNIX时间戳转日期函数：from_unixtime
```
语法：
    from_unixtime(bigint unixtime[, string format])
返回值：
    string
说明：
    转化UNIX时间戳(从 1970-01-01 00:00:00 UTC 到指定时间的秒数)到当前时区的时间格式
举例：
    select from_unixtime(1688718148,'yyyyMMdd')
    结果：20211105
补充：
    1. 如果format为空，则默认为yyyy-MM-dd HH:mm:ss
    2. format参数的格式参考：https://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html
```
### 2.5 Conditional Functions(条件函数)
### 2.6 String Functions(字符串函数)
### 2.7 Data Masking Functions(数据屏蔽函数)
### 2.8 Misc. Functions(杂项函数)
#### 2.8.1 xpath
#### 2.8.2 get_json_object
## 3. Built-in Aggregate Functions(UDAF)(聚合函数)
## 4. Built-in Table-Generating Functions(UDTF)(表生成函数)
### 4.1 Usage Examples
#### 4.1.1 explode (array)
#### 4.1.2 explode (map)
#### 4.1.3 posexplode (array)
#### 4.1.4 inline (array of structs)
#### 4.1.5 stack (values)
### 4.2 explode
### 4.3 posexplode
### 4.4 json_tuple
### 4.5 parse_url_tuple