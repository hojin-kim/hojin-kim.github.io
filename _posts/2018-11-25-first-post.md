---
title: first post
layout: post
categories: misc
tags: blogging
date: '2018-11-25 22:02:23'
---

github page 를 만들어 보려고 했는데 아는 게 없어서 엄청 헤맸다.
정리를 하려고 해도 너무 헤매느라 정리할 엄두도 안 나네...
[so-simple-theme](https://github.com/mmistakes/so-simple-theme) 을 사용했음. 결국은 하라고 하는 대로 하니까 됐다.

layout: post 이고 categories, tags 는 필드 이름이 복수형임

todos:
1. 카테고리랑 태그 모아놓고 어쩌고 하는 페이지 만들 수 있는지. (그리고 글에서 표시되는 카테고리/태그 이름 클릭하면 이동되어야 마땅할 카테고리/태그가 모여있는 페이지도요...)
2. MathJax 설정을 할 수 있는지?<br />
   -- (modified)  https://zishuaiz.github.io/blog/how-to-enable-mathjax-in-github-pages 를 참고했음! <br />
         --  (modified) 알고 보니 markdown 으로 사용하는 kramdown 이 mathjax 을 기본적으로 지원하는 것 같아서 kramdown을 통해서 적용하는 것으로 바꾸었음. 무엇이든 동일하게 동작하는 것 같다. 구체적으로는 _config.yml 파일을에서 markdown 이 kramdown 을 사용하는 지 확인하고 mathjax: true 를 추가해 주면 된다.

수식 표현에 대한 메모 코멘트를 남겨 놓는게 좋겠는데, 일단 달러 기호 한개로는 수식을 열지 못한다. 예를 들면 `$ \frac{\sin x}{x}\to 1 \text{ as } x \to 0 $` 는 $ \frac{\sin x}{x}\to 1 \text{ as } x \to 0 $ 로 보인다. 인라인 수식을 열기 위해서는 달러 두개를 쓰면 된다. 즉 `$$ \frac{\sin x}{x}\to 1 \text{ as } x \to 0 $$ `는 $$ \frac{\sin x}{x}\to 1 \text{ as } x \to 0 $$ 로 보인다. <br />
displaymath 모드를 위해서는 `\$\$ (수식 내용) \$\$ ` 처럼 하면 된다.(텍에서 수식 모드를 여는 규칙에서 `$` 를 `\$` 로 대체한 것인가 했는데, `\$(수식)\$` 는 동작하지 않는다. 열고 닫기 위해서 멀리 떨어져 있는 키들을 너무 많이 교대로 쳐야 하는 것 같은데, `\\[ (수식 내용) ]\\ ` 도 가능하다. \\[ \operatorname{Out}(G) = \operatorname{Aut}(G)/\operatorname{Inn}(G) \\] 예상하실 만한 대로 대괄호 대신 소괄호를 쓰면 그것도 인라인모드 수식이 된다. 그러나 `$$` 와 `\\[` 를 쓰기로 하면 인라인 모드와 디스플레이 모드 사이에 일관성이 없어서 마음에 들지 않는군...
