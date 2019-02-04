# Cheat sheet for common C++ code

### Reading a line with spaces using scant
```
char str[100];
scanf("%[^\n]%*c", str);
```


### Finding LCM
```
long long gcd(long long a, long long b) {
    long long t;

    *while* (b != 0) {
        t = b;
        b = a % t;
        a = t;
    }

    *return* a;
}

long long lcm(long long a, long long b) {
    *return* (a * b) / gcd(a, b);
}

```



