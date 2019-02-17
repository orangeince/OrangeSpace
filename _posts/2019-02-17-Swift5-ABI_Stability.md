---
layout: post
title:  "Swift5 ABI稳定带来的一些影响"
date:   2019-02-17
category:  "Design Pattern"
tag: "Design Pattern"
---
## 好处都有啥
- App不需再自带Swift runtime，因此App占用体积会变小
- 新的Swift runtime和操作系统深度融合并优化，所以App会启动更快，并且有更好的运行性能和更低的内存占用
- Apple以后将会使用Swift来发布平台framework到各操作系统
- 当将来的Swift版本支持`Module stability`模块稳定时，第三方可以使用swift来写framework

## 哪些语言特性和改进提议在未来的OS版本中会被限制
- 标准库的扩张，包括新类型，协议，函数，属性等
- 类型系统的更改，包括新增类型和对已有类型的更改等

## 如果我想继续使用Swift4.0和4.2来维护已有代码的兼容性，会受到ABI稳定的影响吗？ABI稳定会影响我将来迁移代码到新语言吗？
- 不会。语言代码的兼容性不受ABI的影响。

## 我需要使用xcode10.2重新编译现有的App来让它在最新的系统上运行吗？
- 现有的App会继续使用它自身所带的旧Swift runtime来运行，直到runtime和稳定的ABI不兼容。不迁移代码的话，不能享受App store的App瘦身功能

## 我可以选择打包一个新的Swift runtime来使用新特性，而不需要新的OS支持吗？
- 不可以

## 有没有什么可以做的，以允许运行时支持新的Swift功能向后部署到旧操作系统？
- 有一些运行时功能是可能的。但不是一定会成功。成功向后部署功能的能力从根本上受旧操作系统中发布的二进制工件的限制和现有bug的限制。
