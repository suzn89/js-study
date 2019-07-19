## 01 자료형과 변수
- Boolean : True 와 False 두가지 값
- Null
- Undefined : 값을 할당하지 않은
- Number : 숫자
- String : 문자열
- Symbol : ES6에 추가, 변경 불가능한 기본값


## 02 연산자
**＋,-,＊,/,%**
(더하기,빼기,곱하기,나누기,나머지)

**=**
대입연산자

**+=, -=, ＊=, /= **

**＝＝, ＝＝＝**
2개는 느슨한 비교, 3개는 자료형까지 비교하는 엄격한 비교, 자스에서는 ＝＝＝를 사용해야함)

**＞,<,>=,<=**
크기비교 연산자

**&&, ||**
&& : 모두가 참일때 true, || : 하나라도 참이면 true

```js
function add (a, b) {
    return a + b  // returnm은 항상 받아줄 사람이 필요해
}

function add (a, b) {
    
  if(typeof a !== 'number' || typeof b !== 'number') {
      console.log('숫자만 써야대 ')
    return  // 함수 끝내기
  }
  if (a && b) {
   return a + b
  }
  console.log('인자값이 충분하지 않습니다.')
}

var result = add(10, 20)

console.log(result)
```

**++, --**
증감연산자는 위치에 따라서 동작하는 방식이 다르지만 사용을 지양하는 것이 좋다. +=1로 사용하는것이 직관적

**!**
true는 false로, false는 true로 변경

**!!**
배열,객체,문자,숫자 등을 불리언 값으로 변경

### False로 판단되는 값들
- undefined
- null
- 0
- NaN(Not a Number)
- "" (빈문자열)