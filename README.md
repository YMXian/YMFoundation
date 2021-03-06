# YMFoundation

[![Build Status](https://travis-ci.org/YMXian/YMFoundation.svg)](https://travis-ci.org/YMXian/YMFoundation)

一米鲜 iOS App 基础库合集

# 介绍

一米鲜 iOS App 开发过程中，研发团队自己动手从头开发了很多库，其中包含：

* 网络请求库，包含以下特性：
  * 基于 NSURLSession
  * 请求模板
  * 调试信息记录
  * 链式结果转换

* JSON 映射库，包含以下特性:
  * 面向接口设计，兼容其他形式的 JSON 映射
  * 更强大的泛型支持
  * 显式属性声明 (Fool-proofing)

* 异步队列
  * 受 Node.js 启发
  * 最初用于防止 VC 操作冲突
  * 设计上更为轻量级，可以兼容一切基于 Block 的异步调用

* 基于 Plist 的 i18n 方案
  * 支持命名空间
  * 支持多个文件
  * 自动缓存以提高性能

* URL 路由系统
  * 受常见服务器路由(Rails, Express 等等)设计启发
  * 支持路由之间相互注册
  * 面向接口，便于接入带回调的第三方SDK
  * 支持`:name`语法，实现路径内带参

* 依赖注入系统
  * 受 AngularJS 启发

同时我们还嵌入了 `ReactiveCocoa 2.5`，准备向 `ReactiveCocoa` 导入新的 `Objective-C` 语言特性。

尽管我们的团队还很年轻，我们的工作尚不完善，我们依旧迫不及待地想要和大家分享我们的成果，我们会在内部协商后，尽可能全面，尽可能快地开放上述内容。

# 开发风格

我们会快速跟进最新的正式版 Xcode 和 iOS SDK，并在满足兼容性的前提下，将新特性融入到代码中。比如说 Xcode 6.4 - 7 引入的泛型和空值标注`__nonnull`。

代码风格尽可能地跟进 Google Objective-C 代码风格(AppCode 内置)。

# 开源协议

我们使用 MIT 协议，详情参见 `LICENSE` 文件
