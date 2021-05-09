# C++ and Python_ 210509

- 문자열을 받을 경우
  - 앞서 cin 을 통해 int 형 숫자를 입력받았을 경우,
  - getline(cin, str) 을 통해 문자열을 입력받기 전 
  - cin.ignore() 을 통해서 버퍼에서 enter키를 지워주어야 한다.

```c++
#include <bits/stdc++.h>
using namespace std;
string str;
int stepx[] = {-2, 2, -2, 2, 1, 1, -1, -1};
int stepy[] = {1, 1, -1, -1, 2, -2, 2, -2};
int main()
{
    getline(cin, str); // c2라고 가정하면
    int x = str[0] - 'a' + 1; // str의 원소 하나(char)에서 'char'을 빼고 int로 변수를 선언하여 주면 아스키코드 계산의 결과 int형으로 변환
    int y = str[1] - '0'; // c2의 2도 string형으로 받았기 때문에 연산을 수행하기 전에 '0'의 char을 빼주어 int형으로 변환해주어야 한다.
    int result = 0;
    for (int i = 0; i < 8; i++)
    {
        int dx = x + stepx[i];
        int dy = y + stepy[i];
        if (dx < 1 || dy < 1 || dy > 8 || dx > 8)
            continue;
        result++;
    }
    cout << result << '\n';
    return 0;
}
```



- python 
  - for i in range(n) == for i in rango(0,n)
  - i = 0 ~ n-1