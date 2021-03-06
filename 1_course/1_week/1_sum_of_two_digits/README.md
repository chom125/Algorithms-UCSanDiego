# 1. Sum of two digits
[https://en.wikipedia.org/wiki/Digit_sum](https://en.wikipedia.org/wiki/Digit_sum)

## Problem
![](docs/1_sum_of_two_digits.png)

## Solutions
* [C](#c)
* [C++](#cpp)
* [Java](#java)
* [Python3](#python3)

### C
```c
    #include <stdio.h>

    int sum_of_two_digits( int first, int second ){
        return first + second;
    }

    int main(){
        int a = 0, b = 0;
        scanf( "%d%d", &a, &b );
        printf( "%d\n", sum_of_two_digits( a, b ) );
        return 0;
    }
```

### CPP
```cpp
    #include <iostream>

    using namespace std;

    class Solution
    {
    public:

        int sum_of_two_digits( int first, int second )
        {
            return first + second;
        }

    };

    int main()
    {
        Solution solution;

        auto a{ 0 }, b{ 0 };
        cin >> a >> b;
        cout << solution.sum_of_two_digits( a, b );

        return 0;
    }
```

### Java
```java
    import java.util.Scanner;

    class APlusB {
        static int sumOfTwoDigits( int first, int second ){
            return first + second;
        }

        public static void main( String[] args ){
            Scanner s = new Scanner( System.in );
            int a = s.nextInt();
            int b = s.nextInt();
            System.out.println( sumOfTwoDigits( a, b ) );
        }
    }
```

### Python3
```python
    def sum_of_two_digits( first, second ):
        return first + second

    if __name__ == '__main__':
        a, b = map( int, input().split() )
        print( sum_of_two_digits( a, b ) )
```