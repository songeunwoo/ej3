# 58. 전통적인 for 문 보다는 for-each문(enhanced for statement)을 사용하라.

다음 경우들을 제외하고는 모든 경우에 for 대신 for-each를 사용하자.

1. 파괴적인 필터링(destructive filtering) - 컬렉션을 순회하면서 선택된 원소를 제거해야 한다면, 반복자의 remove 메소드를 호출해야 한다. 자바 8부터는 Collection의 removeIf 메서드를 사용해 컬렉션을 명시적으로 순회하는 일을 피할 수 있다.

2. 변형(transforming) - 리스트나 배열을 순회하면서 그 원소의 값 일부 혹은 전체를 교체해야 한다면 리스트의 반복자나 배열의 인덱스를 사용해야 한다.

3. 병렬 반복(parallel iterator) - 여러 컬렉션을 병렬로 순회해야 한다면 각각의 반복자와 인덱스 변수를 사용해 엄격하고 명시적으로 제어해야 한다.

> for-each 문은 컬렉션과 배열은 물론 Iterable 인터페이스를 구현한 객체라면 무엇이든 순회할 수 있다. Iterable을 처음부터 직접 구현하기는 까다롭지만, 원소들의 묶음을 표현하는 타입을 작성해야 한다면, Iterable을 구현하는 쪽으로 고민해보기 바란다.

> 전통적인 for 문과 비교했을 때 for-each 문은 명료하고, 유연하고, 버그를 예방시켜준다. 서능 저하도 없다. 가능한 모든 곳에서 for-each문을 사용하자!
