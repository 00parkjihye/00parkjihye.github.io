---


---

<h2 id="자료형data-type">[자료형(Data Type)]</h2>
<h3 id="숫자형정수-연산">1&gt; 숫자형(정수) 연산</h3>
<h4 id="덧셈addition">덧셈(addition)</h4>
<pre><code>print(4 + 6)  # 10  
</code></pre>
<h4 id="뺄셈subtraction">뺄셈(subtraction)</h4>
<pre><code>print(2 - 4)  # -2  
</code></pre>
<h4 id="곱셈multiplication">곱셈(multiplication)</h4>
<pre><code>print(4 * 2)  # 8  
</code></pre>
<h4 id="나머지modulo-연산">나머지(modulo) 연산</h4>
<pre><code>print(7 % 3)  # 1 (7을 3으로 나누었을때 나머지)  
</code></pre>
<h4 id="거듭제곱exponentiation">거듭제곱(exponentiation)</h4>
<pre><code>print(2 ** 3)  # 8  
</code></pre>
<h4 id="divmod-함수몫과-나머지-한번에-계산">divmod() 함수(몫과 나머지 한번에 계산)</h4>
<pre><code>print(divmod(50, 8))  # (6, 2)  
# 50을 8로 '나눈 몫 6', '나머지 2'가 한 번에 계산됨
</code></pre>
<h3 id="소수형-연산-어느-하나라도-소수형이면-결과-역시-소수형">1-1&gt; 소수형 연산: 어느 하나라도 소수형이면, 결과 역시 소수형</h3>
<h4 id="덧셈">덧셈</h4>
<pre><code>print(4.0 + 6.0)  # 10.0  
</code></pre>
<h4 id="뺄셈">뺄셈</h4>
<pre><code>print(2.0 - 4.0)  # -2.0  
</code></pre>
<h4 id="곱셈">곱셈</h4>
<pre><code>print(4.0 * 2.0)  # 8.0  
</code></pre>
<h4 id="나머지-연산">나머지 연산</h4>
<pre><code>print(7.0 % 3.0)  # 1.0  
</code></pre>
<h4 id="거듭제곱">거듭제곱</h4>
<pre><code>print(2.0 ** 3.0)  # 8.0  
</code></pre>
<h4 id="나눗셈division-언제나-결과는-소수형부동소수-때문">나눗셈(division): ‘언제나’ 결과는 ‘소수형’(부동소수 때문)</h4>
<pre><code>print(7 / 2)  # 3.5  
print(6 / 2)  # 3.0  
print(7.0 / 2)  # 3.5  
print(6.0 / 2.0)  # 3.0  
</code></pre>
<h4 id="복합계산--일반-사칙연산과-같음">복합계산 : 일반 사칙연산과 같음</h4>
<pre><code>print(2 + 3 * 2)  # 3 * 2 = 6 + 2 = 8   
print(2 * (2 + 3))  # 2 + 3 = 5 * 2 = 10 
# (괄호 먼저계산)  
</code></pre>
<h4 id="floor-division버림-나눗셈-나누되-정수형으로-값을-변환">floor division(버림 나눗셈): 나누되 정수형으로 값을 변환</h4>
<pre><code>print(7 // 2)  # 7 / 2에서 소숫점 버리고 '3'만 출력
print(8 // 3)  # 8 / 3에서 소숫점 버리고 '2'만 출력
print(8.0 // 3)  # 2.0 (하나라도 소수면 결과는 소수형)  
print(8 // 3.0)  # 2.0  
print(8.0 // 3.0)  # 2.0  
</code></pre>
<h4 id="round-함수반올림-함수-가장-가까운-정수형으로-반올림">round 함수(반올림 함수): 가장 가까운 정수형으로 반올림</h4>
<pre><code>print(round(3.1415926535))  # 3  
print(round(3.1415926535, 2))  # 3.14 
print(round(3.1415926535, 4))  # 3.1416  
# (숫자, 반올림할 자릿수)  
</code></pre>
<h3 id="문자열string-kbd----kbd-따옴표로-감싸짐">2&gt; 문자열(String): <kbd>"  " ’ ’</kbd> 따옴표로 감싸짐</h3>
<pre><code>print("해리포터")  # 해리포터  
print('론위즐리')  # 론위즐리  
</code></pre>
<h4 id="문장-안-kbd----kbd-표시">문장 안 <kbd>" " ’  ’</kbd> 표시</h4>
<pre><code>print("I'm happy!")  # I'm happy!  
# 문장 전체를 감싸준 따옴표가 아닌, 다른 따옴표 사용

print('I\'m happy!')  # I'm happy!  
# 역슬래쉬 |를 따옴표 앞에 써줌
</code></pre>
<h4 id="문자열-연결string-concatenation-문자열끼리-연결하는-연산">문자열 연결(String Concatenation): 문자열끼리 연결하는 연산</h4>
<pre><code>print("Hello " + "Harry!")  # Hello Harry!  
print("2" + "4")  # 24  
print("프레드 " * 2)  # 프레드 프레드 
# 옆으로 반복출력  
print("헤르미온느\n" * 2)  # 헤르미온느 
                         # 헤르미온느 
# 밑으로 반복출력('\n'은 줄바꿈)
</code></pre>

