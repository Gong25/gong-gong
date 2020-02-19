# 1.수행형 과제

## [주제1] : 생성자(Constructor)

### 내용 설명 및 요약
* 인스턴스를 생성 할 때 특정 파라미터를 입력할 수 있도록 강제하면, 실수를 줄일 수 있을 것이다.
이럴 때 생성자를 사용할 수 있다. 생성자는 인스턴스 변수의 초기화 작업에 주로 사용되며, 인스턴스 생성 시 
실행되어야 할 작업을 강제하기 위해서도 사용할 수 있다.
생성자를 사용하기 위해서는 클래스 안에 클래스와 똑같은 이름의 메서드를 만들어 주면 된다. 생성자가 없을 경우,
파라미터가 없는 기본 생성자가 생략되어 있다. 이 생성자 파라미터 안에 받아야 하는 값들을 넣어주면, 해당 인스턴스를
생성할때, 생성자 안에 있는 파라미터를 입력하도록 강제할 수 있다.
### 예제코드
```java
public class Dog {

	Dog(int leg , int tail ){
		System.out.printf("개의 다리는 %d개이고, 꼬리는 %d개 입니다", leg, tail);
	}
	
	
	
	public static void main (String[] args) {
		
		Dog dog = new Dog(4,1);
		
	}
	
	
	
}
```
### 코드에 대한 설명
* dog인스턴스를 생성할 때 파라미터를 입력하지 않으면 인스턴스가 생성되지 않는다. 생성자에서 지정한 2개의 정수를 
파라미터에 입력해주면, 해당 파라미터가 출력되도록 하는 코드이다. 예를들어 파라미터에 4,1를 입력하면
"개의 다리는 4개이고, 꼬리는 1개 입니다" 라는 문장이 출력된다.

## [주제2] : 오버로딩(overloading)

### 내용 설명 및 요약
* 한 클래스 내에서 같은 이름의 메서드를 여러 개 정의할 수 있는데, 이를 오버로딩이라고 한다.
오버로딩이 작동하기 위해서는 다음의 조건을 충족하여야 한다.
1.메서드의 이름이 같아야 한다.
2.파라미터가 달라야 한다.
오버로딩이 되어 있는 상태에서는, 해당하는 메소드가 실행되면, 파라미터가 같은 메소드를 찾아가야 실행된다.
만약 오버로딩기능이 없다면, 같은 기능을 하는 메소드의 모든 메소드명을 다르게 붙여야 할 것이다.
메소드의 숫자가 적으면 괜찮지만, 메소드의 숫자가 많아지면 일일이 다른 메소드명을 붙이는 것은 한계가 있으므로,
이를 해결하기 위해 오버로딩을 사용한다.
### 예제코드
```java
public class OverSum {

	int add (int a , int b) {
		
		int result = a + b;
		return result;
		
	}
	
	int add (int a, int b, int c) {
		
		int result = a + b + c;
		return result;
	}
	


	public static void main (String[] args) {
		
		OverSum sum = new OverSum();
		
		int result = sum.add(2, 3, 5);
		
		System.out.println(result);
		
		
		
		
	}
}
```
### 코드에 대한 설명
* sum 객체에 2개 또는 3개의 정수를 넣으면 그 정수들의 합을 출력해주는 코드이다.
정수 2개를 넣으면 2개를 계산하는 메소드가 실행되고, 3개를 넣으면 3개를 계산하는 메소드가 실행된다.

## [주제3] : 상속(inheritance)

### 내용 설명 및 요약
* 기존의 클래스를 새로 만들지 않고 재사용하는 것을 상속이라고 한다. 상속을 사용하면, 적은 양의 코드로 같은 기능을 하는 새로운 클래스를 
만들 수 있고, 코드의 변경이 용이한 장점이 있다.
상속받는 자손 클래스 뒤에 extexds Parent 를 붙여서 사용할 수 있고, 이 때 조상 클래스가 가지고 있는 모든 멤버가 자손 클래스에 상속이 된다.
생성자와 초기화 블럭은 상속되지 않는다.
### 예제코드
```java
public class Animal {

	int leg = 4;
	int tail = 1;
	
	
}

```
```java
public class Cat extends Animal {
	public static void main (String[] args) {
		
		Cat cat = new Cat();
		
		
		System.out.println(cat.leg);
		
		
		
	}
	
}

```
### 코드에 대한 설명
* Cat 클래스는 Animal이 가지고 있는 멤버변수를 모두 상속받았기 때문에, Cat클래스로 생성된 cat인스턴스는 leg를 따로 지정해 주지 않아도
4가 출력된다. Animal이 가지고 있는 int leg = 4;를 상속받았기 때문이다.
즉, 자손 클래스의 인스턴스를 생성하면 조상클래스의 멤버와 자손 클래스의 멤버가 합쳐진 하나의 인스턴스로 생성된다.
   
   
# 2. 실습형 과제

## [실습1]

### 실습코드
```java
import java.util.Scanner;

public class ES_3_1 {
	public static void main (String[] args) {
		Scanner scan = new Scanner(System.in);
		System.out.println("첫번째 좌표를 입력하세요");
		int a = scan.nextInt();
		int b = scan.nextInt();
		System.out.println("두번째 좌표를 입력하세요");
		int c = scan.nextInt();
		int d = scan.nextInt();
		
		int result = (c-a)*(d-b);
		
		if(result<0) {
			result = result * -1;
		}
		
		System.out.printf("넓이 : %d ",result);
		
	}
}

```
### 실행결과
```console
첫번째 좌표를 입력하세요
2
4
두번째 좌표를 입력하세요
4
2
넓이 : 4 
```

## [실습2]

### 실습코드
```java
import java.util.Scanner;

public class ES_4_5 {
	public static void main (String[] args) {
		Scanner scan = new Scanner(System.in);
		
		System.out.println("입력할 정수의 개수 : ");
		
		int a = scan.nextInt();
		int sum = 0;
		
		for (int i=0; i<a; i++) {
			System.out.printf("정수입력 : ");
			sum = scan.nextInt() + sum;
			
		}
		
		System.out.printf("평균 : %f",((double)sum/a));
		
		
		
	}
}

```
### 실행결과
```console
입력할 정수의 개수 : 
4
정수입력 : 2
정수입력 : 7
정수입력 : 2
정수입력 : 4
평균 : 3.750000
```

## [실습3]

### 실습코드
```java
import java.util.Scanner;

public class ES_1_2 {
	public static void main (String[] args) {
		
		Scanner scan = new Scanner(System.in);
		System.out.println("정수 세개를 입력하세요");
		int a = scan.nextInt();
		int b = scan.nextInt();
		int c = scan.nextInt();
		
		int result = a*b-c;
		
		System.out.printf("%d * %d - %d = %d",a,b,c,result);
		
		
	}
}

```
### 실행결과
```console
정수 세개를 입력하세요
1
2
3
1 * 2 - 3 = -1
```

## [실습4]

### 실습코드
```java
public class ES_5_4 {
	public static void main (String[] args) {
		
		for (int i=1; i<=9; i++) {
			for (int z=1; z<=9; z++) {
				if(i+z ==9) {
					System.out.printf(" %d\n+%d\n----\n 99\n\n",10*i+z,10*z+i);
				}
			}
		}
		
		
		
	}
}

```
### 실행결과
```console
 18
+81
----
 99

 27
+72
----
 99

 36
+63
----
 99

 45
+54
----
 99

 54
+45
----
 99

 63
+36
----
 99

 72
+27
----
 99

 81
+18
----
 99

```
