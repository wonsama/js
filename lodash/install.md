## 1 개요

> lodash 를 사용하면 배열, 개체, 문자열 반복 등의 조작, 테스트 및 복합 함수생성을  손쉽게 할 수 있습니다.
>
> 이러한 javascript 유틸리티인 lodash 를 손쉽게 사용하고자, [lodash 문서](https://lodash.com/docs/)를 번역+요약 한 내용을 공유합니다.


## 2 홈페이지 & 다운로드

> https://lodash.com/

## 3 설치

브라우져

* CDN 목록 : https://www.jsdelivr.com/package/npm/lodash

npm

* $ npm i --save lodash

## 4 사용하기

브라우져

```
<script src="lodash.js"></script>
```

nodejs

```
// Load the full build.
var _ = require('lodash');
// Load the core build.
var _ = require('lodash/core');
// Load the FP build for immutable auto-curried iteratee-first data-last methods.
var fp = require('lodash/fp');
 
// Load method categories.
var array = require('lodash/array');
var object = require('lodash/fp/object');
 
// Cherry-pick methods for smaller browserify/rollup/webpack bundles.
var at = require('lodash/at');
var curryN = require('lodash/fp/curryN');
```
