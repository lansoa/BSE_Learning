# Effective C++

## Chapter 1

#### Item 1

View c++ as a federation

1. fundamental C
2. objective-oriented C++
3. template C++
4. STL

#### Item 2

Using const replace #define. 

const pointer shuold be `const chat * const authorName`

`enum {NumTurns = 5}` like `#defilne`

- simple constants, perfer `const` objects or `enums` 
- for funtion, perfer inline funtion 

### Item 3

Using const whenever possible.

```c
char *p = greeting;               // non-const pointer,
                                  // non-const data
const char *p = greeting;         // non-const pointer,
                                  // const data
char * const p = greeting;        // const pointer,
                                  // non-const data
const char * const p = greeting;  // const pointer,
                                  // const data
void f1(const Widget *pw);        // f1 takes a pointer to a
void f2(Widget const *pw);        // constant Widget object so does f2

```