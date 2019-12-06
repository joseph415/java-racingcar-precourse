##프리코스 2주차 자동차 경주게임

| 작성자 | git ID| 작성일시 | 변경사유 |
|---|---|---|---|
| 정은석 | joseph415 |2019.12.06 | WinsCar 수정, TryGame 구현  |

___

#####기능 요구 사항
* 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.

* 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
    - 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
    
* 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.

* 전진하는 조건은 0에서 9 사이에서 random 값을 구한 후 random 값이 4 이상일 경우 전진하고,
      3 이하의 값이면 멈춘다.
      
* 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.

___

#####기능 구현 목록
- [x] 차 객체를 생성하는 기능 
    - [x] 기본 생성자 추가할수 없음.
    - [x] name, position 변수의 접근 제어자인 private을 변경할 수 없음.
    - [x] 차의 position을 리턴하는 기능.
    - [x] 3 이하이면 멈추고 4이상이면 전진하는 기능.
    - [x] 차의 이름을 출력하는 기능
    
- [x] 자동차 이름을 입력
    - [x] 구분자 (,)로 파싱해서 배열에 입력
    - [x] 파싱한 결과로 자동차 동적 생성
    * 예외처리
    - [x] 글자수는 1~5글자 까지만 받는다. 예외시 재입력

- [x] 랜덤으로 생성하 기능
    - [x] 0부터 9까지 랜덤으로 값 생성
    
- [x] 사용자에게 시도회수를 입력받는 기능
    * 예외처리
    - [x] 시도횟수는 1회 이상입력

- [x] 게임 시작시키는 기능
    -[x] 시도횟수만큼 게임 진행
    -[x] 시도할때마다 차의 위치 출력
    -[x] 게임을 구성하는 기능
    
- [x] 우승자를 가리는 기능
    - [x] 각 객체의 전진 회수를 체크한다.
    - [x] 우승자를 출력한다.
    - [x] 우승자 1명이상 가능.
    