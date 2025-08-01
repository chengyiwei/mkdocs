

## 变量

程序中的信息是存储在变量中的，例如我们使用 `int a;` 这个语句，就可以定义一个名字为 `a` 的变量，前面的 `int` 表示这个变量里面是存储一个整数的

通俗的讲，我找来了一个盒子，这个盒子专门装整数，我给这个盒子取名叫 a 个整数。

我想把数字 `3` 放到 `a` 盒子里。

在程序里，方法是 `a = 3;`。

这里的等于号不是指左右两边相等，是指把右边的数字放到左边的变量里面，`=` 代表的含义是赋值。

`=` 左边必须是一个变量，右边必须是一个可以算出来数字的式子。

过了一会，我又想把数字 `5` 放到 `a` 盒子里。

那就改成 `a = 5;`

在之后的代码中，只要提到单独的 `a`，那么就代指 `a` 里面的数字。

例如，我们想要输出 `a` 里面的数字，那么只需要写下代码

```cpp
cout << a;
```

这会让程序输出一个 `5`

如果你定义了变量，而没有赋值，就等于拿了个盒子过来，而没有规定里面是什么 赋值这个符号也可以玩出花的，比如，我们现在有两个变量

```c
int a = 3, b = 5;
```

怎么才能交换两个变量里面的值呢?

交换两个盒子里的数字，可以先找来第三个盒子 `c`，先把 `a` 里面的东西放到 `c` 里面，再把 `b` 里面的东西放到 `a` 里面，再把 `c` 里面的东西放到 `b` 里面。

```c
int a = 3, b = 5, c = a;
a = b;
b = c;
```

但是如果是普通的盒子，你或许可以先把 `a` 里面的数字放到 `b`，再把 `b` 里面的数字放回 `a`。

而这个盒子有一个特性，同一时间里面只能存在一个数字，当你把 `a` 里的数字放进 `b`，两个数字就加起来，分不清原来是多少了。

如果是日常做题，你发现 `a = 3, b = 5`，那只要反过来赋值，让 `a = 5, b = 3` 就算交换了。

而在计算机中，你设计的题目不仅仅是为了解决这一种情况。

上面这种方法，不管 `a`，`b` 是多少，都能把它们的值进行交换。

把上面这个问题拓展成一个比较一般的情况，随便输入两个变量，交换这两个变量的值，最后把交换后的变量输出

这里大家可以暂停思考一下

我在这里给出答案：

```cpp
int a,b,c;
cin>>a>>b;//输入 a,b
c=a; a=b; b=c;
cout << a << " " << b << endl;
```

>代码中的 `//` 代表单行注释，电脑会自动忽略这一行中 `//` 后的内容，是方便自己和他人阅读代码用的

![image-20250728203724019](https://pic-1301573324.cos.ap-chengdu.myqcloud.com/image-20250728203724019.png)

运行的结果如下，我输入了 `114 514`，程序输出了 `514 114`

当然，变量还可以有其他操作，例如下面这段代码，大家可以想一想，是做什么用的

```cpp
int a,b,c;
cin>>a>>b;//输入 a,b
c=a+b;
cout << c << endl;
```

### 数据类型

因为存储一个数字，是需要空间的，比如你需要一个盒子来放整数，那你拿的盒子肯定不会是无限大的，所以这个盒子能放的数字也是有范围限制的。

比如说，你想要一个盒子，能装得下 100 以内的自然数，那我给你一个能装 -200~200 的盒子就差不多了，再大就浪费了。

但是如果你想装 10000 以内的自然数，我就要给你换大盒子了。

`int` 类型的变量：存的数字的大小范围是 $-2^{32} \sim 2^{32} - 1$。

`long long` 类型的变量：存的数字的大小范围是 $-2^{64} \sim 2^{64} - 1$。

**还有一些特殊的类型**

`bool` 类型变量：只能存 `0` 或者 `1`，`0` 代表结果为假，`1` 代表结果为真。

这个 `bool` 类型适用于只需要判断两种情况的时候，比如你投一个硬币，只想知道哪面朝上，可以定义一个 `bool flag;`，在 `flag` 里面存投硬币的结果。

`char` 类型变量：用来存字符类型的变量，数值范围是 $-128 \sim 127$。

为什么字符类型还有数值呢？

计算机中，比如你想存一个字符 `x`，但是计算机只有 `0/1` 格子，它只能存数字，所以计算机是靠每个字符和一个数字来对应（对应规则常用的是 ASCII 码），在字符变量中存储数字实现的。

比如，`x` 和 `120` 对应，那么你写 `char ch=x;` 的时候，变量 `ch` 里面真正存的其实是数字 `120`，而 `char` 解释了这是一个字符类型的变量，所以当你对 `char` 输入 `x` 的时候，它自动把 `x` 对应成 `120` 放进 `ch`，当你要输出 `ch` 的时候，它又自动把 `120` 解释为 `x` 进行输出。

如果你在代码中，只写一个 `x`，那么一般代表的是有个变量的名字是 `x`。

如果你想指的是字符 `x`，那么请加单引号 `'x'`。

```c
char x,y;
y='b';
x=y;  // 这时候 x 里面是 'b'。
x='y' // 这时候 x 里面是 'y'。
```

`string` 类型变量: 字符串类型，里面存的是由许多个 `char` 拼接成的字符串，每个字符也遵守对应规则。

如果不想表示变量，而想表示字符串，请加双引号。

```c
string ab,cd;
cd="qaq";
ab=cd;    //此时 ab 里面是 "qaq"。
ab="ac";  //此时 ab 里面是 "cd"。
```

`double` 类型变量: 用来存储小数，没有范围限制，但是当你存的数字过大会过小时，会产生一定的误差。

如果想要输出一个小数，可以用下面的句子来控制输出小数点后多少位数:

```cpp
double a=1.234; cout<<fixed<<setprecision(2)<<a<<endl;
```

这样最后就只会输出 `1.23` 。这个控制遵循四舍五入原则。

## 参考资料

华中师范大学集训队内部文档

