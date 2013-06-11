# C++ expression parsing.
Expression parsing in C++ with Dijkstra's
[Shunting-yard algorithm](http://en.wikipedia.org/wiki/Shunting-yard_algorithm).

Original version by
[Jessee Brown](http://www.daniweb.com/software-development/cpp/code/427500/calculator-using-shunting-yard-algorithm).

## Minimal example.
```C
#include <stdio>
#include "shunting-yard.h"

int main() {
  std::cout << calculator::calculate ("(20+10)*3/2-3") << std::endl;
  return 0;
}
```

## Features.
 + Operators: +, -, /, +, <<, >>
 + Map of variable names to be replaced in string.

## TODO
 + Unary operators.
 + Make a PersistentCalculator object to store data
   to make chains of calculations possible.
 + Suggestions from post.