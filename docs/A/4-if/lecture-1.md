>"即使算法有千万种可能，我也只选择通向你的那条分支"
>——《Code Romance》

##  基础if-else结构

```cpp
#include <iostream>
using namespace std;

int main() {
    int score = 85; // 考试成绩
    if (score >= 60) {              // 条件判断
        cout << "恭喜及格！" << endl;  // 条件成立执行
    } 
    else {                         // 否则
        cout << "需要继续努力！" << endl; // 条件不成立执行
    }
    return 0;
}
```

##  条件运算符

| 运算符 | 含义     | 生活实例           |
| ------ | -------- | ------------------ |
| `>`    | 大于     | 存款 `>` 房价      |
| `<`    | 小于     | 体重 `<` 标准      |
| `==`   | 等于     | 验证码输入正确     |
| `!=`   | 不等于   | 选择与默认选项不同 |
| `>=`   | 大于等于 | 年龄 `>=` 18岁     |
| `&&`   | 逻辑与   | 有钱 `&&` 有闲     |
| `\|\|` | 逻辑或   | 周末 `\|\|` 节假日 |



##  多条件判断阶梯

```cpp
#include <iostream>
using namespace std;

int main() {
    int temperature; // 当前温度
    cin >> temperature; // 输入温度值
    if (temperature > 30) {
        cout << "开启空调制冷" << endl;
    } 
    else if (temperature > 25) {
        cout << "开电扇就够了" << endl;
    } 
    else if (temperature > 18) {
        cout << "舒适温度" << endl;
    } 
    else {
        cout << "可能需要加件衣服" << endl;
    }
}
```

##  if-else嵌套

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string username = "admin";
    string password = "123456";
    string inputUser, inputPass;
    
    cout << "用户名: ";
    cin >> inputUser;
    cout << "密码: ";
    cin >> inputPass;
    
    if (inputUser == username) {
        if (inputPass == password) {
            cout << "登录成功！欢迎回来，" << username << "!" << endl;
        } else {
            cout << "密码错误！" << endl;
        }
    } else {
        cout << "用户名不存在！" << endl;
    }
    
    return 0;
}
```

##  三目运算符

1. **基本语法**

```cpp
条件 ? 表达式1 : 表达式2;
```

2. **实用例子**

```cpp
// 普通if-else
if (score >= 60) {
    result = "及格";
} else {
    result = "不及格";
}
// 三目运算符版本
result = (score >= 60) ? "及格" : "不及格";
```

看吧代码一下就简洁了不少，但同时可读性也下降了

3. **多级三目运算**

```cpp
string grade = (score >= 90) ? "优秀" :
               (score >= 80) ? "良好" :
               (score >= 70) ? "中等" :
               (score >= 60) ? "及格" : "不及格";
```

##  重要注意事项

1. **常见错误警示**  

   ```cpp
   if (a = 5)   // 错误！这是赋值操作
   if (a == 5)  // 正确比较写法
   ```

2. **简洁写法**

   ```cpp
   if (isRaining) 
       takeUmbrella();// 单语句可省略花括号
   ```

    但是要注意`else`总是匹配最近的`if`,加上`{}`可以保证`if-else`对的顺序正确

3. **判断范围技巧**  

   ```cpp
   if (10 <= x && x <= 20) // 判断x在10到20之间
   ```


> "人生没有else，但代码教会我们：每个选择都值得被认真对待" ——《硅谷物语》

请完成**实验4-1**