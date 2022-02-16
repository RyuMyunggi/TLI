# BASE
### 참고자료
* [NoSQL BASE 속성](http://blog.skby.net/nosql-base-%EC%86%8D%EC%84%B1/)
* [nosql 기본 개념 정리](https://ojava.tistory.com/129)
* [[DA] NoSQL의 주요 개념 - Eventually Consistent, BASE, CAP](https://m.blog.naver.com/jeonghj66/221488308779)
### 개념
- ACID와 대조적으로 가용성과 성능을 중시하는 특성을 가진 분산시스템의 특성. 
- 즉 데이터의 약간의 문제가 있더라도 일단 내려줌
### Base Avaliable
- 기본적으로 사용 가능하다는 의미
- 부분적으로 고장은 있을 수 있으나 나머지는 사용가능하다
- 주 서버가 동작하지 않아도 백업 서버는 동작한다
### Soft State
- 외부의 개입이 없이도 정보가 변경될 수 있음. 네트워크 파티션 등 문제가 발생되어 일관성이 유지되지 않는 경우 일관성을 위해 데이터를 자동으로 수정
- 분산 노드 간 업데이트는 데이터가 노드에 도달한 시점에 갱신
### Eventually Consistent
- 일시적으로 비일관적인 상태가 되어도 최적으로는 일관성이 있는 상태가 되는 성질
- 시스템 부하, 네트워크 속도 등의 외부 요인으로 일관성이 있는 일시적으로 깨질 수 있음