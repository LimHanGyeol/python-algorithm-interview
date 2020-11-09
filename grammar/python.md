# 파이썬 문법

## 인덴트 (Indent)
* 공식 가이드 PEP 8에 따라 공백 4칸을 원칙으로 한다.
* 코드 첫 번째 줄에 파라미터가 있다면, 파라미터가 시작되는 부분에 맞춘다.
* 코드 첫 번째 줄에 파라미터가 없다면, 공백 4칸 인덴트를 한 번 더 추가하여 다른 행과 구분되게 한다.

## 네이밍 컨벤션
* 파이썬의 네이밍 컨벤션은 자바와 달리 각 단어를 하이픈(_)으로 구분하여 표기하는 스네이크 케이스(Snake Case)를 따른다.
* 파이썬은 Pythonic Way를 준수하여 카멜 케이스 뿐만 아니라 자바 스타일의 컨벤션을 지양한다.
* 컨벤션으로 인한 질문을 받게 되면 "파이썬의 PEP 8 및 철학에 따라 스네이크 코딩을 지향한다."라고 답할 수 있어야 한다.

## 타입 힌트 (Type Hint)
* 파이썬은 대표적인 동적 타이핑 언어임에도, 타입을 지정할 수 있는 Type Hint 가 PEP 484 문서에 추가됐다.
* 해당 기능은 파이썬 3.5 버전 부터 사용할 수 있다.
* 파이썬의 타입 추론은 빠르게 정의해서 사용할 수 있는 장점이 있지만, 파라미터의 타입과 리턴값이 무엇인지 알 수 없다.  
프로젝트 규모가 커지게 되면 가독성을 떨어트리게 되며 버그 유발의 주범이 된다.  
타입 힌트를 사용하면 파라미터 및 리턴 타입을 분명하게 알 수 있다. 가독성도 좋아지며 버그 발생 확률을 줄일 수 있다.
* 실제로는 강제 규약이 아니다 보니, 여전히 동적으로 할당될 수 있으므로 주의가 필요하다.
* 코딩 테스트는 일반적으로 짧은 알고리즘으로 끝나는 경우가 많고, 타입은 지정하지 않아도 한눈에 보일 만큼 명확하기 때문에 굳이 지정하지 않아도 문제는 없다.  
그러나 코드를 정리할 때만이라도 타입을 모두 지정해서 보기좋게 제출한다면, 코드 리뷰 시 면접관에게 좋은 점수를 받을 수 있을 것이다.

## 리스트 컴프리헨션
* 파이썬은 map, filter 와 같은 함수형 (Functional) 기능을 지원하며 람다 표현식 (Lambda Expression) 도 지원한다.
* 리스트 컴프리헨션 (List Comprehension) 이란 기존 리스트를 기반으로 새로운 리스트를 만들어 내는 구문으로,  
파이썬 2.0 부터 지원 되었으며, 하스켈 (Haskell) 같은 함수형 언어에서 기능을 차용해온 파이썬의 대표적인 특징이기도 하다.
* 리스트 컴프리헨션이 리스트만 가능한 것은 아니다. 버전 2.7 이후 리스트 외에도 딕셔너리 등이 가능하도록 추가됐다.
* 한 줄로 간결하게 작성할 수 있는 리스트 컴프리헨션은 가독성이 좋은 편이지만 이 또한 무리하고 복잡하게 작성할 경우 가독성을 떨어트릴 수 있으므로 적절히 사용하는 게 중요하다.  
대체로 표현식은 2개를 넘지 않아야 한다.
