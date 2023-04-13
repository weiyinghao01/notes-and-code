### 1. C++基础





### 2. STL



#### 1. String





#### 2. Vector

**初始化**

```c++
std::vector<int> b{3}; // creates a 1-element vector holding {3}
std::vector<int> a(3); // creates a 3-element vector holding {0, 0, 0}
 
std::vector<int> d{1, 2}; // creates a 2-element vector holding {1, 2}
std::vector<int> c(1, 2); // creates a 1-element vector holding {2}
```

`push_back`

```c++
#include <vector>
#include <iostream>
#include <iomanip>
#include <string>
 
int main()
{
    std::vector<std::string> letters;
 
    letters.push_back("abc");
    std::string s{"def"};
    letters.push_back(std::move(s));
 
    std::cout << "std::vector `letters` holds: ";
    for (auto&& e : letters) std::cout << std::quoted(e) << ' ';
 
    std::cout << "\nMoved-from string `s` holds: " << std::quoted(s) << '\n';
}
```

`Possible output:`

```sh
std::vector `letters` holds: "abc" "def" 
Moved-from string `s` holds: ""
```



#### 3. List



#### 4. Set



#### 5. Unordered_map







### 3. 智能指针

+ std::unique_ptr   -  single ownership
+ std::shared_ptr   -  shared ownership
+ std::weak_ptr  -  temp / no ownership



![image-20230404201024479](https://blog-1309244887.cos.ap-nanjing.myqcloud.com/blog/image-20230404201024479.png)





![image-20230404202938533](https://blog-1309244887.cos.ap-nanjing.myqcloud.com/blog/image-20230404202938533.png)





![image-20230404203855133](https://blog-1309244887.cos.ap-nanjing.myqcloud.com/blog/image-20230404203855133.png)











