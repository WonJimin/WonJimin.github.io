---
category: javascript
title: JS/기초::프로토타입 체이닝
author: 원지민
layout: post
---

<pre>
    자바스크립트는 기존의 Class를 다루는 언어와는 다르게 프로토타입 기반의 언어이다.
    클래스가 없으므로 상속기능이 없지만 프로토타입을 기반으로 <strong class="bg_faf4c0">new 생성자를 이용해 상속을 흉내내는 방법</strong>이 있다.
    그것이  <strong class="bg_faf4c0">프로토타입 체이닝</strong>이다.

    <div class="image"><img src="https://t1.daumcdn.net/cfile/tistory/99431F4F5AC6D4A718"></div> 

    <b>*</b> 함수가 정의 될 때는 2가지 일이 일어난다.
    <div class="image"><img src="https://t1.daumcdn.net/cfile/tistory/99A2913D5AC7275710"></div> 
    <ol>
        <li>해상 함수에 Constructor(생성자) 자격 부여.</li>
        <li>해당 함수의 Prototype Object 생성 및 연결</li>
    </ol>
</pre>
<div class="provenance">
    [출처]
    <ul>
        <li><a href="https://medium.com/@bluesh55/javascript-prototype-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-f8e67c286b67" target="_blank">오승환::Javascript 프로토타입 이해하기</a></li>
        <li><a href="http://www.nextree.co.kr/p7323/" target="_blank">NEXTREE::JavaScript 프로토타입(prototype) 이해</a></li>
    </ul>
</div>

<!-- 발견한 사실<br>
_includes는 include해서 쓰는 파일<br>
_layouts은 layout을 이루는 skeleton 파일<br>
blog는 글목록 default는 모르겠네, home은 메인<br> 
page는 단일 페이지, post..도 page랑 비슷한데 잘모르겠다.<br>
<br>
_posts에 쓴 md는 _site로 build된다.<br>
2018-01-12는 년, 월, 일 순으로 dir생성되고<br>
-elements 부분은 제목이 된다.<br>
필요한건 title, author, layout<br>
<br>
_sass, assets은 그다지 중요하지 않다.<br>
<br>
_sections 폴더에 있는 글은 home에 노출된다.<br>
또한 파일 내 설정인 order로 정렬할 수 있다.<br>
파일명은 패럴랙스 시 앵커태그로 동작한다.<br> -->