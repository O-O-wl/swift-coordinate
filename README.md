# Swift-Coordinate

다형성에 대해 공부한 프로젝트이다.

앞으로의 요구사항이 추가될 때 코드는 어떤 식으로 변화하는가?

변경사항을 줄일 수 있나? 를 공부했다.

**로버트.C.마틴 - 클린코드**에서 객체와 자료구조 장을 보면 
책을 느끼며 둘의 차이는 이러했다.

자료구조는 하나의 메소드 추가에 대해서는 자료구조를 처리하는 메소드가 바빠질뿐 기존 타입들에게 영향을 미치지 않는다.
대신 자료구조들을 처리하는 객체는 타입의 확장에 대해 무조건적이 수정이 필요해진다.'

반면 많은 객체를 구현한 인터페이스에 추가 요구사항이 생기게되면 
이전 객체들은 그 수정전까지는 자격을 가지지 못하게된다. (자격을 갖추지 못햇기에)
그런데 객체의 타입의 너무 많다면? 아마 엄청난 수정이 발생할 것이다.

타입의 추가와 인터페이스의 추가 어떤 것이 자주 일어나는 지에 따른 객체 설계가 필요할 것 같다.

객체로 구현하게되면 타입추가에 용이하다 - 특정 인터페이스에 의존하게 된다면
특정인터페이스의 조건을 만족하면 객체가 될 수 있었다.

좌표계산기에서 `[Point]`의  가지고 있다면 `Figure`(도형)의 조건을 만족하게되고,
그 결과적을 저 조건을 만족하는 객체들을 모두 유연하게 수용할 수 있었다.



## 좌표계산기 실행 영상

![ezgif com-video-to-gif](https://user-images.githubusercontent.com/39197978/61314630-05c5e100-a838-11e9-8fd4-34d578f1ae1a.gif)
