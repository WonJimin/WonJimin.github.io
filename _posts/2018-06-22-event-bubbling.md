---
category: javascript
title: jQuery::이벤트 캡쳐링/버블링 방지하기
author: 원지민
layout: post
---

<div class="code">
    <code>
        <p><span class="function">$</span>(<span class="script">selector</span>).<span class="function">eventMethod</span>(<span class="script">function</span>(<span class="variable">event</span>){ <span class="script">event</span>.<span class="function">stopPropagation</span>(); });</p>
    </code>
</div>

**event.stopPropagation();**를 사용하면 이벤트 캡쳐링과 버블링을 방지할 수 있다. (IE 하위버전은 작동하지 않는다.) <br>
**event.preventDefault();**와 사용되는 경우가 많은데, jQuery의 경우 구문이 끝나기 전 return false;를 해주면 <br> 
두 가지를 함께 적용하는 것으로 인식한다고 한다. 이 방법은 해당 selector로 인하여 <br>
이벤트 캡쳐링/버블링이 일어나는 구문에 사용해주면 된다. 