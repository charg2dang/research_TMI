# Index

인덱스는 별도의 파일로 존재 용량을 잡아 먹는다.
인덱스는 정렬되어 있다.(clustered index일 때ㅔ)
인덱스를 사용하면 조회가 빨라진다.

인덱스는 갱신, 추가, 삭제를 느리게 한다. 각 연산마다 인덱스를 유지해야 하기 떄문에 비용이 든다.

1. 전체 검색은 대량의 데이터 검색에 적합하지 않다.
2. 원하는 위치까지 '순식간'에 도달하는 방법

## 인덱스 구조

![Index/Untitled.png](Index/Untitled.png)

key - value 구조

![Index/Untitled%201.png](Index/Untitled%201.png)

![Index/Untitled%202.png](Index/Untitled%202.png)

**데이터가 적은 경우** 
일단 보조기억장치의 인덱스 파일에 액세스 하고 실제 테이블에 액세스(2회) 하기떄문에 로우의 갯수가 적은 경우엔 인덱스를 통하지 않고 바로 데이터를 검색하는게 이득이다. 
( 이 부분은 물리적 데이터베이스 설계에 더 자세히 나온다.)

**데이터가 많은 경우**

인덱스파일에서 해당위치를 검색

내부 구조 

B+ Tree,

 B Tree

# Reference

데이터 베이스를 지탱하는 기술 2장