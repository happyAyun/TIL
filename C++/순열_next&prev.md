# [C++] 순열 - 다음 순열과 이전 순열 : vector, 배열

- 다음 순열 : `next_permutation(순열의 시작, 순열의 끝)`
- 이전 순열 : `prev_permutation(순열의 시작, 순열의 끝)`
- 두 함수의 인자는 범위가 들어간다.

- vector와 배열은 인자의 표현방식의 차이가 있다.



- 배열의 경우, 배열의 이름이 주소를 나타내므로, 이름과 함께 범위를 나타낸다.

```c++
#include <iostream>
#include <algorithm>
#include <vector>
using namespace std;
int arr[5];
int main()
{
    for (int i = 0; i < 5; i++)
    {
        cin >> arr[i];
    }
    if (next_permutation(arr, arr + 5))
    {
        for (int i = 0; i < 5; i++)
        {
            cout << arr[i] << ' ';
        }
    }
    cout << '\n';
    if (prev_permutation(arr, arr + 5))
    {
        for (int i = 0; i < 5; i++)
        {
            cout << arr[i] << ' ';
        }
    }
    return 0;
}


```

