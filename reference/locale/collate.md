#collate
* locale[meta header]
* std[meta namespace]
* class template[meta id-type]

```cpp
namespace std {
  template <class charT>
  class collate : public locale::facet;
}
```
* locale::facet[link /reference/locale/locale/facet.md]

##概要
(ここに、クラスの概要を記載する)

###メンバ関数

| | |
|----------------------------|--------------------------------------------|
| `(constructor)` | コンストラクタ |
| `compare` | 文字列を比較する |
| `transform` | 文字の範囲を文字列に変換する |
| `hash` | 文字範囲のハッシュ値を求める |

###protectedメンバ関数

| | |
|---------------------------|--------------------------------------------|
| `(destructor)` | デストラクタ |
| `do_compare` | 文字列を比較する |
| `do_transform` | 文字の範囲を文字列に変換する |
| `do_hash` | 文字範囲のハッシュ値を求める |

###メンバ型

| | |
|-------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| `char_type` | 文字型 `charT` |
| `string_type` | 文字列型 [`basic_string`](/reference/string/basic_string.md)`<charT>` |

###例
```cpp
```

###出力
```
```

###参照
