# [C++] 내림차순 정렬 : vector 

- `greater<int>()` 를 `sort()` 함수의 인자로 넣는다.

```c++
#include <iostream>
#include <algorithm>
#include <vector>
using namespace std;
vector<char> v(5);
int main()
{
    for (int i = 0; i < 5; i++)
    {
        cin >> v[i];
    }
    sort(v.begin(), v.end(), greater<int>());
    for (int i = 0; i < 5; i++)
    {
        cout << v[i] << ' ';
    }
    return 0;
}

```

![image-20210223000212782](C:%5CUsers%5Cshim5%5CAppData%5CRoaming%5CTypora%5Ctypora-user-images%5Cimage-20210223000212782.png)

