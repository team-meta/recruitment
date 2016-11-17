# MDS meta 2차 공채

## 분야
* ModPE 스크립트
* Blocklauncher 애드온
* PTP 모드
* Nukkit 플러그인

## 기간
2016.6.14 ~ 2016.07.31

## 지원자격
MDS 회원 (등급 상관없음)

## 문항 수
* ModPE 스크립트 : 객관식 10문제, 서술형 8문제
* Blocklauncher 애드온 : 객관식 10문제, 서술형 8문제
* PTP 모드 : 객관식 2문제, 서술형 3문제, 논술형 1문제
* Nukkit 플러그인 : 객관식 6문제, 서술형 4문제

**서술형과 논술형 문항은 부분점수가 있습니다.**

## 특혜
MDS VIP 등급 지급



# ModPE 스크립트
## 객관식 (50점)
> ModPE 스크립트 문항은 직접 코드를 실행시켜 답을 구할 수 있으므로, 채점자가 풀이과정을 요구할 수 있습니다.

### 1. Level.spawnMob 메서드로 새로운 엔티티를 스폰할 때, entityAddedHook 함수가 호출되는 시점을 고르시오. 4점

1. 호출되지 않는다.
2. 즉시 호출된다.
3. 10ms 뒤에 호출된다.
4. 100ms 뒤에 호출된다.
5. 보기에 존재하지 않는다.

### 2. 아래의 출력값을 구하시오. 6점
```javascript
let a = 1 && 2,
    c = function (a) {
        return (a > 3 ? Math.pow(a, 2) + 1 : 1);
    },
    b = typeof a !== "number" || (function (b, n) {
        return (function (l) {
            var k = l;
            for (var i = 0; i < n; i++) {
                k = c(k);
            }
            return k;
        })(b);
    })(a, 4);
print(b);
```
1. -16
2. -1
3. 0
4. 1
5. 16

### 3. 아래의 출력값을 구하시오. 5점
```javascript
var a, b, c;
a = b = c = true;
print(a != (b = !c) != (a = !b));
```
1. 0
2. null
3. true
4. false
5. undefined

### 4. 아래의 출력값이 4일 때, variable의 값이 될 수 있는 모든 값을 고르시오. 5점
```javascript
function a() {
  return arguments[variable];
}
a(5, 1, 2, 4);
```
1. 1
2. 2
3. 3
4. 4
5. "length"

### 5. 아래의 출력값을 구하시오. 5점
```javascript
print(Math.ceil(1 / Math.pow(10, 1000)));
```
1. -1
2. 0
3. 1
4. NaN
5. undefined

### 6. 아래의 출력값을 구하시오. 4점
```javascript
Level.setDifficulty(3);
var ent = Level.spawnMob(Player.getX(), Player.getY(), Player.getZ(), 32);
print(Entity.getTarget(ent));
```
1. null
2. ent
3. Player.getEntity()
4. 0
5. 83

### 7. 문법상 옳은 것을 모두 고르시오. 4점
1. var 1st;
2. var Blue;
3. var break;
4. var a = 'ddd";
5. var s = "string 'string'";

### 8. 아래의 출력값을 구하시오. 5점
```javascript
var a = 9;
a = a.toString(2);
print(a);
```
1. "001"
2. "1011"
3. "1001"
4. "1111"
5. "10101"

### 9. 아래의 출력값을 구하시오. 6점
```javascript
var a = 10;
function Obj(a){
  print(this.a);
}
print(Obj(15));
```
1. 10
2. 15
3. 12.5
4. NaN
5. undefined

### 10. 다음 중 true를 반환하는 것을 고르시오. 6점
1. `var str = /Javascript/;
str.test("javascript ModPE");`
2. ` var str = /Javascript/i;
str.test("javascript ModPE");`
3. `var str = /Javascript/s;
str.match("javascript ModPE);`
4. `var str = /Javascript/g;
str.match("Javascript ModPE);`
5. 보기에 존재하지 않는다.

## 서술형 (50점)

### 1. alert 함수가 몇회 실행되는지 구하시오. 4점
```javascript
var i = 0;
do {
    i += 2;
    alert("Alert!");
} while (i < 10);
```

### 2. 아래의 출력값을 구하시오. 5점
```javascript
var a, b;
a = b = 5;
print(a + b);
```

### 3. 아래의 출력값을 구하시오. 7점
```javascript
print(undefined = null || undefined == null && undefined === null);
```

### 4. 아래의 출력값을 구하시오. 7점
```javascript
var n = 1;
print(n--+-++n-++n);
```

### 5. 임의의 두 자연수 A, B 사이의 자연수 중 하나를 무작위로 구하는 코드를 작성하세요. 6점

### 6. 3차원 좌표에서 임의의 두 점 A(x1, y1, z1), B(x2, y2, z2) 사이의 거리를 구하는 코드를 작성하세요. 6점

### 7. 팩토리얼(k!)은 1부터 임의의 양의 정수 k까지의 모든 수를 곱하는 것을 말한다. 이때, 임의의 양의 정수 n에 대하여 n! 값을 구하는 코드를 작성하세요. 7점

### 8. 플레이어가 바라보는 방향에서 d 만큼 떨어진 점의 좌표를 구하는 코드를 작성하세요. (단, 좌표는 플레이어의 머리 좌표를 기준으로 하고 각 수식을 설명할 줄 알아야 한다) 8점



# Blocklauncher 애드온
## 객관식 (46점)

### 1. 애드온을 모바일에서 빌드하기 위한 툴을 고르시오. 4점
1. DroidEdit
2. 지퍼7 2.0
3. Web master
4. Aide
5. Aide Web

### 2. 애드온 제작 시 사용할 수 있는 언어를 모두 고르시오. 4점
1. C
2. C#
3. C++
4. Swift
5. Ruby

#### ※ 아래 문항은 모두 C++ 11을 표준으로 합니다.

### 3. 다음 중 int형 변수에 들어갈 수 없는 값을 고르시오. 4점
1. `1.1f`
2. `(int) 4.0`
3. `0x11`
4. `10`
5. `floor(2.3)`

### 4. 다음 중 배열을 올바르게 사용하지 않은 것을 고르시오. 4점
1. `a[0]`
2. `a[1] = 10`
3. `a[4] = 'A'`
4. `a[3] = 1`
5. `a[2.3] = 2`

### 5. 다음 중 C++의 자료형이 아닌 것을 고르시오. 4점
1. char
2. bool
3. float
4. int
5. String

### 6. 다음 중 마인크래프트에 존재하는 요소가 아닌 것으로 적절한 것을 고르시오. 5점
1. Block
2. BlockEntity
3. Player
4. MobEntity
5. LocalPlayer

### 7. 다음 중 문법에 어긋나는 것을 고르시오. 6점
1. `int a = 0;`
2. `Player& #~a^;`
3. `Player* player; player->setPos(0, 1, 0);`
4. `Entity* arrow; arrow.remove();`
5. `bool a = 0;`

### 8. 다음 중 반복문이 아닌 것을 고르시오. 4점
1. for
2. switch
3. do
4. while
5. 보기에 존재하지 않는다.

### 9. 다음 중 기본적으로 네임스페이스 std를 사용하도록 할 수 있는 구문을 고르시오. 5점
1. `using std;`
2. `namespace using std;`
3. `using namespace std;`
4. `#using std;`
5. `#define std;`

### 10. 다음 중 애드온 개발 시 필요한 최소한의 라이브러리를 모두 고르시오. 6점
1. libfmod.so
2. libminecraft.so
3. libgnustl_shared.so
4. libmcpelauncher.so
5. libmcpelauncher_tinysubstrate.so

## 서술형 (54점)

### 1. Player::attack(Entity&);를 후킹하여 어택훅을 작성한 후, 플레이어가 공격할 수 없도록 코딩하여 정상구동이 확인된 프로젝트를 첨부하시오. 7점

### 2. Mob *mob이라는 변수가 있다. 이 변수가 Player인지 아닌지 구하는 소스를 작성하시오. 6점

### 3. Entity 추가 시, 호출되는 함수를 한 가지만 적으시오. 6점

### 4. 아이템이 코드상으로 곡괭이인지 아닌지 구별하는 소스를 작성하시오. 5점

### 5. 메시지(채팅창)를 관리 패킷의 이름을 적으시요. 6점

### 6. 엔더진주는 코드상으로는 존재하지만 아직 소개되지 않고 있습니다. 엔더진주에 관한 물음에 답하시오.

#### 6-1. 엔더진주 아이템의 클래스명을 작성하시오. 4점

#### 6-2. 엔더진주 아이템을 활성화하고 크리에이티브 인벤토리에 추가하는 애드온을 만드시오. (include 구문 생략 후 작성) 6점

### 7. 땅이나 엔티티에 화살이 꽂히면 폭발하는 애드온을 만드시오. (include 구문 생략 후 작성) 6점

### 8. 금칙어가 들어간 채팅에서 금칙어만 "\*\*" 로 바꾸고 나머지는 그대로 채팅을 보내는 애드온을 만드시오. (단, 서버 원도 적용돼야 하며 문장 전체가 "\*\*" 로 바뀌어서는 안되고, 금칙어는 "블루덕", "레드스톤", "만동이" 이여야 한다) (include 구문 생략 후 작성) 8점



# PTP 모드
## 객관식 (17점)

### 1. 스티브는 열심히 자원을 모아 집으로 돌아가는 길이었다. 그런데 몬스터의 습격을 받아 아이템을 종종 빼앗겼고. 이런 스티브는 자신의 아이템을 보호하기 위해 인벤세이브모드를 만들기로 하였다. 다음 중 인벤세이브모드를 7047 값을 넣어 만들 때 가장 적절한 부분을 고르시오. 7점
1. Player::die
2. Player::dropAll
3. Inventory::setupDefault
4. Player::hurt
5. 보기에 존재하지 않는다.

### 2. 스티브는 자신의 세상에서 극도의 훈련 끝에 날아다니며 신과 필적하는 "크레이티브"라는 능력을 가지게 되었다. 주민이 이 모습을 보고 자신의 마을에 테러를 저지르는 스티브에게 벌을 내리고자 한번 죽으면 다시 살아나지 못하는 저주를 걸려고 할때. 필요한 것으로 올바르지 않은 것을 모두 고르시오. 10점
1. Player::dropAll
2. Player::respawn
3. Player::move
4. Player::attack
5. 보기에 존재하지 않는다.

## 서술형 (53점)

### 1. 스티브는 채팅을 입력할 때 누군가에게 공격받으면 채팅창이 닫히는 단점이 있다. 이 단점을 극복하려 할 때. MPE덤프 파일에서 가장 적절한 것을 고르고 어떤 수정값을 사용하여야 가장 간단하게 적용될지 아래 양식에 맞추어 쓰시오. 14점
> A: 양식 | [오프셋 / 수정값]

### 2. 다음 어셈블리 명령어를 분석할 때 최종적으로 마지막에 반환될 값을 구하시오. 17점
```assembly
movs r2 #1004
mov r0 r2
```

### 3. ARM 명령문 중 ldr과 str의 용도와 쓰임새를 100자 이내로 서술하시요. 22점

## 논술형 (30점)

### 1. 다음 사건을 해결하기 위한 최적의 방법을 자신의 생각을 300자 이내로 논술하시요. 30점
> 사건: 자신의 스피드를 빠르게 상승시키기 위해서 관련 오프셋을 수정하고자 할 때 다른 몬스터나 엔티티를 제외하고 오직 플레이어의 속도만 증가시키고자 할 때 무엇을 해야 할까?



# Nukkit 플러그인
## 객관식 (50점)

### 1. 다음 중 java.util.List 타입으로 현재 플레이어 목록을 뽑아오는 올바른 표현식을 고르시오. (단, server 변수는 cn.nukkit.Server의 인스턴스이고, 바깥에서 모든 Throwable을 캐치한다.) 7점
1.
```java
server.getOnlinePlayers();
```
2.
```java
server.getOnlinePlayers().keySet();
```
3.
```java
server.getOnlinePlayers().values();
```
4.
```java
(java.util.List) new java.util.ArrayList(server.getOnlinePlayers().values());
```
5.
```java
java.lang.reflect.Field playersField = cn.nukkit.Server.class.getDeclaredField("players");
playersField.setAccessible(true);
(java.util.List) new java.util.ArrayList(((java.util.Map) playersField.get(server)).values());
```

### 2. 아래에 클래스 선언문 두 개가 있다. 두 클래스의 차이점으로 올바른 것을 모두 고르시오. 7점
```java
final class ThreadA extends Thread implements cn.nukkit.InterruptibleThread {}
class ThreadB extends Thread {}
```
1. `ThreadA.class.getInterfaces().length`와 `ThreadB.class.getInterfaces().length`의 반환 값이 다르다.
2. ThreadA의 인스턴스는 인터럽트가 가능하지만 ThreadB는 불가능하다.
3. ThreadA의 인스턴스는 서버 종료 처리 과정에서 실행되고 있을 시에 자동으로 인터럽트 되지만, ThreadB는 그렇지 않다.
4. ThreadA는 `cn.nukkit.InterruptibleThread`의 추상 메소드를 구현하지 않았으므로 잘못된 클래스이다. 반면 ThreadB는 완전하다.
5. ThreadA는 상속이 불가능하다. ThreadB는 상속이 가능하다.

### 3. cn.nukkit.scheduler.Task와 cn.nukkit.scheduler.AsyncTask의 차이점으로 올바르지 않은 것을 고르시오. 7점
1. onRun 메소드의 매개변수 개수가 다르다.
2. `cn.nukkit.scheduler.AsyncTask`는 정적 멤버가 있지만 `cn.nukkit.scheduler.Task`는 그렇지 않다.
3. `cn.nukkit.scheduler.Task`의 인스턴스는 동기적으로 실행할지 비동기적으로 실행할지 자유롭게 선택할수 있지만, `cn.nukkit.scheduler.AsyncTask`의 인스턴스는 그렇지 않고 무조건 비동기적으로 실행할수 밖에 없다.
4. `cn.nukkit.scheduler.AsyncTask`를 직접 상속하는 Nukkit 클래스의 개수가 `cn.nukkit.scheduler.Task`보다 많다.
5. `cn.nukkit.scheduler.AsyncTask`는 setTaskId 메소드가 있지만 `cn.nukkit.scheduler.Task`는 없다.

### 4. 다음 중 Runnable을 구현(간접적 구현도 포함)하는 클래스가 아닌 것을 고르시오. 8점
1. `cn.nukkit.scheduler.PluginTask`
2. `cn.nukkit.plugin.certification.PluginCertificateTask`
3. `java.util.concurrent.FutureTask`
4. `cn.nukkit.level.format.anvil.ChunkRequestTask`
5. `java.util.TimerTask`

### 5. 항상 일정하게 y축 음의 방향으로 중력(9.8 kg * block / s ^ 2)을 받는 발사체를 진공 상태인 공간의 (0, 0, 0)에서 발사한다. 발사 초기 x축 양의 방향으로의 속도(block / s)가 a이고 y축 양의 방향으로의 속도(block / s)가 b, 그리고 발사체의 질량이 w(kg)일 때, 발사 시작시점 부터 그 발사체의 y좌표가 다시 0이 될 때까지의 x축 양의 방향으로의 변위(block)를 예측하는 표현식으로 알맞은 것을 고르시오. (단, block은 마인크래프트 한 블록 크기의 단위이며 a, b, w는 int형으로 주어진다) 9점
1. `2 * a * b / 9.8`
2. `2 * w * a * b / 9.8`
3. `a * b / 9.8`
4. `w * a * b / 9.8`
5. `√(a ^ 2 + b ^ 2) / 9.8`

### 6. 1 + 1 = 2; 라는 문장과 관련된 대화이다. 바르게 말한 것을 모두 고르시오. 12점
> ㄱ. 이 문장은 우변 식에 할당 연산자를 사용하였으니까 틀린 문장이야!

> ㄴ. 아니, 그건 좌변 식인데? 등호 좌변에 있으니 그건 좌변 식이야.

> ㄷ. 뭔 소리니? 좌변 식은 한번 사용 이후에도 수명이 있는 것들을 말해.
>  예를 들면,
>  int a = 1;
>  System.out.println(a);
>  System.out.println(a);
>  에서 a라는 것은 System.out.println 에서 사용 하고도 1이라는 값이 그대로 변함없이 있잖아. 그래서 두 번째 System.out.println에서도 쓸 수 있는 거야. 이때 a를 좌변 식이라로 불러. 그런데 1 + 1은 한번 사용 이후에 값이 바로 사라지니 우변 식이야.

> ㄹ. 맞아. 1 + 1 같은 것을 lvalue라고도 하지.

> ㅁ. 1 + 1은 rvalue 중에서도 prvalue이야.

1. ㄱ, ㄷ
2. ㄷ, ㅁ, ㅂ
3. ㄱ, ㄴ, ㄷ
4. ㄱ, ㄷ, ㅁ
5. ㄷ, ㄹ, ㅂ

## 서술형 (50점)
### 1. Integer.valueOf(156) == Integer.valueOf(156)는 false이지만, Integer.valueOf(37) == Integer.valueOf(37)은 true이다. (특정 실행 환경에서는 결과가 다를 수도 있지만, 일반적으로는 맞다) 그 이유를 서술하시오. 10점

### 2. "/back" 명령을 다음 조건에 맞게 구현하는 플러그인을 작성하시오. 12점
> ⅰ) 인자는 받아들이지 않는다. 인자가 있다면 사용자에게 경고 메시지를 보낸다.

> ⅱ) 명령 실행 시에 가장 최근의 TP 장소로 이동한다.
>   ex) 내가 광질하고 있다가 스폰으로 TP 했을 때 "/back"을 치면 아까 그 광질하던 장소로 돌아가야 한다.

> ⅲ) 이때, "/back" 명령을 쳐 이동하는 것은 TP로 인식하지 않는다.
>   ex) 내가 A 장소에 있다 치자. 이때 B 장소로 TP 했다. 또 한 번 더 C 장소로 TP 했다. 여기서 "/back"을 치면 B 장소로 이동할 것이다. 여기서 한 번 더 "/back"을 치면 C로 다시 이동하는 게 아니라 A로 이동해야 한다. 즉, "/back"을 쳐서 C에서 B로 이동하는 것을 텔레포트로 인식하면 안 된다.

> ⅳ) TP는 최대 10개까지 기억한다. TP 횟수가 10개 초과 시에 가장 오래된 TP는 기억에서 삭제한다.

### 3. cn.nukkit.event.EventPriority의 사용 방법과 용도를 서술하시오. 13점

### 4. Nukkit은 어느 JDK 버전에서 개발되었는지, 그리고 그것에 대한 타당한 근거를 제시하시오. (단, 근거는 Nukkit 개발에 사용된 Java 문법 관련 내용만 인정한다.) 15점
> ex) 다이아몬드 연산자가 사용되어서 JDK 7 이다. (인정)

> .travis.yml에 oraclejdk6이라고 적혀있어서 JDK 6이다. (인정 안 함)

> java.util.stream.IntStream 클래스가 사용되어서 JDK 8이다. (인정 안 함)