- [x] View the MarkDown Document
- [x] Install the Xcode and print "Hello World" with `Playground`
- [x] Make an account in Github and study MarkDown syntax
- [ ] [Answer below questions.](#questions)
  - [ ] [var 와 let의 차이점에 대해 서술하고 그 예제 코드 작성](#var-와-let의-차이점에-대해-서술하고-그-예제-코드-작성)
  - [ ] 반복문(Loop)의 종류와 1~10까지 출력하는 코드 작성
  - [ ] 타입 추론(Type Inference)이란?
  - [ ] 논리연산자(Boolean Logic) 인 AND(&&) 와 OR(||) 로 나올 수 있는 경우의 수 4가지


<br/>

## MarkDown Syntax

#### Styling Text
- **Bold**
- *Italic*
- ~~Strike Trhough~~
- **Bold and _nested italic_**
- ***All Bold and Italic***
- <sub>Subscript</sub>
- <sup>Superscript</sup>

#### Quotiong
> This is a quote text

This is a `quote code`
```
This is a quoue code too.
```
#### Link
This is a link to [Google](https://www.google.com/)

This [relative link](/sky.jpeg) goes to the sky image.

#### List
- This is a list
  - This is a nested list
1. This is a list in number

This is a footnote[^1].

[^1]: Footnote Sample.

## Questions

### var 와 let의 차이점에 대해 서술하고 그 예제 코드 작성

1. 중복선언 가능 여부 
  - var은 중복선언이 가능하지만, let은 불가능하다
``` javascript
// 첫번째 변수 선언+초기화
var sample = 10;
console.log(sample); // 10


// 두번째 변수 선언+초기화
var sample = 20;
console.log(sample); // 20


// 세번째 변수 선언(초기화X)
var sample;
console.log(sample); // 20
```

```javascript
// let 중복 선언
let sample2 = 100;
let sample2 = 200; // SyntaxError: Identifier 'sample2' has already been declared
```

2. 재할당 가능 여부
  - var과 let은 둘 다 재할당이 가능하다.
```javascript
var sample = 10;
sample = 20;
console.log(sample);  // 20

let sample2 = 100;
sample2 = 200;
console.log(sample2);  // 200
```

3. 지역변수 전역변수
  - var은 함수 내에서 선언했을 때에만 지역변수이며, 그 외에는 전역변수이다.
```javascript
if(true) {
    var sample = 10;
    console.log(sample); // 10
}


console.log(sample);  // 10
```
  - let은 코드 블럭 안에서 선언되면 언제나 지역변수이다.
```javascript
if(true) {
    let sample2 = 10;
    console.log(sample2); // 10
}

console.log(sample2);  // ReferenceError: sample2 is not defined
```

4. 호이스팅
  - var은 선언문 이전에 변수를 참조할 수 있다.
```javascript
console.log(sample); // undefined

var sample;
console.log(sample); // undefined

sample = 1; // 할당문에서 할당 단계 실행
console.log(sample); // 1
```
  - let은 선언문 이전에 변수를 참조하면 일시적 사각지대(Temporal Dead Zone; TDZ)에 빠지므로, 오류가 발생한다.
```javascript
console.log(sample2); // ReferenceError: foo is not defined

let sample2; // 변수 선언문에서 초기화 단계 실행
console.log(sample2); // undefined

sample2 = 1; // 할당문에서 할당 단계 실행
console.log(sample2); // 1
```

### 


<img src="https://user-images.githubusercontent.com/106911494/178134448-8a411889-3bee-4126-ab08-9a06dd1cf089.jpeg" width="200"/>


<!---
- 👋 Hi, I’m @Eunice0927
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

Eunice0927/Eunice0927 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.

--->
<!--![KakaoTalk_Photo_2022-07-10-15-50-31](https://user-images.githubusercontent.com/106911494/178134448-8a411889-3bee-4126-ab08-9a06dd1cf089.jpeg)-->
