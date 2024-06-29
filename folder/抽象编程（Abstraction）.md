# 抽象编程（Abstraction）
在计算机编程中，抽象编程是一种在复杂的软件系统中，降低复杂度，实现系统搞笑设计与方法的实现的方法。它将系统各功能实现的技术细节隐藏在相对简单的 API 接口中。

## 数据抽象的好处
* 使用户避免撰写低等级的代码。
* 避免代码重复，增加代码的复用性。
* 在不影响用户的前提下可以独立修改类的内部实现。
* 有助于提高应用程序的安全性，因为只用向用户提供重要的细节。

## 示例
```javascript
class ImplementAbstraction{
    // 设置一系列内部成员的值的方法
    set(x, y){
        this.a = x;
        this.b = y;
    }
    display(){
        console.log(`a = ${this.a}`);
        console.log(`b = ${this.b}`);
    }
}
const obj = new ImplementAbstraction();
obj.set(10, 20);
obj.display();
// a = 10
// b = 20
```