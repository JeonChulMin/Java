# 자바란?



# 1. 자바의 역사

 자바의 역사는 1991년 썬의 엔지니어들에 의해서 고안된 Oak라는 언어에서부터 시작되었다. 원래 목표는 가전제품에 탑재될 소프트웨어를 만드는 것이었다. 하지만 여러 종류의 운영체제를 사용하는 컴퓨터들이 통신하는 인터넷이 등장하자 운영체제에 독립적인 Oak를 인터넷에 적합하도록 개발하면서 이름을 Java로 변경하였으면 1996년 1월에 자바의 정식 버전을 발표했다. 

 2010년 썬이 Oracle에 인수되면서 자바 또한 Oracle의 제품이 되었다.



# 2. 자바 언어의 특징



## 1) 운영체제 독립적이다.

 기존의 언어는 한 운영체제에 맞게 개발된 프로그램을 다른 운영체제에 적용하기 위해 많은 노력이 필요하였지만, 자바는 일종의 에뮬레이터인 JVM을 통해, 자바 응용 프로그램은 운영체제나 하드웨어가 아닌 JVM하고만 통신하고 JVM이 자바 응용 프로그램으로부터 전달받은 명령을 해당 운영체제가 이해할 수 있도록 변환하여 전달한다. 자바로 작성된 프로그램은 운영체제에 독립적이지만 JVM은 운영체제에 종속적이어서 운영체제마다 서로 다른 버전의 JVM을 제공한다.



## 2) 객체지향언어이다.

  객체지향 프로그래밍언어 중 하나로 객체지향개념의 특징은 상속, 캡슐화, 다형성이 잘 적용된 언어라는 평가를 받고 있다.



## 3) 비교적 배우기 쉽다.

 자바의 연산자와 기본구문은 C++에서, 객체지향관련 구문은 스몰톡이라는 객체지향언어에서 가져왔다. 이 두 언어의 장점은 취하면서 복잡한 부분은 제거해 단순화함으로써 간결하고 이해하기 쉬운 코드를 작성할 수 있도록 하였다.



## 4) 자동 메모리 관리 (Garbage Collection)

 자바로 작성된 프로그램이 실행되면 가비지 컬렉터가 자동적으로 메모리를 관리해주기 때문에 프로그래머는 따로 메모리를 관리하지 않아도 된다.



## 5) 네트워크와 분산처리를 지원한다.

 인터넷과 대규모 분산환경을 염두에 두어 다양한 네트워크 프로그래밍 라이브러리(Java API)를 통해 비교적 짧은 시간에 네트워크 관련 프로그램을 쉽게 개발할 수 있도록 지원한다.



## 6) 멀티쓰레드를 지원한다,

 자바에서 개발되는 멀티쓰레드 프로그램은 시스템과는 관계없이 구현가능하며, 관련된 라이브러리가 제공되므로 구현이 쉽다. 그리고 여러 쓰레드에 대한 스케줄링을 자바 인터프리터가 담당하게 된다.



## 7) 동적 로딩(Dynamic Loading)을 지원한다.

 자바는 동적 로딩을 지원하기 때문에 실행 시에 모든 클래스가 로딩되지 않고 필요한 시점에 클래스를 로딩하여 사용할 수 있다는 장점이 있다. 그 외에도 일부 클래스가 변경되어도 전체 애플리케이션을 다시 컴파일하지 않아도 되며, 애플리케이션의 변경사항이 발생해도 비교적 적은 작업만으로도 처리할 수 있는 유연한 애플리케이션을 작성할 수 있다.



# 3. JVM (Java Virtual Machine)

 JVM은 '자바를 실행하기 위한 가상 기계'로 여기서 가상 기계는 실제 컴퓨터가 아닌 소프트웨어로 구현된 컴퓨터라는 뜻으로 컴퓨터 속의 컴퓨터라고 생각하면 된다. 자바로 작성된 애플리케이션은 모두 이 가상 컴퓨터(JVM)에서만 실행되기 때문에, 자바 애플리케이션이 실행되기 위해서는 반드시 JVM이 필요하다.

[JVM.md 파일 링크 넣기]



# 4. 자바 개발 도구 (JDK)

 자바로 프로그래밍을 하기 위해서는 먼저 JDK(Java Development Kit)를 설치해야 한다. JDK를 설치하면, JVM과 Java API 외에 자바로 개발하는데 필요한 프로그램들이 설치된다. JDK 설치 후에는 설치된 디렉터리의 bin 디렉터리를 path에 추가해주어야 한다. 이 디렉터리에는 자바로 프로그램을 개발하는데 필요한 실행파일들이 들어있다. path는 OS가 파일의 위치를 파악하는데 사용하는 경로로, path에 디렉터리를 등록하면, 해당 디렉터리에 포함된 파일을 파일 경로없이 파일 이름만으로도 사용할 수 있게 된다.



### JDK의 bin 디렉터리에 있는 주요 실행 파일들

#### javac.exe

- 자바 컴파일러, 자바 소스 코드를 바이트코드로 컴파일한다.
- 바이트코드는 JVM이 이해할 수 있는 기계어, JVM은 바이트코드를 해당 OS의 기계어로 변환하여 OS에게 전달

#### java.exe

- 자바 인터프리터, 컴파일러가 생성한 바이트코드를 해석하고 실행한다.

#### javap.exe

- 역어셈블러, 컴파일된 클래스파일을 원래의 소스로 변환한다.

#### javadoc.exe

- 자동문서생성기, 소스파일에 있는 주석을 이용하여 Java API 문서와 같은 형식의 문서를 자동으로 생성한다.

#### jar.exe

- 압축프로그램, 클래스파일과 프로그램의 실행에 관련된 파일을 하나의 jar 파일로 압축하거나 압축해제한다.



### * JRE(Java Runtime Environment)

 자바실행환경으로 자바로 작성된 응용프로그램이 실행되기 위한 최소환경, JRE 안에는 라이브러리 파일들과 기타 파일, JVM을 가지고 있다. JDK는 JRE + 추가적인 개발 도구들이라고 생각하면 된다.



# 5. 자바로 프로그램 작성하기

 자바에서 모든 코드는 반드시 클래스 안에 존재해야 하며, 서로 관련된 코드들을 그룹으로 나누어 별도의 클래스를 구성하게 된다. 그리고 이 클래스들이 모여 하나의 자바 애플리케이션을 이룬다.



```
class 클래스 이름 {
	public static void main(String[] args) {
		
	}
}
```



 위의 main 메서드는 프로그램을 실행할 때 java.exe.에 의해 호출될 수 있도록 미리 약속된 부분으로 항상 똑같이 적어주어야 한다. 자바 애플리케이션은 main 메서드의 호출로 시작해서 마지막 문장까지 수행을 마치면 종료된다. 모든 클래스가 main 메서드를 가지고 있어야 하는 것은 아니지만 하나의 자바 애플리케이션에서는 main 메서드를 포함한 클래스가 반드시 하나는 있어야 한다.



# 6. 자바의 실행과정

 사용자가 자바 문법을 이용해 Hello.java 소스 파일을 만들었다고 하자 이를 실행하면 먼저 자바 컴파일러(javac.exe)를 이용해서 소스파일 .java로부터 클래스파일 .class을 생성한다. 그 다음에 자바 인터프리터(java.exe)로 실행한다.

 내부적인 진행순서는 아래와 같다.

1. 프로그램의 실행에 필요한 클래스(.class 파일)를 로드한다.
2. 클래스파일을 검사한다. (파일형식, 악성코드)
3. 지정된 클래스에서 main(String[] args)를 호출한다.



# 7. 주석(comment)

 작성하는 프로그램이 커질수록 이해하고 수정하기 어려워진다. 이러한 어려움을 덜기 위해 주석을 사용한다. 주석을 이용해서 코드에 대한 설명을 써놓으면 이해하는 데 많은 도움을 준다.

 컴파일러는 주석을 무시하고 건너뛰기 때문에 주석이 많다고 해서 프로그램의 성능이 떨어지는 일은 없다.



```
// 한줄 주석
/* comment */ 범위 주석 
```



