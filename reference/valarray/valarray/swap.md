#swap (C++11)
```cpp
void swap(valarray& v) noexcept;
```

##概要
他の`valarray`オブジェクトと値を入れ替える。


##効果
`*this`の内容を`x`と交換する。


##計算量
定数時間


##例
```cpp
#include <iostream>
#include <valarray>

template <class T>
void print(const char* name, const std::valarray<T>& v)
{
  std::cout << name << " : {";
  bool first = true;

  for (const T& x : v) {
    if (first) {
      first = false;
    }
    else {
      std::cout << ',';
    }
    std::cout << x;
  }
  std::cout << "}" << std::endl;
}

int main()
{
  std::valarray<int> a = {1, 2, 3};
  std::valarray<int> b = {4, 5, 6};

  a.swap(b);

  print("a", a);
  print("b", b);
}
```

###出力
```
a : {4,5,6}
b : {1,2,3}
```


##バージョン
###言語
- C++11

###処理系
- [Clang](/implementation#clang.md): 3.0
- [GCC](/implementation#gcc.md): 
- [GCC, C++0x mode](/implementation#gcc.md): 4.7.3
- [ICC](/implementation#icc.md): ??
- [Visual C++](/implementation#visual_cpp.md) ??

