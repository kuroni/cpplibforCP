# dataStructure.hpp

Data Structures are ideals or models, It is hard to write once, used everywhere, for example, `Segment Tree, Disjoint set union, Mo's algorithm`, monicDeque, monicStack. We will provide some Frames (you should implement it to meet for needs)


## method

### nextBinom

Just the same as `next_permutation` to bruteForce all permutation, we have `nextBinom` to bruteForce all Binom.
for example `bruteForceBinom(2, 4)` will get

``` markdown
0 1
0 2
0 3
1 2
1 3
2 3
```

and It can be used in `ECC`


### discrete

``` cpp
#include <bits/stdc++.h>
#define clog(x) std::clog << (#x) << " is " << (x) << '\n';
using LL = long long;
#include "cpplib/all.hpp"

int main() {
  // freopen("in", "r", stdin);
  std::cin.tie(nullptr)->sync_with_stdio(false);
  std::vector<int> a{-12, 232, 12, 23};
  auto b = discrete(a);
  for (auto &x : a) std::cout << x << ' ';
  std::cout << '\n';
  for (auto &x : b) std::cout << x << ' ';
  std::cout << '\n';
  return 0;
}
// output:
// 0 3 1 2
// -12 12 23 232
```

## DSU: Disjoint Set Union

## Bit tree

- BitreeMin: min version
- Bitree: origin version(provide binary search)
- BitreePlus: plus version(support segment add)

## SegmentTree

There are two versions: sum and `min/max`

`min/max` version slightly hard: you should record `min/max`, and second `min/max` value: [https://codeforces.com/gym/102992/problem/J](https://codeforces.com/gym/102992/problem/J)

## Persistent Segment Tree

It save all version of update, and version number are saved in `roots`.

> Is this data structure used in Git ?

## BitPstSegTree

Bitree inside a Persistent Segment Tree to get dynamic k-th smallest number(online algorithm)

## subsequence

- LIS: length of longest increasing subsquence
- LNDS: length of longest non-decreasing subsquence
- LISP: (one of) longest increasing subsquence

## Cartesian Tree

## CDQ divided and conquer

## second Block
