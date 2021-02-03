---


---

<h3 id="문자열-관련-함수들">5&gt; 문자열 관련 함수들</h3>
<p>문자열 자료형은 자체적으로 '문자열 내장함수’가 있다<br>
내장함수 사용시 문자열 변수이름 뒤에 <code>.</code>를 붙이고 함수이름을 쓴다</p>
<h4 id="문자-갯수-세기-.countx-문자열-중-문자-x의-갯수를-돌려줌">1) 문자 갯수 세기: ‘.count(x)’ 문자열 중 문자 x의 갯수를 돌려줌</h4>
<pre><code>a = "hobby"  
print(a.count('b'))  # 2  
</code></pre>
<h4 id="위치-알려주기-.findx-문자열-중-문자-x가-처음으로-나온-위치-반환.-만약-찾는-문자문자열이-존재하지-않으면--1-반환">2) 위치 알려주기: ‘.find(x)’ 문자열 중 문자 x가 ‘처음으로 나온’ 위치 반환. 만약, 찾는 문자/문자열이 '존재하지 않으면 <code>-1</code>’ 반환</h4>
<pre><code>a = "Python is the best choice"  
print(a.find('b'))  # 14  
print(a.find('k'))  # -1  # 찾는 문자/문자열이'존재하지 않아 -1반환' 
</code></pre>
<h4 id="위치-알려주기2-.indexx-문자열-중-문자-x가-처음으로-나온-위치-반환.-찾는-문자문자열이-존재하지-않으면-오류발생">3) 위치 알려주기2: ‘.index(x)’ 문자열 중 문자 x가 처음으로 나온 위치 반환. 찾는 문자/문자열이 존재하지 않으면 오류발생</h4>
<pre><code>a = "Life is too short"  
print(a.index('t'))  # 8 # 문자열 중 문자 t가 처음나온 위치반환
print(a.index('k'))  # Traceback(most recent call last):  
# ValueError: substring not found  
만약 찾는 문자/문자열이 존재하지 않으면 위처럼 오류발생 
'find(x)'함수와 다른점: 문자열에 존재하지 않는 문자를 찾으면'오류발생'  
</code></pre>
<h4 id="문자열-삽입--or-.join">4) 문자열 삽입: <code>,</code> or <code>/</code>.join()</h4>
<pre><code>e = ",".join('abcd')  
print(e)  # 'a,b,c,d'  
abcd 문자열 각각의 문자사이에 `,` 삽입
join 함수는 문자열뿐 아니라 리스트, 튜플에도 사용
</code></pre>
<h4 id="join-함수의-입력으로-리스트를-사용시">4-1) join 함수의 입력으로 리스트를 사용시,</h4>
<pre><code>g = `,`.join(['a', 'b', 'c', 'd'])  
print(g)  # 'a,b,c,d'  
</code></pre>
<h4 id="소문자를-대문자로upper-.upper-소문자를-대문자로-바꿈.-문자열이-이미-대문자면-아무변화도-일어나지-않음">5) 소문자를 대문자로(upper): <code>.upper()</code> 소문자를 대문자로 바꿈. 문자열이 이미 대문자면, 아무변화도 일어나지 않음</h4>
<pre><code>a = "hi"  
print(a.upper())  # 'HI'  
</code></pre>
<h4 id="대문자를-소문자lower-.lower-대문자를-소문자로-바꿈">6) 대문자를 소문자(lower): ‘.lower()’ 대문자를 소문자로 바꿈</h4>
<pre><code>a = "HI"  
print(a.lower())  # 'hi'  
</code></pre>
<h4 id="왼쪽-공백-지우기lstrip-.lstrip-문자열-중-가장-왼쪽공백을-모두지움-lstrip의-l은-left">7) 왼쪽 공백 지우기(lstrip): <code>.lstrip()</code> 문자열 중 가장 왼쪽공백을 모두지움 lstrip의 l은 left</h4>
<pre><code>a = " hi "  
print(a.lstrip())  # 'hi '  
</code></pre>
<h4 id="오른쪽-공백-지우기rstrip-.rstrip-문자열-중-가장-오른쪽공백을-모두지움-rstrip의-r은-right">8) 오른쪽 공백 지우기(rstrip): <code>.rstrip()</code> 문자열 중 가장 오른쪽공백을 모두지움 rstrip의 r은 right</h4>
<pre><code>a = " hi "  
print(a.rstrip())  # ' hi'  
</code></pre>
<h4 id="양쪽-공백-지우기strip-.strip-문자열-양쪽공백-모두지움">9) 양쪽 공백 지우기(strip): <code>.strip()</code> 문자열 양쪽공백 모두지움</h4>
<pre><code>a = " hi "  
print(a.strip())  # 'hi'  
</code></pre>
<h4 id="문자열-바꾸기-.replace바꾸고싶은-문자-바꿀-문자-문자열-안의-특정-값을-다른-값으로-변경">10) 문자열 바꾸기: <code>.replace(바꾸고싶은 문자, 바꿀 문자)</code> 문자열 안의 특정 값을 다른 값으로 변경</h4>
<pre><code>a = "Life is too short"  
print(a.replace("Life", "Your leg"))  # 'Your leg is too short'  
</code></pre>
<h4 id="문자열-나누기.split-.split">11) 문자열 나누기(.split()): <code>.split()</code></h4>
<pre><code>a = "Life is too short"  
print(a.split())  # ['Life', 'is', 'too', 'short']  
b = "a:b:c:d"  
print(b.split(':'))  # ['a', 'b', 'c', 'd']  
</code></pre>
<p><code>a.split()</code> 처럼 괄호 안에 아무값도 넣지않으면, 공백(스페이스, 탭, 엔터 등) 기준으로 문자열을 나눔<br>
만약 <code>b.split(':')</code> 처럼 괄호 안 특정 값이 있을경우, 괄호 안의 값을 구분자로 문자열을 나눔<br>
위처럼 나눈값은 리스트에 하나씩 들어감 [‘Life’, ‘is’, ‘too’, ‘short’]나 [‘a’, ‘b’, ‘c’, ‘d’]가 리스트</p>
<h4 id="이스케이프-문자escape-character-원래-가지고-있던-문자열의-출력하는-기능이-아닌-다른-특정기능을-하는-문자">6&gt; 이스케이프 문자(escape character): 원래 가지고 있던 문자열의 출력하는 기능이 아닌 다른 특정기능을 하는 문자</h4>
<h4 id="백슬래시-기호가-붙은-특수문자"><code>\</code>(백슬래시) 기호가 붙은 특수문자</h4>
<h5 id="n--다음-줄로-이동개행">1) <code>\n</code> : 다음 줄로 이동(개행)</h5>
<h5 id="r-해당-줄의-처음으로-이동">2) <code>\r</code>: 해당 줄의 처음으로 이동</h5>
<h5 id="t--8칸-공백">3) <code>\t</code> : ‘8칸’ 공백</h5>
<h5 id="or----or--문자">4) <code>\'</code> or <code>\"</code> : ’ or " 문자</h5>
<h5 id="문자">5) <code>\\</code> : \문자</h5>
<hr>
<h5 id="n">1) <code>\n</code></h5>
<pre><code>print("Hello\nWorld")  
결과:  
Hello  # 다음줄로 개행(줄 바꿈)  
World  
</code></pre>
<h5 id="r">2) <code>\r</code></h5>
<pre><code>print("Hello\rHi")   
결과:  
Hillo # Hello 출력후 '맨 앞으로 이동해 Hi를 덮어씀'  
</code></pre>
<p>한글과 영어를 섞어쓸 땐 결과가 다를 수 있는데, 영어는 글자당 1byte 한글은 2byte라서</p>
<h5 id="t">3) <code>\t</code></h5>
<pre><code>print("Hello\tWorld")  
결과:  
Hello   World # 문자사이 8칸이아닌'앞글자 포함8칸'확보(이경우'Hello+공백'합해8칸)  
</code></pre>
<h5 id="section">4) <code>\'</code></h5>
<pre><code>print("\'Hello World\'")  
결과:  
'Hello World'  
</code></pre>
<h5 id="section-1">4-2) <code>\"</code></h5>
<pre><code>print("\"Hello World\"")  
결과:  
"Hello World"  
</code></pre>
<h5 id="section-2">5) <code>\\</code></h5>
<pre><code>print("C:\\Program Files\\Python35\Scripts\\")  
결과:  
C:\Program Files\Python35\Scripts\  # \ 문자
</code></pre>
<h5 id="문자열-곱하기-응용-1">6) 문자열 곱하기 응용 1</h5>
<pre><code>print("-"*10)  # 출력: ---------- (-가 10번 반복)
# 문자열 곱하기는'문자열이 곱한 수 만큼'반복

print("\nHello Harry! "*3)  
결과:  
Hello Harry! 
Hello Harry! 
Hello Harry!  
# 문자열이 3번나옴
</code></pre>
<h5 id="문자열-곱하기-응용-2">7) 문자열 곱하기 응용 2</h5>
<pre><code>multistring.py  
print("=" * 50)  
print("My Program")  
print("=" * 50)  

결과: 프로그램을 실행시킬때 출력되는 화면 제일위에 프로그램 제목이 
이렇게 표시됨
================================================
My Program  
================================================
</code></pre>

