# #include <bits/stdc++.h>

### 장점
 - Pre-compiled header의 일종으로, 사람들이 많이 사용하는 표준 라이브러리 헤더들을 모두 한번에 Compile 될 수 있도록 해둠
 - 알고리즘 대회같은 곳에서 코딩 시간을 줄이기 위해 많이 사용함

### 단점
 - 모든 header를 compile해야 하는 상황을 맞이 하기 때문에, 불필요한 연산작업이 들어가 컴파일 시간이 느려지고, 프로그램의 크기가 쓸데없이 커지게됨 (ex) java의 import java.util.*;)
