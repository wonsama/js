# 1. Lodash

## 1.1 학습 항목 : Array

* 원문 링크 : https://lodash.com/docs/4.17.10#chunk


# 2. 함수 종류 및 사용방법 

## 2.1 chunk

* `_.chunk(array, [size=1])`

> 입력받은 배열(array)를 size 기준으로 나눠준다
>
> 정확하게 딱 떨어지지 않는 경우는 나머지 만큼 나눠짐

예시)

```
_.chunk(['a', 'b', 'c', 'd'], 2);
// => [['a', 'b'], ['c', 'd']]
 
_.chunk(['a', 'b', 'c', 'd'], 3);
// => [['a', 'b', 'c'], ['d']]
```
## 2.2 compact

* `_.compact(array)`

> 배열 내부 값에서 `false, null, 0, "", undefined, NaN` 등의 false 에 해당하는 값을 제거한 이후 결과를 반환시켜준다

```
_.compact([0, 1, false, 2, '', 3]);
// => [1, 2, 3]
```
## 2.3 concat

* `_.concat(array, [values])`

> 배열또는 값을 연결시켜 새로운 배열을 생성시켜준다

```
var array = [1];
var other = _.concat(array, 2, [3], [[4]]);
 
console.log(other);
// => [1, 2, 3, [4]]
 
console.log(array);
// => [1]
```

## 2.4 difference

* `_.difference(array, [values])`

> 배열(array) 에서 포함하지 않은 값(values)을 제외한 나머지 값을 배열로(참조) 반환합니다. 결과 값의 순서와 참조는 첫 번째 배열에 의해 결정됩니다.
>
> 이와 달리 _.pullAll 은 기능은 동일하나, 결과 값을 신규 배열로(new array) 반환합니다. 

```
_.difference([2, 1], [2, 3]);
// => [1]
```

## 2.5 differenceBy

* `_.differenceBy(array, [values], [iteratee=_.identity])`

> 위 difference 와 기능은 동일하나, 내부 값 항목을 반복자(iteratee)에 매칭 후 해당 결과를 반환한다

```
_.differenceBy([2.1, 1.2], [2.3, 3.4], Math.floor);
// => [1.2]
 
// The `_.property` iteratee shorthand.
_.differenceBy([{ 'x': 2 }, { 'x': 1 }], [{ 'x': 1 }], 'x');
// => [{ 'x': 2 }]
```

