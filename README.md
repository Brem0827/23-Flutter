[![Since](https://img.shields.io/badge/since-2023.11.13-333333.svg?style=flat-square)](https://github.com/Brem0827/23-Flutter)
[![author](https://img.shields.io/badge/author-Brem0827-0066FF.svg?style=flat-square)](https://github.com/Brem0827/23-Flutter)
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#23-Flutter)

[![Watch on GitHub](https://img.shields.io/github/watchers/Brem0827/23-Flutter.svg?style=social)](https://github.com/Brem0827/23-Flutter/watchers)
[![Star on GitHub](https://img.shields.io/github/stars/Brem0827/23-Flutter.svg?style=social)](https://github.com/Brem0827/23-Flutter/stargazers)
[![Fork on GitHub](https://img.shields.io/github/forks/Brem0827/23-Flutter.svg?style=social)](https://github.com/Brem0827/23-Flutter/network/members)

# 🏃Flutter

<table align="center">
    <tr>
        <td align="center">
	    <a href="https://github.com/Brem0827">
	    	<img src="https://avatars.githubusercontent.com/u/62270266?v=4?s=100" width="100px;" alt=""/>
				<br/>
					<sub>
					<b>이현종</b>
				<br/>
	    	<img src="https://us-central1-progress-markdown.cloudfunctions.net/progress/100"/>
	        </sub>
	    </a>
	</td>
    </tr>
</table>

💕 주차
---

1. 💭[1주차](#1주차)➡️
1. 💭[2주차](#2주차)➡️

---
# 2주차

🔋 2023.11.21 ~ 2023.11.27

# 7일차

<details><summary>💬 리스트 반복문 </summary>

- Dart에서는 다양한 반복문을 활용하여 리스트의 요소를 순회하고 처리할 수 있습니다.

- 주 반복문으로는 for-in 루프와 forEach() 메서드가 있습니다.

## 1차원 리스트 반복문

* for-in 루프

```dart

List<String> fruits = ['apple','banana','cherry'];

for(String fruit in fruits) {
	print(fruit);
}

```

* forEach()

```dart

List<String> fruits = ['apple','banana','cherry'];

fruits.forEach((fruits) {
	print(fruit);
});

```

## 2차원 리스트

- 2차원 리스트는 리스트 안에 또 다른 리스트를 요소로 갖는 리스트입니다.

- 각각의 내부 리스트는 행 이라고 생각할 수 있고, 전체 리스트는 행들을 모아놓은 표나 행렬 형태로 이해할 수 있습니다.

- 행과 열의 개념을 가진 데이터를 표현하고 처리할 수 있습니다.

```dart

List<List<int>> twoDimensionalList = [
	[1,2,3],
	[4,5,6]
];

```

## 다차원 리스트

- 2차원 이상의 차원을 가지는 리스트를 말합니다.

- 2차원 리스트는 행과 열로 이루어져 있지만, 다차원 리스트는 그 이상의 차원을 가질 수 있습니다.

- 다차원 리스트는 각 차원마다 해당하는 인덱스를 사용하여 요소에 접근할 수 있습니다.

</details>

<details><summary>💬 맵 </summary>

- Dart에서 맵은 키-값 쌍으로 이루어진 컬렉션 데이터 타입입니다.

- 각 키는 고유한 값으로 설정되어 있으며, 키와 연결된 값을 얻거나 설정할 수 있습니다.

```dart

Map<String, int> map1 = {'apple':1, 'banana':2, 'orange':3 };
Map<String, int> map2 = {};
Map<String, int> map3 = new Map();

```

```dart

var fruits = {'apple': {'color' : 'red', 'piece' : 1000}, 'banana' : {'color' : 'yellow', 'piece' : 500} };
print(fruits['apple', 'color']);
print(fruits['banana', 'price']);

```

</details>

<details><summary>💬 오류 </summary>

- 변수 미선언 에러 : 코드에서 salesRecords와 inventory 리스트가 초기화 되기 전에 사용되는 경우 변수 미선언 오류가 발생할 수 있습니다.

- 타입 불일치 에러 : selfFruit 함수와 매개변수 quantity는 정수타입으로 선언되었지만, 문자열이나 다른 타입의 값이 전달될 경우 타입 불일치 오류가 발생할 수 있습니다.

- null 안전성 에러 : 코드에서 salesRecords 리스트를 초기화 할 떄 빈 리스트로 선언하였기 때문에 null 체크를 하지 않아도 됩니다.

- checkinventory 함수에서 inventory 리스트가 null인지 확인 하지 않고 사용할 경우 null 참조 오류가 발생할 수도 있습니다.

- 인덱스 범위 초과 에러 : checkinventory 함수에서 inventory 리스트의 인덱스 범위를 초과하여 접근하는 경우 인덱스 범위 초과 오류가 발생합니다.

</details>

<details><summary>💬 예제 </summary>

- 조건문

```dart

int A = 10;
int B = 20;
int C = 30;

if ( A < B && A < C ) {
	print('A가 가장 작다.');
} else {
	print('A가 가장 작지 않다.');
}

if ( A < B ) {
	if(A < C) {
	print('A가 가장 작다.');
  }
	print('A가 가장 작지 않다.');
}

if ( A >= B ) {
	print('A가 B보다 크거나 같다.');
} else if ( A >= C ) {
	print('A가 C보다 크거나 같다.');
} else {
	print('A가 가장 작다.');
}

```

- 반복문

```dart

for( int i = 1 ; i <= 5 ; i++ ) {
	for( int j = 1 ; j <= i ; j++ ) {
		stdout.write('*');
	} 
	stdout.write(' ');
}

for( int i = 1 ; i <= 5 ; i++ ) {
	for( int j = 1 ; j <= i ; j++ ) {
		stdout.write('');
	} 
	for( int k = 1 ; k <= i ; j++ ) {
		stdout.write('*');
	} 
	stdout.write(' ');
}

for( int i = 5 ; i >= 1 ; i-- ) {
	for( int j = 1 ; j <= i ; j++ ) {
		stdout.write('*');
	} 
	stdout.write(' ');
}

for( int i = 5 ; i >= 1 ; i-- ) {
	for( int j = 5 ; j > 1 ; j-- ) {
		stdout.write('');
	} 
	for( int k = 1 ; k <= i ; j++ ) {
		stdout.write('*');
	} 
	stdout.write(' ');
}

for( int i = 1 ; i <= 9 ; i++ ) {
	if( i <= 5 ) {
		for( int j = 5 ; j > i ; j-- ) {
			stdout.write(' ');
		}
		for( int k = 1 ; k <= 2 * i ; k++ ) {
			stdout.write('*');
		}
		stdout.write('\n');
	} else {
		for( int j = 1 ; j <= i - 5 ; j++ ) {
			stdout.write(' ');
		}
		for( int k = 1 ; k <= 20 - 2 * i ; k++ ) {
			stdout.write('*');
		}
		stdout.write('\n');
	}
}

```

- switch 문

```dart

String sports = 'soccer';

switch (sports) {
	case 'soccer' :
		print('축구입니다.');
		break;
	case 'basketball' :
		print('농구입니다.');
		break;
	case 'baseball' :
		print('야구입니다.');
		break;
	case 'tennis' :
		print('테니스입니다.');
		break;
	default :
		print('기타 스포츠입니다.');
		break;
}

```

- 리스트

```dart

void main() {
	List<int> numbers = [10, 20, 30, 40, 50];
	int target = 30;
	bool found = false;
	int index;

	for ( int i = 0 ; i < numbers.length ; i++ ) {
		if ( numbers[i] == target ) {
			found = true;
			index = i;
			break;
		}
	}

	if(found) {
		print('원하는 값 $target은 리스트에 있습니다. 인덱스 : $index');
	} else {
		print('원하는 값 $target은 리스트에 없습니다.');
	}
}

```

</details>

<details><summary>💬 클래스 </summary>

- 클래스와 객체는 객체 지향 프로그래밍에서 핵심 개념 중 하나입니다.

- Dart에서 클래스는 객체를 만들기 위한 설계도 역할을 합니다.

- 객체는 클래스를 바탕으로 만들어진 것 입니다.

- 클래스는 속성과 메서드로 구성됩니다.

- 속성을 클래스의 상태를 나타내고, 메서드는 클래스가 수행할 수 있는 동작을 정의합니다.

- 클래스 선언은 class 키워드로 시작하며, 클래스명을 지정합니다.

- 중괄호 내에는 클래스의 속성, 생성자, 메서드 등을 선언합니다.

- 클래스 속성에는 대개 해당 클래스가 가지는 데이터를 저장하기 위한 변수들이 선언됩니다.

- 생성자는 객체를 초기화 하기 위해 사용되며, 클래스의 인스턴스를 만들기 위해 호출됩니다.

- 메서드는 클래스 안에서 정의된 함수로, 클래스가 가지는 동작을 수행 합니다.

```dart

class Person {
	String name = "kim";
	int age = 20;


	Person(String name, int age) {
		this.name = name;
		this.age = age;
	}

	void sayHello() {
		print("Hello, my name is $name and I'm $age years old");
	}
}

void main() {
	Person person = new Person("John", 18);
	person.sayHello();
}

```

</details>



---
# 1주차

🔋 2023.11.14 ~ 2023.11.20

## 6일차

<details><summary>💬 변수 코드 </summary>

```dart

import 'dart:io';

int selectedTable = 0;

void printMultiplicationTable(int start, int value) {
	for( var i = start ; i <= selectedTable ; i += value) {
		print('=== $i 단 ===');
		for( var j = 1 ; j <= 9 ; j++ ) {
			var result = i * j;
			print('$i x $j = $result');
		}
		print('----------------------');
	}
}

void printOptions() {
	print('1. 홀수단 출력');
	print('2. 짝수단 출력');
	print('3. 입력한 단까지 출력');
	print('4. 종료');
	print('원하는 작업 번호를 입력 하세요 : ');
}

void handleUserInput(int input) {
	if(input == 1) {
		selectedTable = 9;
		printMultiplicationTable(3,2);
	} else if(input == 2) {
		selectedTable = 8;
		printMultiplicationTable(2,2);
	}
	else if(input == 3) {
		print('출력할 단을 입력하세요 : ');
		selectedTable = int.parse(stdin.readLineSync()!);
		printMultiplicationTable(2,1);
	} else if(input == 4) {
		print('프로그램을 종료합니다.');
		exit(0);
	} else {
		print('잘못된 입력입니다. 다시 입력해 주세요');
	}
}

void main() {
	while(true) {
		printOptions();
		var input = int.parse(stdin.readLineSync()!);
		handleUserInput(input);
		print(' ');
	}
}

```

</details>

<details><summary>💬 리스트 </summary>

- Dart에서 가장 일반적으로 사용되는 데이터 구조 중 하나이자, 여러 개의 항목을 순서대로 저장하는 컬렉션입니다.

- 각 항목은 인덱스를 통해 접근할 수 있습니다.

- 동적으로 크기가 조정될 수 있으며, 같은 리스트에 서로 다른 데이터 유형의 항목을 포함할 수 있습니다.

</details>

<details><summary>💬 리스트의 생성 </summary>

- 리스트는 대괄호를 사용하여 생성하며, 각 항목은 쉼표로 구분합니다.

- 리스트의 각 항목은 값을 나타내며, 인덱스를 통해 개별 항목에 접근할 수 있습니다.

```dart

List<int> numbers = [1,2,3,4,5];
List<String> fruits = ['apple','banana','orange'];
List<dynamic> mixed = [1,'two',true];

```

</details>

<details><summary>💬 리스트의 길이 확인 </summary>

```dart

List<int> numbers = [1,2,3,4,5];
int length = numbers.length;
print(length);

```

</details>

<details><summary>💬 리스트의 요소 추가하기 </summary>

```dart

List<int> numbers = [1,2,3,4,5];
numbers.add(6);
numbers.add(7);

print(numbers);

```

</details>

<details><summary>💬 리스트의 요소 접근하기 </summary>

- Dart에서 리스트의 요소에 접근하는 방법은 인덱스를 사용하는 것 입니다.

- 리스트의 각 요소는 0 부터 시작하는 인덱스를 가지고 있으며, 해당 인덱스를 사용하여 요소에 접근할 수 있습니다.

```dart

List<int> numbers = [1,2,3,4,5];

int firstNumber = numbers[0];
print(firstNumber);

int thirdNumber = numbers[2];
print(thirdNumber);

```

</details>

<details><summary>💬 리스트의 요소 변경하기 </summary>

- Dart에서 리스트의 특정 위치에 있는 요소를 수정하려면 인덱스를 사용하여 접근하고 값을 할당하면 됩니다.

```dart

List<int> numbers = [1,2,3,4,5];

numbers[1] = 8;
print(numbers);

```

</details>

<details><summary>💬 리스트의 요소 제거하기 </summary>

- Dart에서 리스트의 특정 위치에 있는 요소를 제거하려면 remove() 메서드나 removeAt() 메서드를 사용할 수 있습니다.

```dart

List<int> numbers = [1,2,3,4,5];

numbers.remove(1);
numbers.removeAt(2);
print(numbers);

```

</details>

<details><summary>💬 리스트의 요소 복사하기 </summary>

- Dart에서 리스트를 복사하려면 List.from() 생성자를 사용하거나 toList() 메서드를 사용할 수 있습니다.

```dart

List<int> numbers = [1,2,3,4,5];
List<int> copiedNumbers = List.from(numbers);

List<int> numbers = [1,2,3,4,5];
List<int> copiedNumbers2 = List.toList();

```

</details>

<details><summary>💬 리스트의 요소 복사하기 </summary>

- Dart에서 리스트를 복사하려면 List.from() 생성자를 사용하거나 toList() 메서드를 사용할 수 있습니다.

```dart

List<int> numbers = [1,2,3,4,5];
List<int> copiedNumbers = List.from(numbers);

List<int> numbers = [1,2,3,4,5];
List<int> copiedNumbers2 = List.toList();

```

</details>

<details><summary>💬 리스트 합치기 </summary>

- Dart에서 리스트를 합치려면 + 연산자를 사용하거나 addAll() 메서드를 사용할 수 있습니다.

```dart

List<int> numbers = [1,2,3,4,5];
List<int> numbers2 = [6,7,8,9,10];
List<int> combinednumber = numbers + numbers2;

```

</details>

## 5일차 

<details><summary>💬 함수 </summary>

- 입력 값을 받아서 출력 값을 내놓는 일련의 과정을 수행하는 코드 블록을 말합니다.

- 특정한 기능을 수행하는 코드를 함수로 묶어서 필요할 때 마다 호출해서 사용할 수 있습니다.

- 코드의 재 사용성을 높여주고, 코드의 가독성과 유지보수성을 높여줍니다.

</details>

<details><summary>💬 지역변수 </summary>

- 함수나 코드 블록 내에서 선언된 변수로, 해당 함수나 코드 블록 내에서만 사용 가능 합니다.

- 다른 함수나 코드 블록에서는 사용할 수 없습니다.

- 이러한 특징을 변수의 유효범위라고도 합니다.

- 함수나 코드 블록이 종료되면 해당 변수는 소멸되며, 재 사용이 불가능합니다.

- 주로 함수 내에서 사용되며, 함수 내부에서 임시적으로 값을 저장하거나, 특정한 연산을 수행할 때 사용됩니다.

</details>

<details><summary>💬 전역변수 </summary>

- 프로그램 전체에서 접근 가능한 변수로서, 어느곳에서나 값을 읽거나 쓸수있다는 특징을 지니고있습니다.

- 프로그램 내에서 공유되어 사용되며, 프로그램이 종료될 때까지 유지됩니다.

- 함수 외부에서 선언되며, 함수 내부에서는 함수 인자를 포함하여 어떤 곳에서든지 참조할 수있습니다.

- 함수 내부에서 값을 변경하더라도 함수 호출이 종료된 후에도 그 값을 유지합니다.

</details>

<details><summary>💬 에러 </summary>

- 함수 호출 에러 : 존재하지 않는 함수를 호출하거나 함수의 이름을 잘못 입력하는 경우 함수 호출 오류가 발생할 수 있습니다. 함수 이름을 정확하게 입력하고, 호출하는 곳에서 함수의 인자와 반환값을 올바르게 처리해야 합니다.

- 무한 루프 에러 : 반복문이나 재귀 함수에서 탈출 조건을 정확하게 설정하지 않아 무한히 반복되는 루프가 발생할 수 있습니다. 이 경우 프로그램이 정지하지 않고 지속적으로 실행되므로 주의해야 합니다.

</details>

## 4일차 

<details><summary>💬 출력 </summary>

- Dart에서 표준 출력을 하기 위해서는 dart:io 라이브러리의 stdout 객체를 사용합니다.

- stdout.write()메서드를 사용하면 문자열을 출력할 수 있습니다. 

```dart

	stdout.write('Hello, world!');

```

</details>

<details><summary>💬 입력 </summary>

- Dart에서 표준 입력을 받기 위해서는 dart:io 라이브러리의 stdin 객체를 사용합니다.

- stdin.readLineSync() 메서드를 사용하면 사용자로부터 한 줄을 입력 받을수 있습니다.

```dart

	String name = stdin.readLineSync();

```

</details>

<details><summary>💬 조건문 </summary>

- 프로그램의 흐름을 제어하는 데 사용되는 구문입니다.

- 주어진 조건이 참일 경우에만 특정 코드 블록을 실행시키거나, 거짓일 경우에 다른 코드 블록을 실행시키는 등의 제어가 가능합니다.

</details>

<details><summary>💬 if문 </summary>

- 주어진 조건이 참인 경우에만 특정 코드 블록을 실행시키는 구문입니다.

```dart

if (조건식){
	// 조건식이 참일 때 실행할 코드
}

```

</details>

<details><summary>💬 switch문 </summary>

- 조건에 따라 다른 동작을 수행하는 제어문 입니다.

- 일반적으로 switch 문은 특정 변수의 값을 비교하고, 해당 값과 일치하는 경우에 해당하는 코드 블록을 실행합니다.

```dart

switch(변수) {
	case 값1 :
		// 값1과 일치하는 경우 실행할 코드
	break;
	case 값2 :
		// 값2와 일치하는 경우 실행할 코드
	break;
	case 값3 :
		// 값3과 일치하는 경우 실행할 코드
	break;
	default :
		// 모든 case에 해당하지 않는 경우 실행할 코드
	break;
}

```

</details>

<details><summary>💬 에러 </summary>

- 변수 초기화 에러 : selectedTable 변수가 초기화되지 않은 상태에서 사용되는 경우 변수 초기화 오류가 발생할 수 있습니다. selectedTable 변수는 초깃값을 설정 해야합니다.

- 반복문 조건 에러 : 반복문의 조건식을 잘못 작성하는 경우 반복문 조건 오류가 발생할 수 있습니다.

- 출력 형식 에러 : 출력문을 잘못 작성하거나, 변수나 문자열의 형식을 정확하게 지정하지 않는 경우 출력 형식 오류가 발생할 수 있습니다.

- 논리 에러 : 코드의 논리적인 흐름을 잘못 구성하는 경우 논리 에러가 발생할 수 있습니다.

- 기타적인 문법 에러 : 중괄호의 누락, 괄호의 불균형, 오타, 세미콜론의 누락 등과 같은 기본적인 문법 오류가 발생할 수 있습니다.

</details>

<details><summary>💬 반복문 </summary>

- 동일한 작업을 여러번 수행해야 할 때 사용되는 제어문 입니다.

- 일반적으로는 반복문은 조건식과 실행 블록으로 구성되며, 조건식이 참인 동안 실행 블록을 반복해서 실행합니다.

</details>

<details><summary>💬 for문 </summary>

- 지정된 횟수만큼 반복하는데 주로 사용됩니다.

```dart

for(초기화 ; 조건식 ; 증감식) {
	// 반복해서 실행할 코드
}

```

</details>

<details><summary>💬 while문 </summary>

- 조건식이 참인 동안 반복하는 데 주로 사용됩니다.

- 조건식이 거짓이면 반복문을 실행하지

```dart

while(조건식) {
	// 반복해서 실행할 코드
}

```

</details>

<details><summary>💬 do ~ while문 </summary>

- while문과 유사하지만, 반복문의 실행 블록을 먼저 실행한 다음에 조건식을 평가합니다.

- do~while문은 조건식이 거짓이더라도 실행 블록을 적어도 한 번은 실행 합니다.

```dart

do {
	// 반복해서 실행할 코드
}while(조건식);

```

</details>

<details><summary>💬 에러 </summary>

- 구문 오류 : 코드에서 세미콜론을 잘못 사용하거나 누락하는 경우, 구문 오류가 발생합니다.

- 세미콜론은 문장의 끝을 나타내는 구문 기호로 사용되며, 각 문장은 세미콜론으로 종료되어야 합니다.

- 변수 선언 오류 : 코드에서 변수에 잘못된 데이터 타입을 할당하거나 서로 다른 데이터 타입 간의 연산을 시도하는 경우 타입 불일치 오류가 발생

- 사용자 입력 에러 : 사용자가 숫자 대신 문자열을 입력하는 경우 int.tryParse()함수는 null을 반환하므로 number 변수는 null이 됩니다.

- 런타임 에러 : 입력된 문자열이 정수로 파싱될 수 없는 경우 int.tryParse()는 null을 반환합니다.

- 코드에서 null일 경우 -1을 할당했기 때문에 이 경우 에러는 발생하지 않습니다.

</details>

## 3일차

<details><summary>💬 Dart를 사용하는 이유 </summary>

- 클라이언트 측과 서버 측에서 모두 사용할 수 있기 때문에 플랫폼 간 개발이 가능합니다.

- 이러한 특징은 다양한 종류의 애플리케이션을 개발할 수 있는 기반이 됩니다.

- 주요 IDE와 텍스트 에디터에서 지원되며, 그중에서도 VSCode를 사용하면 편리하게 사용할 수 있습니다.

- Dart는 쉽게 배울수 있는 문법을 제공하며, 개발 생산성을 향상시키는 다양한 기능도 제공합니다.

- Dart 언어는 높은 생산성과 안정성을 제공합니다.

- 빠른 실행속도와 개발자 친화적인 기능을 모두 갖추고 있습니다.

- 자바스크립트를 대체할 수 있는 언어로 각광받고 있습니다.

</details>

<details><summary>💬 변수 </summary>

- 컴퓨터가 데이터를 사용하기 위해서 특정 값을 저장해두기위한 공간을 변수라고 합니다.

- 변수는 값을 저장하는 메모리 공간을 말합니다.

</details>

<details><summary>💬 자료형 </summary>

- 숫자형 데이터 타입 : int(정수형), double(실수형)

- 문자형 데이터 타입 : String

</details>

<details><summary>💬 특수문자 </summary>

- "\n" : 문자열 안에서 이 특수문자를 사용하면 새로운 줄로 이동하여 텍스트를 출력합니다.

- "\f" : 문자열 안에서 이 특수문자를 사용하면 수평 탭 간격만큼 공간을 띄웁니다.

- "\\" : 문자열 안에서 역슬래시 자체를 출력하고자 할 때 사용합니다.

- "$" : 문자열 안에서 이 특수문자를 사용하면 변수를 참조하여 변수의 값을 문자열에 포함시킬 수 있습니다.

- "\" : 문자열 안에서 따옴표를 포함하고자 할 때, 반드시 역슬래시 앞에 붙여주어야 합니다.

- 불리언 데이터 타입 : true, false 값으로 가지며, 초기 컴퓨터에서 이진법으로 연산을 하던 것이 현재에 이르러 불리언 타입으로 발전하여 다양하게 사용되고 있습니다.

- 'var' : 컴파일러가 변수의 타입을 추론하여 자동으로 할당 합니다.

</details>

<details><summary>💬 주석 </summary>

- 라인주석 : 라인주석은 `//` 기호를 사용하여 작성되며, 해당 라인에 대한 주석을 표시합니다.

- 주로 코드의 일부를 설명하거나 임시적으로코드를 비활성화하는 용도로 사용됩니다.

- 블록주석 : 블록주석은 `/* */`사이에 작성되며, 여러 줄에 걸친 주석을 표시하는 데 사용됩니다.

- 코드나 함수, 클래스 등에 대한 상세한 설명이나 문서화를 작성하는데 사용됩니다.

</details>

<details><summary>💬 연산자 </summary>

- 연산자는 하나 이상의 값을 가지고 연산을 수행하는 기호나 단어로, 프로그래밍에서 데이터를 처리하거나 비교할 때 사용되며 매우 중요한 역할을 합니다.

</details>

<details><summary>💬 산술 연산자 </summary>

- 숫자형 데이터의 덧셈, 뺄셈, 곱셈, 나눗셈 등 수학적 연산을 수행합니다.

- 덧셈은 + 연산자, 뺄셈은 - 연산자, 곱셈은 * 연산자, 나눗셈은 / 연산자를 사용합니다.

- 나머지는 % 연산자를 사용하여 반환할 수 있습니다.

</details>

<details><summary>💬 대입 연산자 </summary>

- 값을 변수에 할당하는 연산을 수행합니다.

- 연산자가 일반적으로 사용되며, 값을 할당하려는 변수 왼쪽에 위치하고 할당하려는 값을 오른쪽에 위치합니다.

</details>

<details><summary>💬 비교 연산자 </summary>

- 두 개의 값을 비교하고, 두 값이 서로 같은지 큰지 등의 결과를 반환

- 비교 연산자에서 반환되는 값을 데이터 타입에서 배웠던 불리언 타입이라고 할 수 있습니다.

- 동등 비교 연산자(==) : 두 개의 값이 서로 같은지를 비교합니다. 만일 같을경우 true를 반환하고, 다르면 false를 반환합니다.

- 부등 비교 연산자(!=) : 두 개의 값이 서로 다른지를 비교합니다. 만일 다르면 true를 반환하고, 같으면 false를 반환합니다.

- 대소 비교 연산자(<, >, <=, >=) : 두 개의 값을 대소 비교합니다. 작은지, 큰지, 작거나 같은지, 크거나 같은지를 비교하여 결과를 반환합니다.

</details>

<details><summary>💬 논리 연산자 </summary>

- &&(논리 곱) : 양쪽 피연산자가 모두 참일 경우에만 참을 반환합니다.

- ||(논리 합) : 양쪽 피연산자 중 하나 이상이 참일 경우 참을 반환합니다.

- !(논리 부정) : 피연산자가 참이면 거짓을, 거짓이면 참을 반환합니다.

</details>

<details><summary>💬 증감 연산자 </summary>

- 증감 연산자는 변수의 값을 증가시키거나 감소시킬 때 사용합니다.

- 변수를 하나씩 증가시키거나 감소시키는 경우에는 +=1, -=1 대신 ++, --을 사용하는 것이 더 간편하고 가독성이 좋습니다.

- 전위 증가, 감소 연산자는 코드를 실행하기 전에 값을 미리 증가, 감소시키고 코드를 실행합니다.

- 후위 증가, 감소 연산자는 코드를 실행하고 난 뒤에 값을 증가, 감소 시킵니다.

</details>

<details><summary>💬 삼항 연산자 </summary>

- 조건식에 따라서 다른 값을 반환하는 연산자입니다.

- `(조건식) ? 값1 : 값2`

- 조건식은 참 또는 거짓 값을 가지는 표현식이며, 값1은 조건식이 참일 경우 반환할 값이고, 값2는 조건식이 거짓일 경우 반환할 값입니다.

</details>

<details><summary>💬 제어문 </summary>

- 프로그램에서 실행 흐름을 제어하는 구문입니다.

- 주어진 조건에 따라서 다른 코드 블록을 실행하거나 실행을 중지하고 다른 코드로 이동 할 수 있도록 합니다.

- 조건문은 주어진 조건식의 참, 거짓 여부에 따라서 실행할 코드 블럭을 선택합니다.

- 제어문은 프로그램의 실행 흐름을 명확하게 제어할 수 있기 때문에, 프로그래밍에서 매우 중요한 역할을 합니다.

</details>

<details><summary>💬 입출력 </summary>

- 입력은 프로그램이 외부에서 데이터를 받아들이는 것 입니다.

- 출력은 프로그램이 처리한 결과를 외부로 보내는 것을 말합니다.

</details>

## 2일차

<details><summary>💬 Dart 언어란? </summary>

- Dart 언어는 구글이 개발한 객체 지향 프로그래밍 언어입니다.

- 자바스크립트와 같은 앱 프론트엔드 개발에서 사용되는 것이 일반적이지만, 서버 사이드 개발에서도 사용할 수 있습니다.

- Dart는 안정성, 확장성, 성능, 코드 가독성, 개발 생산성 등 다양한 측면에서 우수한 기능을 제공합니다.

- Dart는 C, C++, Java, JavaScript, Python 등 다양한 프로그래밍 언어에서 영감을 받아 탄생했습니다.

- 정적 타이핑과 동적 타이핑 모두 가능하며, 컴파일러를 통해 빠른 실행 속도를 제공합니다.

</details>

<details><summary>💬 정적 타이핑 </summary>

- 변수와 식의 타입을 컴파일 시점에 결정하고, 타입이 고정되어 있는 언어입니다.

- 프로그래머가 변수를 선언할 때 변수의 타입을 명시하거나, 컴파일러가 변수의 타입을 추론하여 결정합니다.

- 변수의 타입이 한번 결정되면 실행 중에 타입이 변경되지 않습니다.

- 컴파일러가 타입 체크를 수행하여 타입 관련 오류를 사전에 찾아내고, 코드의 안정성과 예측 가능성을 높일 수 있습니다.

</details>

<details><summary>💬 동적 타이핑 </summary>

- 실행 이전에 값이 확정되면 정적 바인딩이라고 합니다.

- 컴파일 타임에 호출될 함수가 결정되는 것으로, 함수는 기본적으로 정적 바인딩됩니다.

- 컴파일러는 선언되어있는 자료형을 보고 바인딩을 하기 때문에 실제로 가리키는 객체가 무엇이든 포인터의 자료형을 기반으로 호출의대상을 결정합니다.

- 빌드 중에 이루어집니다.  

</details>

<details><summary>💬 정적 바인딩 </summary>

- 실행 이후에 값이 확정되면 동적 바인딩이라고 합니다.

- 런타임에 호출될 함수가 결정되는 것으로, virtual 키워드를 통해 동적 바인딩하는 함수를 가상 함수라고 합니다.

- 함수가 가상 함수로 선언이 되면, 포인터 변수가 실제로 가리키는 객체에 따라 호출의 대상이 결정됩니다.

</details>

<details><summary>💬 동적 바인딩 </summary>

- 실행 이후에 값이 확정되면 동적 바인딩이라고 합니다.

- 런타임에 호출될 함수가 결정되는 것으로, virtual 키워드를 통해 동적 바인딩하는 함수를 가상 함수라고 합니다.

- 함수가 가상 함수로 선언이 되면, 포인터 변수가 실제로 가리키는 객체에 따라 호출의 대상이 결정됩니다.

</details>

<details><summary>💬 개발도구 </summary>

- 개발도구란 앱을 개발하는 데 사용되는 모든 소프트웨어를 말합니다.

- 앱 개발에 필요한 여러 개발 도구는 다음과 같습니다.

* 통합 개발 환경(IDE) : 코드 작성, 디버깅, 프로젝트 관리 등 개발 전반적인 작업을 수행하는 도구

* 코드 에디터 : 코드 작성을 위한 간단한 텍스트 에디터

* 시뮬레이터 또는 에뮬레이터 : 앱을 실행하고 테스트 할 수 있는 가상 환경

* 개발자 도구 : 앱의 성능을 분석하고 디버깅 할 수 있는 도구

</details>

<details><summary>💬 에디터 설정 </summary>

- 설치한 개발 도구를 플러터 개발에 적합하게 설정 해야 합니다.

- 이 설정에는 플러터 및 Dart 플러그인 설치, 에디터 확장기능 설치, SDK 경로 설정 등이 포함될 수 있습니다.

- 이를 통해 개발 도구가 플러터 애플리케이션 개발을 지원하고 필요한 도구와 기능을 제공할 수 있게 됩니다.

</details>

<details><summary>💬 프로젝트 생성 </summary>

- 플러터 개발을 시작하려면 새로운 플러터 프로젝트를 생성해야 합니다.

- 프로젝트 생성은 명령행 도구인 Flutter CLI를 사용하거나 개발 도구의 GUI를 통해 수행할 수 있습니다.

- 프로젝트 생성시에는 프로젝트 이름, 패키지 이름, 플랫폼 설정 등의 정보를 입력하고, 프로젝트 디렉토리가 생성되며 초기 플러터 코드와 구조가 구성됩니다.

</details>

## 1일차

<details><summary>💬 플러터란? </summary>

- 플러터(Flutter)는 구글에서 개발한 모바일앱 SDK로, 안드로이드와 iOS 모두에서 작동하는 하이브리드 앱 개발 도구 입니다.

- 플러터는 Dart 언어를 사용하여 개발됩니다.

- 플러터는 위젯을 기반으로 UI를 구성하는데, 위젯은 특정 플랫폼에 종속되지 않기 때문에 안드로이드와 iOS 모두에서 같은 디자인을 사용할 수 있습니다.

- 높은 생산성과 일관된 UI를 가진 것이 특징 입니다.

</details>

<details><summary>💬 SDK </summary>

- Software Development Kit의 약자로 안드로이드 앱을 개발하기 위한 도구 모음입니다.

</details>

<details><summary>💬 플러터의 특징 </summary>

* 크로스 플랫폼 개발 - 플러터는 하나의 코드베이스로 iOS와 Android 모두에서 동작하는 앱을 개발 할 수 있습니다.

* UI - 플러터는 Material Design과 Cupertino Design을 지원하며, 이를 이용하여 편리하게 보기 좋은 UI를 구현할 수 있습니다.

* 생산성 - 플러터는 Hot Reload 기능을 지원하여 코드를 수정할 때마다 앱을 즉시 새로 고침하여 수정 결과를 확인할 수 있습니다. 이로 인해 개발 생산성이 높아집니다.

* 성능 - 플러터는 모바일 앱의 성능을 최적화 하기 위해 C/C++ 엔진인 Skia를 사용합니다. 또한, 네이티브 컴포넌트에 접근하여 더욱 빠른 성능을 제공합니다.

* 위젯 - 플러터는 다양한 위젯을 제공하며, 이를 조합하여 여러 디자인을 구현할 수 있습니다.

* 상태 관리 - 플러터는 상태 관리를 위해 Provider, BLoC 등의 패턴을 지원하며, 이를 이용하여 복잡한 앱의 상태를 효과적으로 관리할 수 있습니다.

* 배포 - 플러터는 Google Play Store, Apple App Store 등의 앱 스토어에 쉽게 배포할 수 있습니다.

</details>

<details><summary>💬 UI </summary>

- User Interface 사용자 인터페이스의 약자로 우리가 볼 수 있는 화면 내에 그림이나 디자인 등의 모든 것을 이야기합니다.

</details>

<details><summary>💬 네이티브 컴포넌트 </summary>

- 모바일 플랫폼(Android 또는 iOS)에서 제공하는 기본적인 UI 요소를 말합니다.

- 각 플랫폼에서 제공되는 네이티브 컴포넌트는 해당 플랫폼의 UI 디자인 가이드라인을 따르며, 사용자 인터페이스를 구성하는 데 사용됩니다.

</details>

<details><summary>💬 플러터의 장단점 </summary>

* 장점

- 하나의 코드로 iOS와 ANdroid 모두 지원할 수 있어 크로스 플랫폼 개발이 용이합니다.

- 다양한 위젯과 레이아웃을 제공해 UI 구현이 간편합니다.

- 플러터는 내장된 빠른 사이클을 가지고 있어서, 소프트웨어를 빠르게 개발하고 배포할 수 있습니다.

- 다양한 개발 도구와 호환되며, 디버깅이 쉽습니다.

- 모바일 애플리케이션 개발에 있어 좋은 성능을 보여줍니다.

* 단점

- 크로스 플랫폼의 특성상, 특정 플랫폼에 최적화된 애니메이션 및 UI 요소는 구현하기 어렵습니다.

- 플러터 앱의 크기가 다른 프레임워크에 비해 상대적으로 큽니다.

</details>

<details><summary>💬 디버깅 </summary>

- 컴퓨터 프로그램의 오류를 찾아 수정하는 과정을 말합니다.

</details>
