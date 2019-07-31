## 메소드 시그니처를 신중히 설계하라.

## 메소드 설계요령
1. 메소드 이름을 신중히 짓자 
   * 일관된 이름, 긴이름 피하기
2. 편의 메소드를 너무 많이 만들지 말자.
   * 너무많은 메소드를 가진 클래스는 익히고 사용하기, 유지보수하기 힘들다
   * 확신이 서지 않으면 만들지 말자
3. 매개변수 목록은 짧게유지하자 
   * 매개변수 목록은 4개이하가 좋다
   * 같은타입의 매개변수 여러개 연달아 나오는 경우를 피하자
   * 매개변수 목록이 길경우 여러개로 쪼개자 
      => 클래스가 많아 질수 있지만 메소드를 적절히 나누면 메소드 조합을 통해 원하는 기능
         가능 할수 있다.
   * 매개변수를 묶어주는 도우미 클래스를 만들어라
4. 매개변수 타입으로는 클래스 보다는 인터페이스가 낫다
5. boolean 보다는 우너소 2개짜리 열거타입이 낫다
