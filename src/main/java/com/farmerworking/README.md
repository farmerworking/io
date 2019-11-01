# 总结
## 系统调用
1. 直接减少系统调用 —— Client2
2. 通过 buffer 方式减少系统调用 —— BufferedClient

## GC
1. 减少临时对象创建，避免 young gc —— BufferedClient3，BufferedClient2 (反例)

## Buffer vs Stream
1. 利用 Java NIO 中的 channel 和 byteBuffer —— ByteBufferClient

## 内存拷贝
1. 使用 ByteBuffer.duplicate 创建一份引用而不是拷贝 —— ByteBufferClient3


ByteBufferClient2 ???