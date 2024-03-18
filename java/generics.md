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