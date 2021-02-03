---


---

<h3 id="형-변환type-conversioncasting-값을-한-자료형에서-다른-자료형으로-변경">3&gt; 형 변환(Type Conversion/Casting): 값을 한 자료형에서 다른 자료형으로 변경</h3>
<pre><code>print(int(3.8))  # 3  # 소수형 &gt;정수형  
print(float(3))  # 3.0  # 정수형 &gt; 소수형  
print(int("2") + int("5"))  
# 2 + 5 = 7  # 문자열 &gt; 정수형  
print(float("1.1") + float("2.5"))  
# 1.1 + 2.5 = 3.6  # 문자열 &gt; 소수형  
print(str(2) + str(5))  
# "2" + "5" = "25" # 정수형 &gt; 문자열  
  
age = 17  
print("제 나이는 " + str(age) + "살 입니다.")  
# 제 나이는 17살 입니다.  # 정수형 &gt; 문자열  
print(int("Hello harry!"))  
# 문자열을 정수형으로 형 변환 할 수 없는 경우
</code></pre>
<h3 id="문자열-포맷팅format">4&gt; 문자열 포맷팅(format)</h3>
<p>year = 2020<br>
month = 12<br>
day = 29</p>
<h4 id="기본적인-방법">1) 기본적인 방법</h4>
<pre><code># 오늘은 2020년 12월 29일 입니다.  
print("오늘은 " + str(year) + "년 " + str(month) + "월 " + str(day) + "일 입니다.")  
</code></pre>
<h4 id="format-을-이용한-문자열-작성">2) ‘.format’ 을 이용한 문자열 작성</h4>
<pre><code># 오늘은 2020년 12월 29일 입니다.  
print("오늘은 {}년 {}월 {}일 입니다.".format(year, month, day))  
</code></pre>
<h4 id="변수를-이용한-문자열-작성">3) '변수’를 이용한 문자열 작성</h4>
<pre><code># 오늘은 2020년 12월 30일 입니다.  
date_string = "오늘은 {}년 {}월 {}일 입니다."  
print(date_string.format(year, month, day + 1)) 
</code></pre>
<h4 id="f-string을-이용한-문자열-작성">4) 'f-string’을 이용한 문자열 작성</h4>
<pre><code># 오늘은 2020년 12월 31일 입니다.  
print(f"오늘은 {year}년 {month}월 {day + 2}일 입니다.") 
</code></pre>
<h4 id="를-이용한-문자열-작성">5) '%'를 이용한 문자열 작성</h4>
<pre><code># 오래된 방법(잘 안씀)  
# 오늘은 2020년 12월 30일 입니다.
print("오늘은 %s년 %d월 %r일 입니다." % (year, month, day + 1))  
</code></pre>
<h4 id="format-어떤-자료형이든-문자열로-변환">6) format: 어떤 자료형이든 문자열로 변환</h4>
<pre><code> # 난 해리, 론, 조지를(을) 좋아해!  
print("난 {}, {}, {}를(을) 좋아해!".format("해리", "론", "조지")) 
</code></pre>
<h4 id="파라미터-순서변경012순으로-순서지정">7) 파라미터 순서변경(0,1,2순으로 순서지정)</h4>
<pre><code> # 난 조지, 해리, 론를(을) 좋아해!  
print("난 {2}, {0}, {1}를(을) 좋아해!".format("해리", "론", "조지"))  
</code></pre>
<h4 id="소수형-반올림-및-자리수-표시방법">8) 소수형 반올림 및 자리수 표시방법</h4>
<pre><code>num_1 = 1  
num_2 = 3  
# 1나누기 3은 0.3333333333333333입니다.  
print("{0} 나누기 {1}은 {2}입니다.".format(num_1, num_2, num_1 / num_2))  
</code></pre>
<h4 id="반올림-표시-원하는-파라미터-뒤-.nf-소숫점-이하-몇자리까지-표시지정">반올림 표시: 원하는 파라미터 뒤 ‘:.(n)f’ 소숫점 이하 몇자리까지 표시지정</h4>
<pre><code># 1나누기 3은 0.33입니다 
print("{0} 나누기 {1}은 {2:.2f}입니다.".format(num_1, num_2, num_1 / num_2))  
</code></pre>
<h4 id="소수형을-정수로-표시-할-때-.0f">소수형을 정수로 표시 할 때 ‘:.0f’</h4>
<pre><code># 1나누기 3은 0입니다
print("{0} 나누기 {1}은 {2:.0f}입니다.".format(num_1, num_2, num_1 / num_2))  
</code></pre>
<h4 id="round-함수를-이용한-반올림">round 함수를 이용한 반올림</h4>
<pre><code># 1나누기 3은 0.33입니다
print("{0} 나누기 {1}은 {2}입니다.".format(num_1, num_2, round(num_1 / num_2, 2)))  
</code></pre>
<h4 id="or--표현하기">9) ‘{’ or ‘}’ 표현하기</h4>
<pre><code>c = "{{ and }}".format()  
print(c)  # { and }  
</code></pre>
<h4 id="format-함수로-문자열-포맷팅시--와-같은-중괄호를-문자-그대로-쓸-경우--처럼-2개를-연속해-사용">format 함수로 문자열 포맷팅시 { }와 같은 중괄호를 문자 그대로 쓸 경우, {{ }}처럼 2개를 연속해 사용</h4>

