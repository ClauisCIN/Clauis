# Clauis
### 指针的 `const` 修饰

`const` 可以修饰数据类型，也可以修饰指针变量。

#### 常量指针（修饰数据类型）

`const` 修饰数据类型时，指针指向的地址可以改变，但指针指向的地址所对应的内容不可以改变。

```cpp
int a = 0, b = 0;
const int *p = &a;
*p = 1; // 错误
p = &b; // 正确
```

#### 指针常量（修饰指针变量）

`const` 修饰指针变量时，指针指向的地址不可以改变，但指针指向的地址所对应的内容可以改变。

```cpp
int a = 0, b = 0;
int *const p = &a;
*p = 1; // 正确
p = &b; // 错误
```
