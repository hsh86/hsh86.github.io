# java反射
Java 反射是指在运行时动态加载类并获取类的信息（包括方法、属性、注解等），并能操作类的属性和方法的一种能力。

## 获取 Class 对象
`Class<?> clazz = Class.forName("java.lang.String");`

## nio简介
非阻塞式 I/O、选择器、通道、缓冲区等新的概念和机制。相比与传统的 I/O 多出的 N 不是单纯的 New，更多的是代表了 Non-blocking 非阻塞，NIO具有更高的并发性、可扩展性以及更少的资源消耗等优点。

## 定义
NIO：是同步非阻塞的，服务器实现模式为 一个线程处理多个连接。服务端只会创建一个线程负责管理Selector（多路复用器），Selector（多路复用器）不断的轮询注册其上的Channel（通道）中的 I/O 事件，并将监听到的事件进行相应的处理。每个客户端与服务端建立连接时会创建一个 SocketChannel 通道，通过 SocketChannel 进行数据交互。



# java泛型
泛型的本质是参数化类型，也就是说所操作的数据类型被指定为一个参数。

## 泛型类
类名后面添加了类型参数声明部分。

```
public class Box<T> {
   
  private T t;
 
  public void add(T t) {
    this.t = t;
  }
 
  public T get() {
    return t;
  }
 
  public static void main(String[] args) {
    Box<Integer> integerBox = new Box<Integer>();
    Box<String> stringBox = new Box<String>();
  }
}
```


## @Resource 详解
@Resource注解与@Autowired类似，也是用来提供依赖注入的  
@Resource注解是Java层面所提供的注解，@Autowired是Spring所提供的注解，

**依赖注入**  
*java提供*

## spring-boot-configuration-processor是干什么用的
作用是生成配置的元数据信息。