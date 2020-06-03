# my_valgrind_memory
Awesome valgrind memories.

## 关于`--track-origins=yes`
当出现'Conditional jump or move depends on uninitialised value(s)'这样的error时，我们需要使用`--track-origins=yes`然后就可以通过错误提示可以精确定位到哪个变量，例如：常见的new[]了一个空间之后，没有初始化，则会报：  
```Uninitialised value was created by a heap allocation```  
