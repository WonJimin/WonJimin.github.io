---
category: javascript
title: jQuery::동적 생성 태그에 이벤트 바인딩 하기
author: 원지민
layout: post
---

<div class="code">
    <code>
        <p><span class="function">$</span>(<span class="variable">selector</span>).<span class="function">eventMethod</span>(<span class="script">function</span>(){ <span class="annotation">/* 실행코드 */</span> });</p>
        <p><span class="function">$</span>(<span class="variable">selector</span>).<span class="function">on</span>(<span class="variable">event</span>, <span class="script">function</span>(){ <span class="annotation">/* 실행코드 */</span> });</p>
    </code>
</div>
위의 두 방식으로 연결 된 이벤트는 현재 존재하는 태그에만 연결된다. <br>
동적으로 생성된 태그에도 이벤트를 연결시키려면, <br>
<div class="code">
    <code>
        <span class="function">$</span>(<strong class="script">parentSelector</strong>).<span class="function">on</span>(<span class="variable">event</span>, <strong class="variable">selector</strong>, <span class="script">function</span>(){ <span class="annotation">/* 실행코드 */</span> });
    </code>
</div>
이런 식으로 작성해야 한다. 이런 식으로 연결 된 방식을 **delegate방식**(연결 범위를 한정하는 방법)이라고 한다.<br>
이 구문의 return 되는 this는 parentSelector이 아닌 selector이다.