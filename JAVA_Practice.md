# JAVA_Practice
# JAVA

### type
```java
package test2;

public class type {

    public static void main(String[] args) {

        char car = 'D' - 3;

        char car1 = 'A';
        char car2 = 'B';
        char car3 = 'C';
        System.out.println(car1);
        System.out.println(car2);
        System.out.println(car3);
        char[] car = { 'A', 'B', 'C' };

//        car[0]
//        car[1]
//        car[2]
        for (int i = 0; i < car.length; i++) {
            System.out.println(car[i]);
        }

        System.out.println(car.length);
        char[] carr = new char[] { 'A', 'b', 'c' };
        System.out.println(ca);
        System.out.println(car);
        car[0] = 'F';
        System.out.println(car);


        System.out.println(carr);
        carr = new char[] { 'B', 'F', 'G', 'Y' }; 
        System.out.println(carr);

        int as = 0;
        int[] a = { 1, 2, 3 };
        int[] an = new int[] { 1, 2, 3 };

        long lo = 1L;
        float fo = 1.0f;
        double dou = 1.0001;

        char[] c = new char[3];
        String[] s = new String[3];
        long[] l = new long[3];

        char[][] c2 = new char[3][3];

    }
}
```

### PrintTest
```java

public class PrintTest {

    public static void main(String[] args) {

//        서식없는 출력(print() : 출력 후 줄을 바꾸지 않는다, println() : 출력 후 줄을 바꾼다.
        System.out.print("Hi \nJAVA");
        System.out.println(); // 아무것도 출력하지 않고 줄을 바꾼다. 한 줄 바꾸
        System.out.println("HI JAVA");

//    "+" 연산자는 "+" 연산자의 양쪽에 모두 숫자가 나올 경우 덧셈을 하고 한쪽이라도 문자열이 나오면 문자열을 연결하는 연결 연산자로 사용된다.
        System.out.println("5 + 3 = " + (5 + 3));
        System.out.println("5 - 3 = " + (5 - 3));
        System.out.println("5 * 3 = " + (5 * 3));
        System.out.println("5 / 3 = " + (5 / 3)); // 정수와 정수의 연산은결과도 정수다. 묵시적 형변환
        System.out.println("5 % 3 = " + (5 % 3)); // 나머지

//    묵시적 형변환 : 자료형의 크기가 서로 다른 자료의 연산 결과는 크기가 큰 자료형으로 자동 변환된다.
//    자바의 기본 자료형
//    boolean : 1바이트(8비트), true 또는 false를 기억한다.
//    char : 2바이트, 1문자를 기억한다.
//  short : 2바이트, -32768 ~ 32767 사이의 정수를 기억한다.
//    int : 4바이트, -2147483648 ~2147483647 사이의 정수를 기억한다.
//    long : 8바이트, -2의 63제곱 ~ 2의 63제곱 -1 사이의 정수를 기억한다.
//    float : 4바이트, 단정도 실수, 소수점 아래로 6자리 정도를 표현한다.
//    double : 8바이트, 배정도 실수, 소수점 아래로 16자리 정도를 표현한다. float 보다 더 정밀한 연산이 가능하다.

        System.out.println("5 /3. = " + 5 / 3.);
        System.out.println("5. / 3 = " + 5. / 3);
        System.out.println("A + 32 = " + ('A' + 32));
        System.out.println("a - 32 = " + ('a' - 32));

//  서식 있는 출력(printf() ==> c언어의 printf 사용법과 같다.
//    printf("출력서식", 출력할 내용);
//    출력 서식은 출력 서식 문자를 제외한 나머지 문자는 입력한 그대로 출력된다.
//    출력 서식문자 : d(정수), f(실수), c(문자), s(문자열)
//        출력 서식의 형식 : %[-][0][n][.m]서식문
//        - : 출력할 전체 자리수가 지정된 경우 왼쪽에 맞춰 출력한다.
//        0 : 출력한 전체 자리수가 지정된 경우 왼쪽의 남는 자리에 0을 채워 출력한다.
//        n : 출력할 전체 자리수
//        .m : 소수점 아래 자리수, 잘리는 자리에서 반올림 시켜 출력한다. 원래 데이터 값은 변경되지 않는다.

        System.out.printf("5 + 3 = %d\n", 5 + 3);
        System.out.printf("%d + %d = %d\n", 5 , 5 + 3);
        System.out.printf("5 / 3. = %f\n" , 5 / 3.);

    }
}
```

### ScannerTest01
```java
import java.util.Scanner;

public class Scanner01 {
    public static void main(String[] args) {

//        키보드를 통해서 데이터를 입력받는 스캐너
        Scanner sc = new Scanner(System.in);
        
//        next() : 문자열을 력받는다. 띄어쓰기 전까지 입력받는다.
//        nextLine() : 문자열을 입력받는다. 한 줄 전체를 입력받는다.
//        nextLine() 메소드는 키보드 버퍼가 비어있을 경우 입역을 요구하며 대기하고 키보드 버퍼가 비어있지 않으면 
//        키보드 버퍼 전체의 내용을 읽어들인다.
        
        String addr = "";
        System.out.print("주소를 입력하세요 : ");
        addr = sc.nextLine();
        String name = "";
        System.out.println("이름을 입력하세요 : ");
        name = sc.nextLine();
        
        System.out.println(name + "님은" + addr + "에 삽니다.");
        
        sc.close();
    }
}

```

### ScannerTest02
```java
import java.util.Scanner;

public class Scanner02 {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int age = 0;
        System.out.print("나이를 입력하세요 : ");
        age = sc.nextInt();

//        문자열을 제외한 데이터를 입력받은 후 nextLine() 메소드가 실행이 되야 한다면 
//        키보드 버퍼의 엔터키를 읽어들이는 문제가 발생된다.
//        문자열을 제외한 데이터를 입력받은 후 키보드 버퍼를 비워주는 동작을 실행하고 nextLine() 메소드를 실행한다.

        String name = "";
        System.out.println("이름을 입력하세요 : ");
        name = sc.nextLine();

        System.out.println(name + "님은" + age + "살 입니다.");

        sc.close();

    }
}
```

### StringTest01
```java

public class StringTest01 {
    public static void main(String[] args) {

//        클래스로 만드는 모든 객체(변수)는 주소를 기억하는 참조형 변수이다.
//        문자열이 최초로 만들어지면 메모리 어딘가에 문자열이 생성된 메모리의 주소가 저장된다.

        String str1 = "AAA"; // str1에는 "AAA"가 생성된 메모리의 주소가 저장된다.
//                메모리에 같은 내용의 문자열이 있으면 다시 만들지 않고 기존에 있는 문자열의 주소값이 변수에 저장된다.
        String str2 = "AAA"; // str2에는 str1에 저장된 "AAA"가 생성된 메모리의 주소가 저장된다.

//        관계 연산자 : 연산 결과는 true(참), false(거짓) 둘 중의 하나이다.
//        >(크다, 초과), >=(크거나 같다, 이상), <(작다, 미만), <=(작거나 같다, 이하), ==(같다), !=(같지 않다)
//        "=="를 사용해서 같은가 비교할 수 있는 데이터는 기본 자료형과 NULL(아무것도 없는 상태)만 가능하다.

//        논리 연사자
//        && : 논리곱, AND, 두 조건이 모두 참일 경우에만 참, ~이고, ~이면서, ~중에서
//        || : 논리합, OR, 두 조건 중에서 한 개 이상 참일 경우에 참, ~또는, ~이거나
//        ! : 논리부정, NOT

//        if(조건식) {
//            조건식이 참일 경우 실행할 문장;
//            ...;
//        }    else {
//            조건식이 거짓일 경우 실행할 문장;
//            ...
//        }

//        "=="을 사용해서 비교했으므로 변수에 저장된 문자열 자체를 비교한게 아니고 변수에 저장된 주소를 비교하게 된다.
        if (str1 == str2) {
            System.out.println("같다");
        } else {
            System.out.println("다르디");
        }

//        new라는 예약어를 사용해서 객체를 생성하게되면 메모리에 같은 내용이 있나 상관하지 않고 무조건 다시 만든다.
        String str3 = new String("AAA");

//        문자열을 비교하려 하는 경우 반드시 equals() 메소드를 사용해서 비교해야 한다. 
        if (str1.equals(str3)) {
            System.out.println("같다");
        } else {
            System.out.println("다르다");

        }

    }
}

```

### StringTest02
```java
import java.util.Scanner;

public class StringTest02 {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("문자열을 입력하세요 : ");
        String str = sc.nextLine();

//        lenth() : 변수에 저장된 문자열을 구성하는 문자의 갯수를 얻어온다.
        System.out.println("입력한 문자열의 크기 : " + str.length());

//        trim() : 문자열 앞, 뒤의 불필요한 공백을 제거한다.
        System.out.println("입력한 문자열에서 불필요한 공백을 제거한 문자열의 크기 : " + str.trim().length());

//        toUpperCase() : 영문자를 무조건 대문자로 변환한다.
        System.out.println("무조건 대문자로 출력 : " + str.toUpperCase());
//        toLowerCase() : 영문자를 무조건 문자로 변환한다.
        System.out.println("무조건 소문자로 출력 : " + str.toLowerCase());

//        chatAt(index) : 문자열에서 index번째 문자 1문자를 얻어온다. 문자의 위치를 계산할 때 맨 앞의 문자 index가 0부터 시작된다.
        System.out.println("3번째 문자 : " + str.charAt(2));

        sc.close();
    }
}

```

### IfTest01
```java
import java.util.Scanner;

public class IfTest {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("3과목 점수를 입력하세요 : ");
        int java = sc.nextInt();
        int jsp = sc.nextInt();
        int spring = sc.nextInt();

        int total = java + jsp + spring;
        double average = (double) total / 3; // total 이 double 타입을 받을 수 있게 캐스팅.

        System.out.println("평균 점수 : " + average);
        System.out.printf("평균 점수 : %6.2f\n", average);

        if (average >= 90) {
            System.out.println("수");
        } else if (average > 80) {
            System.out.println("우");
        } else if (average > 70) {
            System.out.println("미");
        } else if (average > 60) {
            System.out.println("양");
        } else { // (average < 60)를 할 필요가 없어요.
            System.out.println();
        }
//        if (average >= 90) {
//        System.out.println("수");
//         }
//         if (average < 90 && average >= 80) {
//        System.out.println("우");
//        }        
//        if (average < 80 && average >= 70) {
//        System.out.println("미");
//         }
//        if (average < 70 && average >= 60) {
//        System.out.println("양");
//         }
//        if (average < 60)  {
//        System.out.println("가");
//         }                                  --> 이게 아니에요.

    }
}
```

### IfTest02
```java
import java.util.Scanner;

public class IfTest02 {
	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);

		System.out.print("윤년/평년을 판별할 년도를 입력하세요 : ");

		int year = sc.nextInt();

//		프로그램에서 여러번 사용되는 값은 변수에 저장시켜 사용하면 편리하다.
//		논리값을 기억하는 변수나 논리값을 리턴하는 메소드의 이름은 "is"로 시작하는 것이 관례이다.

		boolean isLeapYear = year % 4 == 0 && year % 100 != 0 || year % 400 == 0;

//		년도가 4로 나눠 떨어지고(&&) 100으로 나눠 떨어지지 않거나(||) 400으로 나눠 떨어지면 윤년, 그렇지 않으면 평년이다.

		if (isLeapYear) {
			System.out.println(year + "년은 윤년입니다.");
		} else {
			System.out.println(year + "년은 평년입니다.");
		}
		
//		삼항 연산자(?:)
//		if의 조건을 비교한 결과 조건이 참일 때와 거짓일 때 실행할 문장이 1문장인 경우 사용하면 편리하다.
//		조건식 ? 조건식이 참일 경우 실행할 내용 : 조건식이 거짓일 경우 실행할 내용
		
		System.out.println(year + "년은" + (isLeapYear ? "윤" : "평") +"년입니다.");
		
		sc.close();

	}
}
```

### SwitchTest
```java
import java.util.Scanner;

public class SwitchTest {

	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);
		
		System.out.print("3과목 점수를 입력하세요 : ");
		int java = sc.nextInt();
		int jsp = sc.nextInt();
		int spring = sc.nextInt();

		int total = java + jsp + spring;
		double average = (double) total/3;
		
		System.out.println("평균 점수 : " + average);
		System.out.printf("평균 점수 : %6.2f\n", average);
		
//		key 값은 정수를 기억하는 변수 또는 연산 결과가 정수인 수식, 자바 1.7 부터는 문자열도 가능하다.
//		switch (key) {
//			case value:         //":"임을 주의한다.
//				key와 value가 일치할 경우 실행할 문장;
//				...;
//				[break;]        //if문을 제외한 나머지 제어문의 {}블록을 탈출한다.
//				...;
//			[default:
//				key와 일치하는 value가 없을 경우 실행할 문장;
//				...;
//				break;]
//		}
		
		switch ((int) average / 10) {
			case 10:
				System.out.println("참 잘했어요!");
				System.out.println("수"); break;  //조건을 만족 했으면 아래는 할 필요가 없어서 탈출.
			case 9:
				System.out.println("우"); break;   
			case 8:
				System.out.println("미"); break;
			case 7:
				System.out.println("양"); break;
//				같은 작업을 하는 case는 나열할 수 있다.
//				case 5: case 4: case 3: case 2: case 1: case 0:
			default:
				System.out.println("가"); break;
		}
	}
}
```

