# UML 다이어그램
## 선택한 이유 & 시사점 등
> UML이 통합모델링언어이고 UML다이어그램이 모델 요소, 시나리오 등을 시각화해 의사소통을 용이하게 한다... 는 건 알겠지만 여전히 추상적이고 UML 다이어그램이 그래서 도대체 무엇인가 싶어 자세히 다루어 보았다.
-------------
## 내용작성 

### UML이 중요한 이유
건축 등의 실제 세게에서의 설계는 구현 이전에 모델링을 통한 설계 검증이 필수다. 비용적으로도 훨씬 저렴하고 예상치못한 위험을 큰 피해를 입기 전에 확인할 수 있기 때문이다.

소프트웨어 설계 또한 하드웨어적인 설계들과 마찬가지로 설계 과정에서 모델링이 많은 도움이 된다. 개발자가 시스템의 구조를 파악하기 쉽고, 파악이 쉬우니 서로 설계와 관련된 의사소통을 하기가 쉬워진다.

하지만 소프트웨어 설계는 하드웨어적인 설계와는 다르게 모델링의 비용절감이 아주 극적이지는 않다. 모델링을 하는 것이 오히려 비용도 많이 들고 비효율적일 수도 있다. 그럼에도 많은 장점이 있고 널리 사용되므로 자세히 파악해보자.

#### UML의 장점
- 의사소통 및 설계 논의가 원활해진다.
- 전체 시스템의 구조나 클래스의 의존성을 쉽게 파악할 수 있다.
- 설계의 back-end 문서를 통한 유지보수에 용이하다.

### UML 다이어그램이란?
UML을 사용해 그리는 일종의 도면으로, 시스템의 구조나 흐름을 시각적으로 파악할 수 있도록 돕는다.

#### UML 다이어그램의 분류
UML은 구조 다이어그램 7개, 행위 다이어그램 7개로 총 14종류의 다이어그램이 있다.
![image](https://www.nextree.co.kr/content/images/2021/01/--1-UML---.png)
구조 다이어그램은 시스템의 개념, 관계 등 정적인 면을 보기 위한 것이고, 행위 다이어그램은 요소들의 변화, 흐름, 동작 등을 보기 위한 것이다.

### 대표적인 UML 다이어그램들
##### Structural/Static Diagram
1. Class Diagram
![image](https://cms.boardmix.com/images/kr/articles/2022/skills/what-is-uml-diagram1.png)
클래스의 정적인 내용과 클래스 간의 관계를 표기한다. *객체 지향 시스템에서 공통적으로 많이 쓰인다.* 의존 관계를 명확히 보여줘, 순환 의존이 발생하는 지점을 찾아내 어떻게 해결하면 되는지 파악이 쉬워지기도 한다.

2. Package Diagram
![image](https://cms.boardmix.com/images/kr/articles/2022/skills/what-is-uml-diagram3.png)
여러 모델 요소를 그룹화하여 표현한다. 여러 클래스들의 묶음인 패키지들 사이의 의존관계를 잘 표현한다. (의존관계: 하나의 패키지가 다른 패키지를 사용하는 관계)

3. Component Diagram
![image](https://cms.boardmix.com/images/kr/articles/2022/skills/what-is-uml-diagram6.png)
시스템을 구성하는 요소들의 조직과 종속성을 보여준다. 클래스 다이어그램과 비슷한데, 클래스는 논리적인 추상화에 가깝고 속성과 오퍼레이션을 직접 가지지만, 컴포넌트는 물리적인 요소를 나타내고 자신의 인터페이스를 통해 접근 가능한 오퍼레이션만 가질 수 있다.

#### Behavioral/Dynamic Diagram
1. Use case Diagram
![image](https://cms.boardmix.com/images/kr/articles/2022/skills/what-is-uml-diagram2.png)
시스템과 사용자(Actor)의 상호작용 및 관계를 나타내는 다이어그램이다. 사용자가 어떤 시스탬의 어떤 기능을 사용할 수 있는지 나타내기 때문에 *요구사항 관련 의견 조율에 용이하다.*

2. Sequence Diagram
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F9957FA465F25731A34)
특정 행동이 어떠한 순서로 어떤 객체와 어떻게 상호작용 하는지 표현한다. 현 시스템이 *어떠한 시나리오로 움직이는지 파악하기 용이하다.*

3. State/Statechart Diagram
![image](https://cms.boardmix.com/images/kr/articles/2022/skills/what-is-uml-diagram4.png)
객체가 가지는 모든 가능한 상태를 표현한다. 진입 조건, 탈출 조건, (상태 전이에 필요한) 사건(Event) 등의 자세한 상황을 표현한다. 설계 단계에서 *객체가 어떤 동적 행동을 하는지 나타낼 때 주로 쓰인다.*

4. Activity Diagram
![image](https://cms.boardmix.com/images/kr/articles/2022/skills/what-is-uml-diagram5.png)
객체가 로직이나 조건에 따라 어떤 순서로 처리되는지 보여준다. 시작과 종료 상태, 선택점과 전이 등 클래스의 관계와 생명 주기를 표현한다. (ps. 무언가를 하고있는 상태를 '활동(Activity)'이라고 한다.)

## 마치며
UML, CASE 등등 여러 개발에 도움되는 도구들을 공부하다 보면 텍스트로만 배우기 때문에 잘 와닿지 않고 왜 배우는지 모르겠고 실제로 쓰기는 하는 건지 의문이 들때가 많지만, 일종의 CAD처럼 생각하면 이해가 한결 편해진다. 하드웨어적인 설계 과정에서 설계 툴, 모델링 툴을 사용해야 한다는 게 자연스럽게 떠오르듯이 소프트웨어 설계에도 이러한 과정이 당연히 필요했던 것이다.

이렇듯 공부 과정에서 내용이 잘 와닿지 않는다면 실제로 어떻게 쓰이고 있는지 찾아보자. 이해 위주의 학습에 있어서는 많은 도움이 될 것이다.