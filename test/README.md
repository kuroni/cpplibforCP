# Welcome your tests

## Example

You may add test here for example:

add file `docs/test/math/poly1.cpp` to solve $n! \mod p$ in [SPOJ](https://www.spoj.com/problems/FACTMODP/en/)

``` cpp
// docs/test/math/poly1.cpp
#include <bits/stdc++.h>
#define clog(x) std::clog << (#x) << " is " << (x) << '\n';
using LL = long long;
#include "../cpplib/math.hpp"

// https://www.spoj.com/problems/FACTMODP/en/
int main() {
  // freopen("in", "r", stdin);
  std::cin.tie(nullptr)->sync_with_stdio(false);
  int cas = 1;
  std::cin >> cas;
  while (cas--) {
    LL n, p;
    std::cin >> n >> p;
    std::cout << factorial(n, p) << '\n';
  }
  return 0;
}
```