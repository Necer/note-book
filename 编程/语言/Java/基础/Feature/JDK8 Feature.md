 [[JDK Feature]]
JDK8 新特性
#JDK8 #Java/feature


### Lambda语法 
#Lambda #形式语言与自动机

> Lambda Expressions, a new language feature, has been introduced in this release. They enable you to treat functionality as a method argument, or code as data. Lambda expressions let you express instances of single-method interfaces (referred to as functional interfaces) more compactly.

#### 基本语法

```java
parameter -> expression
```

```java
(parameter1, parameter2) -> expression
```

```java
(parameter1, parameter2) -> { code block }
```

```java
() -> expression
```

### 函数式接口

> @FunctionalInterface