#ios_base::sync_with_stdio(false)

###장점
 - c의 stdio와 cpp의 iostream을 동기화 시켜, iostream과 stdio의 버퍼를 모두 사용하기 때문에 생기는 딜레이를 false해버림
 - cpp만의 독립적인 버퍼가 생성되어, c의 버퍼와 병행하여 사용할 수 없지만, 사용하는 버퍼의 수가 줄어들어 실행속도가 빨라짐

###단점
 - 동기화 된 c++ 버퍼의 경우 thread-safe하기 때문에 모든 IO의 순서가 예상한 것과 정확히 일치함, 이를 false해줌으로써 동기화가 비활성화 되어서 멀티 쓰레드 환경에서는 출력 순서를 보장할 수 없게됨
 - 버퍼가 분리되어 cin과 c의 scanf, gets, getchar 등을 같이 사용하면 안되고 count과 c의 printf, puts, putchar 등을 같이 사용하면 잘못된 결과가 나올 확률이 높음.
 
