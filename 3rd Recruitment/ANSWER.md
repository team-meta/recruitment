# MDS meta 3차 공채 예시답안

## 주관식 (50점)

### 1. 주어진 배열의 중복된 원소를 제거하는 코드를 작성하시오. 단, 배열의 순서는 유지해야 한다.
```
입력예시: [false, "true", true, "ㄹ혜", "하야", true, 123, "하야"]
출력예시: [false, "true", true, "ㄹ혜", "하야", 123]
```
```javascript
/**
 * @author Astro
 */
function one(arr) {
    var tmp = [];
    for (var i = 0; i < arr.length; i++) {
        if (tmp.indexOf(arr[i]) < 0) {
            tmp.push(arr[i]);
        }
    }
    return tmp;
}
```

### 2. 주어진 2이상의 정수 A에 대해, A의 모든 양의 약수의 합을 구하는 코드를 작성하시오.
```
입력예시: 12
출력예시: 28
```

### 3. 두 자연수 A, B에 대해 최소공배수를 구하는 코드를 작성하시오.
```
입력예시: 12, 9
출력예시: 36
```

### 4. 두 자연수 A, B가 주어졌을 때, A이상 B이하인 피보나치 수의 개수를 구하는 코드를 작성하시오. 단, A < B이다.
```
입력예시: 3, 15
출력예시: 4
```

### 5. 소스코드에 탭(Tap)으로 들여쓰기 한 것과 공백(Space)로 들여쓰기 한 곳이 섞여있다. 주어진 문자열 `str`에 대해 들여쓰기로 사용된 탭(Tap)을 모두 공백문자(4 Space)로 바꾸는 코드를 작성하시오. 단, 들여쓰기는 각 줄에 첫 줄에서만 사용된다.
```javascript
/**
 * @author Astro
 */
function five(str) {
    return str.replace(/^\t{4}/gm, "    ");
}
```

### 6. 369 게임은 원으로 둘러앉아 순서대로 숫자를 부르며 3,6,9가 들어가는 숫자에 숫자 대신 박수를 치는 게임이다. 참가인원이 A명이고 B까지 숫자를 불렀을 때 3번째 사람은 몇 번 박수를 쳐야하는지 구하는 코드를 작성하시오. 단, A는 3이상의 정수, B는 A이상의 정수이다. (33과 같은 숫자가 나올 경우 박수는 한번만 친다)
```
예시입력: 5, 20
예시출력: 2
```
```javascript
/**
 * @author Rigel
 */
function six(a, b) {
    var x = 0;
    for (var i = 0; i < Math.floor(b / 10); i++) {
        for (var j = 0; j < Math.floor(b / a); j++) {
            if ((a * j + 3) - (10 * i + 3) == 0 || (a * j + 3) - (10 * i + 6) == 0 || (a * j + 3) - (10 * i + 9) == 0) {
                x++;
            }
        }
    }
    return x;
}
```

### 7. `democracy`을 출력하시오. 단, 아래의 5가지 기준을 모두 만족해야 합니다.
> 1. 코드 내에 `A,a,C,c,D,d,E,e,M,m,O,o,R,r,Y,y,\`가 없어야 합니다.

> 2. 외부의 파일이나 경로를 사용해서는 안됩니다.

> 3. 시간, 날짜 함수를 사용해서는 안됩니다.

> 4. 에러 번호 출력을 이용해서는 안됩니다.

> 5. 소스 파일의 크기는 150B(바이트)미만이여야 합니다.

```javascript
/**
 * @author ManDongI
 */
_ = [].push;
x = !0 + "";
b = x[1];
f = (_ + "")[3];
g = (_ + "")[6];
_[f + g + "nst" + b + "u" + f + "t" + g + b](b + x[3] + "tu" + b + "n p" + b + "int")()(37820888922418['t' + g + "St" + b + "ing"](36));
```

### 8. 수열 `a`의 일반항을 구하고, 함수화하시오.
> a는 다음과 같은 점화식을 가진다.

> a_1 = 0

> a_(n + 1) = (n + 1) * a_n - (-1) ^ n

```
입력예시: 10
출력예시: 1334961
```
```javascript
function factorial(m) {
    var num = 1;
    for (var i = 2; i <= m; i++) {
        num *= i;
    }
    return num;
}

function eight(n) {
    var sum = 0;
    for (var k = 0; k <= n; k++) {
        sum += Math.pow(-1, k) * factorial(n) / factorial(k);
    }
    return sum;
}

```