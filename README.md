TypeScript Declare a Fake Module Demo
=====================================

如何在typescript中定义假的module（这个假module可用来作为占位符，然后在webpack中将它替换为真正的代码，
以实现在不同环境下打包不同代码的作用，比如node/web）

有两种不同的方式：

1. 使用`.d.ts`：需要在tsconfig的`files`中声明，否则在代码中使用不了
2. 使用`.ts`：不需要在tsconfig中声明，但是在代码中使用时，需要先import

可以根据不同的情况选择不同的做法。

```
npm install
npm run demo
```

对于本demo来说，编译通过就说明一切正常。运行时会报如下面的错：

```
Cannot find module '#fake1'
```
