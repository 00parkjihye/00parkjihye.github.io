---


---

<h1 id="python">Python</h1>
<p><img src="https://www.python.org/static/community_logos/python-logo-master-v3-TM-flattened.png" alt="python logo"></p>
<h4 id="python-page파이썬-공식-홈페이지-httpswww.python.org">Python Page(파이썬 공식 홈페이지): <a href="https://www.python.org/">https://www.python.org/</a></h4>
<h4 id="pep-8---style-guide-for-python-code-파이썬-공식-스타일가이드-httpswww.python.orgdevpepspep-0008">PEP 8 - Style Guide for Python Code (파이썬 공식 스타일가이드): <a href="https://www.python.org/dev/peps/pep-0008/">https://www.python.org/dev/peps/pep-0008/</a></h4>
<hr>
<h5 id="스타일가이드-한글-번역-블로그-httpskongdols-room.tistory.com18">스타일가이드 한글 번역 블로그: <a href="https://kongdols-room.tistory.com/18">https://kongdols-room.tistory.com/18</a></h5>
<h5 id="내용-중-일부-출처-httpswikidocs.net13">내용 중 일부 출처: <a href="https://wikidocs.net/13">https://wikidocs.net/13</a></h5>
<h5 id="내용-중-일부-출처-httpswww.codingfactory.net11753">내용 중 일부 출처: <a href="https://www.codingfactory.net/11753">https://www.codingfactory.net/11753</a></h5>
<h5 id="내용-중-일부-출처-httpsterms.naver.comentry.nhndocid3580815cid59088categoryid59096">내용 중 일부 출처: <a href="https://terms.naver.com/entry.nhn?docId=3580815&amp;cid=59088&amp;categoryId=59096">https://terms.naver.com/entry.nhn?docId=3580815&amp;cid=59088&amp;categoryId=59096</a></h5>
<hr>
<h3 id="파이썬">[파이썬?]</h3>
<p>파이썬은 1991년 네덜란드 개발자 귀도 반 로섬(Guido  van  Rossum)이  발표한 고급 프로그래밍 언어로, 인터프리터식, 객체지향적, 동적 타이핑 대화형 언어이다.  ‘파이썬(Python)’이란 원래 그리스 신화에 나오는 뱀 이름으로 파이썬 로고에 두 개의 뱀 그림이 있다. 파이썬 홈페이지에 따르면 “귀도 반 로섬은 짧고, 특별하고, 미스터리한 느낌의 단어를 찾았다”며 “그래서 파이썬이란 이름을 결정했다”라고 되어있다</p>
<hr>
<h3 id="기본용어">[기본용어]</h3>
<ul>
<li><strong>프로그래밍(Programming):</strong> 계산할 수식을 컴퓨터에 알려줌</li>
<li><strong>소스 코드 (source code):</strong> 사람들이 쉽게 읽고 이해하도록 프로그래밍 언어로 작성한 코드. 프로그래밍 언어로 소스코드를 만들고, 이를 컴퓨터가 이해하는 이진코드로 바꾼다</li>
<li><strong>토큰(Token):</strong> 공백, 쉼표, 마침표 등으로 분리할 수 없는 가장 작은 단위  (토큰 &gt; 식별자(Identifier): 함수, 변수)<br>
ex&gt; my_name: 공백이 아닌, 언더스코어<kbd>_</kbd> 로 구분</li>
<li><strong>코멘트(Comment):</strong> 복잡한 코드설명 및 다른 개발자들과 소통</li>
<li><strong>할당(지정)연산자(Assignment Operator):</strong> <kbd>=</kbd> 우측 값을 좌측(변수)에 할당(지정)</li>
<li><strong>비교연산자(Comparison Operator):</strong> <kbd>==</kbd>  값이 동일하다  &lt;-&gt; <kbd>!=</kbd> 값이 동일하지 않다</li>
<li><strong>세계 표준시(UTC):</strong> 세계표준시(UTC)로 1970년 1월 1일 0시 0분 0초를 기준으로 몇 초가 지났는지를 정수로 나타내는 시간</li>
<li><strong>인터프리터(interpreter):</strong> 프로그래밍 소스코드를 실행시켜주는 프로그램. 한 번에 한 줄씩 읽어 실행하며, 파이썬의 경우 ‘파이썬 인터프리터’</li>
<li><strong>자료형(Data Type):</strong> 자료 형태로 사용하는 모든 것. 프로그램의 기본이자 핵심단위가 바로 ‘자료형’</li>
<li><strong>추상화(Abstraction):</strong> 복잡한 내용을 숨겨, 주요기능에만 신경쓰도록 함</li>
</ul>
<hr>
<h3 id="기본개념">[기본개념]</h3>
<ul>
<li>
<p><strong>자료형(Data Type)</strong><br>
숫자(Number) &gt; 정수(Integer) + 소수(Floating Point) &gt; 연산<br>
문자열(String) &gt; " ", ’ '로 감싸짐 &gt; 포맷팅 &gt; 문자열 함수<br>
불린(Boolean) &gt; 불대수[참(True) / 거짓(False)] &gt; 불린 연산<br>
리스트(List), 튜플(Tuple), 딕셔너리(Dictionary), 집합(Set)</p>
</li>
<li>
<p><strong>추상화(Abstraction)</strong><br>
변수(Variable) / 함수(Function) / 객체(Object)</p>
</li>
</ul>
<hr>
<h2 id="pep-8--style-guide-中-중요포인트">[PEP 8 : Style Guide 中 중요포인트]</h2>
<h3 id="이름-변수함수-이름은-소문자--여러단어는-kbd_kbd로-연결">1) 이름: 변수/함수 이름은 ‘소문자’ + 여러단어는 '<kbd>_</kbd>'로 연결</h3>
<pre><code>some_variable_name = 1  
def some_function_name():  
    print("Hello!")  
</code></pre>
<h4 id="상수-이름은-대문자">1-2) 상수 이름은 ‘대문자’</h4>
<pre><code>SOME_CONSTANT_NAME = 3.14  
</code></pre>
<h4 id="의미있는-이름--a-b같은-이름x">1-3) ‘의미있는 이름’  (a, b같은 이름x)</h4>
<pre><code>radius = 2  
PI = 3.14  
print(PI * radius * radius)  
  
  
def say_hello():  
    print("Hello, Harry!")  
</code></pre>
<h3 id="white-space화이트-스페이스-들여쓰기는-무조건-4-스페이스">2) White space(화이트 스페이스): 들여쓰기는 무조건 ‘4 스페이스’</h3>
<pre><code>def say_hello():  
    print("Hello, Harry!")  # 들여쓰기 4번 (tab x)
</code></pre>
<h3 id="함수정의-함수정의-위아래-빈-줄-2줄씩.">3) 함수정의: 함수정의 ‘위,아래 빈 줄 2줄씩.’</h3>
<p><em>BUT, 파일의 첫 줄이 함수면 괜찮다.</em></p>
<pre><code>def a():  # 위,아래 빈 줄 2줄씩.  
  print('a')  
</code></pre>
<h3 id="괄호-안-괄호-바로-안은-띄어쓰기-하지-말-것">4) 괄호 안: 괄호 바로 안은 띄어쓰기 하지 말 것</h3>
<pre><code>harry(ron[1], {james: 2})        # good
harry( ron[ 1 ], { james : 2 } )  # bad
</code></pre>
<h3 id="함수-괄호-함수-정의-및-호출시-함수이름과-괄호사이-띄어쓰기-하지-말-것">5) 함수 괄호: 함수 정의 및 호출시, 함수이름과 괄호사이 띄어쓰기 하지 말 것</h3>
<pre><code>def name(x):   # good
def name (a):  # bad
</code></pre>
<h3 id="쉼표-쉼표-앞은-띄어쓰기-하지-말-것">6) 쉼표: 쉼표 앞은 띄어쓰기 하지 말 것</h3>
<pre><code>print(a, a)   # good
print(a , b)  # bad  
</code></pre>
<h3 id="지정연산자-지정연산자-앞뒤-띄어쓰기-한-번씩">7) 지정연산자: 지정연산자 앞,뒤 띄어쓰기 한 번씩</h3>
<pre><code>x = 1 # good  
 x=1  # bad
</code></pre>
<h3 id="연산자-연산자-앞뒤-띄어쓰기-한-번씩">8) 연산자: 연산자 앞,뒤 띄어쓰기 한 번씩</h3>
<pre><code>x = x + 1  
x += 1  # 위와 같은 의미를 가진 식
</code></pre>
<h3 id="연산의-우선순위-강조시-연산자-앞뒤-붙여쓰기-권장">9) 연산의 ‘우선순위’ 강조시 연산자 앞,뒤 붙여쓰기 권장</h3>
<pre><code>x = x*2 - 1  
x = x*x + x*x  
c = (x+x) * (x-x)  
</code></pre>
<h3 id="주석코멘트-일반코드와-같은-줄에-코멘트를-쓸-경우-코멘트-앞-띄어쓰기-두-번-뒤-띄어쓰기-한-번">10) 주석/코멘트: 일반코드와 같은 줄에 코멘트를 쓸 경우, 코멘트 앞 띄어쓰기 두 번, 뒤 띄어쓰기 한 번</h3>
<p><strong><em>주석 토글 단축키:</em> <kbd>ctrl+<kbd>/</kbd></kbd></strong></p>
<pre><code>x = x + 1  # 코멘트 
</code></pre>
<hr>
<h3 id="코딩스타일-이해-쉽고-가독성-좋은-코드--좋은-스타일의-코드">코딩스타일: 이해 쉽고 가독성 좋은 코드 &gt; 좋은 스타일의 코드</h3>
<h4 id="좋은-코딩스타일-숫자를-변수에-넣어-사용-적절한-함수사용-및-코멘트로-설명을-달아주어-알아보고-이해하기-쉬운-경우">좋은 코딩스타일: 숫자를 변수에 넣어 사용, 적절한 함수사용 및 코멘트로 설명을 달아주어 알아보고 이해하기 쉬운 경우</h4>
<pre><code>PI = 3.14  # 이것은 원주율(파이)를 나타냄
</code></pre>
<h4 id="나쁜-코딩스타일-코드의-목적이나-숫자들이-뭘-의미하는지-알-수-없고-가독성이-떨어짐">나쁜 코딩스타일: 코드의 목적이나 숫자들이 뭘 의미하는지 알 수 없고, 가독성이 떨어짐</h4>
<pre><code>print(6.28*4)  # 200.96  
print(3.14*4*4)  # 50.24  
print(6.28*8)  # 50.24  
print(3.14*8*8)  # 200.96  
# 무엇을 위한 코드인지, 숫자들이 무엇을 의미하는지 알 수 없다
</code></pre>

