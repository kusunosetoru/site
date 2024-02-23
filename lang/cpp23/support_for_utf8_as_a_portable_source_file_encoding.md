# 汎用的なソースコードのエンコーディングとしてUTF-8をサポート
* cpp23[meta cpp]

## 概要
C++20まで、ソースコードの文字集合は実装定義だったが、その仕様では移植性に問題があった。C++23からは、すべてのコンパイラはUTF-8文字コードのソースコードをサポートしなければならないことが規定される。

コンパイラは、ほかの文字コードと区別するため、入力ファイルがUTF-8であることを決定する実装定義の手段をもたなければならない。つまり、BOM (バイトオーダーマーク) を認識するだけでは十分ではない。


## 参照
- [P2295R6 Support for UTF-8 as a portable source file encoding](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2022/p2295r6.pdf)