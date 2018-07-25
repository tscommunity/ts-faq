# TypeScript 常见问题 TypeScript FAQ

​	关于 TypeScript 的常见问题。Frequently asked questions about TypeScript.

------

目录 Contents

- TypeScript 是什么？What is TypeScript?
- TypeScript 为何而出现？
- TypeScript 能做什么？What can TypeScript do?
- TypeScript 的优势有哪些？What are the advantages of TypeScript?
- TypeScript 的生态如何？What is the ecology of TypeScript?
- 使用 TypeScript 开发的大型的、成功的项目有哪些？What are the large and successful projects developed by TypeScript?
- 学习、使用 TypeScript 有什么前提要求？What are the prerequisites for learning and using TypeScript?
- 如何正确地、高效地学习 TypeScript？How to learn TypeScript properly and efficiently?
- TypeScript 的开发工具有哪些？What are the TypeScript development tools?
- [FAQ 主题 FAQ Topics](#faq-主题-faq-topics)
  - [类型及类型系统 主题 Type and Type System Topics](#类型及类型系统-主题-type-and-type-system-topics)
  - [函数 主题 Function Topics](#函数-主题-function-topics)
  - [类 主题 Class Topics](#类-主题-class-topics)
    - [TypeScript 中有抽象类吗？](#typescript-中有抽象类吗)
    - [TypeScript 中支持内部类吗？](#typescript-中支持内部类吗)
    - [TypeScript 中支持分部类（partial class）吗？](#typescript-中支持分部类partial-class吗)
  - [接口 主题 Interface Topics](#接口-主题-interface-topics)
  - [枚举 主题 Enum Topics](#枚举-主题-enum-topics)
  - [继承与扩展 主题 Inheritance and Extension Topics](#继承与扩展-主题-inheritance-and-extension-topics)
  - [泛型 主题 Generic Topics](#泛型-主题-generic-topics)
  - [修饰符 主题 Modifier Topics](#修饰符-主题-modifier-topics)
  - [类型保护 主题 Type Guards Topics](#类型保护-主题-type-guards-topics)
  - [类型声明 主题 Type Declaration Topics](#类型声明-主题-type-declaration-topics)
  - [模块化 主题 Module Topics](#模块化-主题-module-topics)
  - [工程化 主题 Project Organization Topics](#工程化-主题-project-organization-topics)
  - [编译选项 主题 Compilation Topics](#编译选项-主题-compilation-topics)
  - [装饰器 主题 Decorator Topics](#装饰器-主题-decorator-topics)

------

## TypeScript 是什么？What is TypeScript?

​	TypeScript 是由 Microsoft 出品的开源、MIT 授权、用于开发大型 JavaScript 应用程序的新一代编程语言。它是 JavaScript 的一个类型化超集（typed superset），被编译为纯净的 JavaScript，由微软的 C# 之父安德斯 · 海尔斯伯格（Anders Hejlsberg ）主导开发并持续迭代发展。

​	TypeScript 的官方网站是 [https://www.typescriptlang.org](https://www.typescriptlang.org)，开源项目地址是 [https://github.com/Microsoft/TypeScript](https://github.com/Microsoft/TypeScript)。

## TypeScript 为何而出现？

## TypeScript 能做什么？What does TypeScript can do?

## TypeScript 的优势有哪些？What are the advantages of TypeScript?

## 使用 TypeScript 开发的大型的、成功的项目有哪些？What are the large and successful projects developed by TypeScript?

## 学习、使用 TypeScript 有什么前提要求？What are the prerequisites for learning and using TypeScript?

## 如何正确地、高效地学习 TypeScript？How to learn TypeScript properly and efficiently?

## TypeScript 的开发工具有哪些？What are the TypeScript development tools?

## FAQ 主题 FAQ Topics

### 类型及类型系统 主题 Type and Type System Topics

### 函数 主题 Function Topics

### 类 主题 Class Topics

#### TypeScript 中有抽象类吗？

​	TypeScript 中有抽象类，通过关键字 `abstract` 来声明抽象类。例如：

```typescript
abstract class Animal {
  public abstract shout():void;
}

class Cat extends Animal {
  public shout():void {
    console.log(`Meow ~ Meow ~~`);
  }
}
```

#### TypeScript 中支持内部类吗？

​	TypeScript 中支持内部类，通过对静态字段赋值一个类来实现。例如

```typescript
class Foo {
  public foo():void {
    const bar = new Foo.Bar();
    bar.bar(); // The console outputs the message 'TypeScript is great!'.
  }
  
  private static Bar = class Bar {
    public bar():void {
      console.log(`TypeScript is great!`);
    }
  };
}
```



#### TypeScript 中支持分部类（partial class）吗？

### 接口 主题 Interface Topics

### 枚举 主题 Enum Topics

### 继承与扩展 主题 Inheritance and Extension Topics

### 泛型 主题 Generic Topics

### 修饰符 主题 Modifier Topics

### 类型保护 主题 Type Guards Topics

### 类型声明 主题 Type Declaration Topics

### 模块化 主题 Module Topics

### 工程化 主题 Project Organization Topics

### 编译选项 主题 Compilation Topics

### 装饰器 主题 Decorator Topics
