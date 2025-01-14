---
layout: single
title: 评估·改造·守护 ｜ 整洁代码
header:
  overlay_filter: "rgba(99, 183, 175, 0.6)"
  overlay_image: /assets/images/background.jpg
sidebar:
  nav: "models"
permalink: /models/evaluate-models/clean-code/
toc: true
---

## 面向对象原则

### SOLID原则
> SOLID（单一功能、开闭原则、里氏替换、接口隔离以及依赖反转）
>            ---- 罗伯特·C·马丁在21世纪早期引入
{: .notice--info}

| S 	| 单一功能原则 	| 认为对象应该仅具有一种单一功能的概念。 	|
| O 	| 开闭原则 	| 认为“软件体应该是对于扩展开放的，但是对于修改封闭的”的概念。 	|
| L 	| 里氏替换原则 	| 认为“程序中的对象应该是可以在不改变程序正确性的前提下被它的子类所替换的”的概念。<br>参考契约式设计。 	|
| I 	| 接口隔离原则 	| 认为“多个特定客户端接口要好于一个宽泛用途的接口”的概念。 	|
| D 	| 依赖反转原则 	| 认为一个方法应该遵从“依赖于抽象而不是一个实例”的概念。<br>依赖注入是该原则的一种实现方式。 	|

### Head First 9原则
> From 《Head First》
{: .notice--info}

* **封装变化**： 找出应用中可能需要变化之处，把他们独立出来，不要和那些不需要变化的代码混在一起
* **针对接口编程，而不是针对实现编程**
* **多用组合，少用继承**
* **松耦合**：为了交互对象之间的松耦合设计而努力
* **开闭原则**：类应该对扩展开放，对修改关闭
* **依赖倒置**： 要依赖抽象，不要依赖具体类
* **最少知识原则**：只和你的密友谈话
* **好莱坞原则**： 别调用（打电话给）我们，我们会调用（打电话给）你
* **单一职责原则**： 一个类应该只有一个引起变化的原因

### 其他原则
* **不要重复你自己DRY**： “系统中的每一部分，都必须有一个单一的、明确的、权威的代表”，指的是（由人编写而非机器生成的）代码和测试所构成的系统，必须能够表达所应表达的内容，但是不能含有任何重复代码 [wiki](http://wiki.c2.com/?OnceAndOnlyOnce)


## 代码坏味道
### 代码重复
> 相同或者相似的代码存在于一个以上的地方。(违反了DRY原理)
{: .notice--info}

### 长方法
> 一个非常长的方法、函数或者过程。
{: .notice--info}

### 巨类
> 一个非常庞大的类。
{: .notice--info}

### 太多的参数
> 函数或者过程的冗长的参数列表使得代码可读性和质量非常差。
{: .notice--info}

### 特性依恋
> 一个类过度的使用另一个类的方法。
{: .notice--info}

### 亲密关系
> 一个类依赖另一个类的实现细节。
{: .notice--info}

### 拒绝继承
> 子类以一种‘拒绝’的态度，覆盖基类中的方法，换句话说，子类不想继承父类中的方法，参考里氏替换原则。
{: .notice--info}

### 冗余类 / 寄生虫
> 一个功能太少的类。
{: .notice--info}

### 人为的复杂
> 在简单设计已经满足需求的时候，强迫使用极度复杂的设计模式。
{: .notice--info}

### 超长标识符
> 尤其，在软件工程中，应该毫无保留的使用命名规则来消除歧义。
{: .notice--info}

### 超短标识符
> 除非很明显，一个变量名应该反映它的功用。
{: .notice--info}

### 过度使用字面值
> 为提高可读性和避免编码错误，应该使用命名常量。此外，字面值可以且应该在可能的情况下，独立存放于资源文件或者脚本中，在软件部署到不同区域时，可以很方便的本地化。
{: .notice--info}


## 面向对象模式

（其中前三行为常用模式）

| 策略模式 	| 观察者模式 	| 装饰者模式 	| 工厂方法模式 	| 抽象工厂模式 	|
| 单例模式 	| 命令模式 	| 适配器模式 	| 外观模式 	| 模版方法模式 	|
| 迭代器模式 	| 组合模式 	| 状态模式 	| 代理模式 	| 复合模式 	|
| 桥接模式 	| 生成器模式 	| 责任链模式 	| 蝇量模式（Flyweight） 	| 解释器模式 	|
| 中介者模式 	| 备忘录模式 	| 原型模式 	| 访问者模式 	|  	|


### 用模式思考
* 保持简单（Keep it simple / KISS)
* 设计模式非万灵丹；事实上，连什么丹都算不上
* 你知道何时需要模式
* 重构的实践就是模式的实践
* 拿掉你所不需要的，不要害怕将一个设计模式从你的设计中删除
* 如果你现在不需要，就别做






