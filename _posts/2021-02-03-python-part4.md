---


---

<h1 id="문자열-관련-함수들">5&gt; 문자열 관련 함수들</h1>
<h1 id="문자열-자료형은-자체적으로-문자열-내장함수가-있다.">문자열 자료형은 자체적으로 '문자열 내장함수’가 있다.</h1>
<h1 id="내장함수-사용시-문자열-변수이름-뒤-‘.’를-붙인뒤-함수이름을-써주면-된다.">내장함수 사용시 문자열 변수이름 뒤 ‘.’를 붙인뒤 함수이름을 써주면 된다.</h1>
<h1 id="문자-갯수-세기-.countx-문자열-중-문자-x의-갯수를-돌려줌.">1) 문자 갯수 세기: ‘.count(x)’ 문자열 중 문자 x의 갯수를 돌려줌.</h1>
<p>a = “hobby”<br>
print(a.count(‘b’))  # 2</p>
<h1 id="위치-알려주기-.findx-문자열-중-문자-x가-처음으로-나온-위치-반환.-만약-찾는-문자나-문자열이-존재하지-않는다면--1을-반환.">2) 위치 알려주기: ‘.find(x)’ 문자열 중 문자 x가 ‘처음으로 나온’ 위치 반환. 만약, 찾는 문자나 문자열이 '존재하지 않는다면 -1’을 반환.</h1>
<p>a = “Python is the best choice”<br>
print(a.find(‘b’))  # 14<br>
print(a.find(‘k’))  # -1  # 찾는 문자나 문자열이 ‘존재하지 않아 -1 반환’</p>
<h1 id="위치-알려주기2-.indexx-문자열-중-문자-x가-처음으로-나온-위치-반환.-찾는-문자나-문자열이-존재하지-않으면-오류-발생.">3) 위치 알려주기2: ‘.index(x)’ 문자열 중 문자 x가 처음으로 나온 위치 반환. 찾는 문자나 문자열이 존재하지 않으면 오류 발생.</h1>
<p>a = “Life is too short”<br>
print(a.index(‘t’))  # 8  # 문자열 중 문자 t가 맨 처음으로 나온 위치 반환.</p>
<h1 id="printa.indexk---traceback-most-recent-call-last---valueerror-substring-not-found">print(a.index(‘k’))  # Traceback (most recent call last):  # ValueError: substring not found</h1>
<h1 id="만약-찾는-문자나-문자열이-존재하지-않는다면-위처럼-오류-발생.">만약 찾는 문자나 문자열이 존재하지 않는다면 위처럼 오류 발생.</h1>
<h1 id="findx-함수와-다른-점-문자열에-존재하지-않는-문자를-찾으면-오류-발생">‘find(x)’ 함수와 다른 점: 문자열에 존재하지 않는 문자를 찾으면 ‘오류 발생’</h1>
<h1 id="문자열-삽입--or-.join">4) 문자열 삽입: “, or /”.join()</h1>
<p>e = “,”.join(‘abcd’)<br>
print(e)  # ‘a,b,c,d’</p>
<h1 id="abcd-문자열-각각의-문자-사이에-를-삽입.">abcd 문자열 각각의 문자 사이에 ','를 삽입.</h1>
<h1 id="join-함수는-문자열뿐-아니라-리스트나-튜플에도-사용.">join 함수는 문자열뿐 아니라 리스트나 튜플에도 사용.</h1>
<h1 id="join-함수의-입력으로-리스트를-사용시">4-1) join 함수의 입력으로 리스트를 사용시,</h1>
<p>g = “,”.join([‘a’, ‘b’, ‘c’, ‘d’])<br>
print(g)  # ‘a,b,c,d’</p>
<h1 id="소문자를-대문자로upper-.upper-소문자를-대문자로-바꿈.-문자열이-이미-대문자면-아무-변화도-일어나지-않음.">5) 소문자를 대문자로(upper): ‘.upper()’ 소문자를 대문자로 바꿈. 문자열이 이미 대문자면, 아무 변화도 일어나지 않음.</h1>
<p>a = “hi”<br>
print(a.upper())  # ‘HI’</p>
<h1 id="대문자를-소문자lower-.lower-대문자를-소문자로-바꿈.">6) 대문자를 소문자(lower): ‘.lower()’ 대문자를 소문자로 바꿈.</h1>
<p>a = “HI”<br>
print(a.lower())  # ‘hi’</p>
<h1 id="왼쪽-공백-지우기lstrip-.lstrip-문자열-중-가장-왼쪽-공백을-모두-지움.-lstrip의-l은-left.a---hi-">7) 왼쪽 공백 지우기(lstrip): ‘.lstrip()’ 문자열 중 가장 왼쪽 공백을 모두 지움. lstrip의 l은 left.a = " hi "</h1>
<p>print(a.lstrip())  # 'hi ’</p>
<h1 id="오른쪽-공백-지우기rstrip-.rstrip-문자열-중-가장-오른쪽-공백을-모두-지움.-rstrip의-r은-right.a---hi-">8) 오른쪽 공백 지우기(rstrip): ‘.rstrip()’ 문자열 중 가장 오른쪽 공백을 모두 지움. rstrip의 r은 right.a = " hi "</h1>
<p>print(a.rstrip())  # ’ hi’</p>
<h1 id="양쪽-공백-지우기strip-.strip-문자열-양쪽-공백을-모두-지움.">9) 양쪽 공백 지우기(strip): ‘.strip()’ 문자열 양쪽 공백을 모두 지움.</h1>
<p>a = " hi "<br>
print(a.strip())  # ‘hi’</p>
<h1 id="문자열-바꾸기-.replace바꾸고싶은-문자-바꿀-문자-문자열-안의-특정-값을-다른-값으로-변경.">10) 문자열 바꾸기: ‘.replace(바꾸고싶은 문자, 바꿀 문자))’ 문자열 안의 특정 값을 다른 값으로 변경.</h1>
<p>a = “Life is too short”<br>
print(a.replace(“Life”, “Your leg”))  # ‘Your leg is too short’</p>
<h1 id="문자열-나누기.split-.split">11) 문자열 나누기(.split()): ‘.split()’</h1>
<p>a = “Life is too short”<br>
print(a.split())  # [‘Life’, ‘is’, ‘too’, ‘short’]<br>
b = “a🅱️c:d”<br>
print(b.split(’:’))  # [‘a’, ‘b’, ‘c’, ‘d’]</p>
<h1 id="a.split처럼-괄호-안에-아무값도-넣지-않으면-공백스페이스-탭-엔터-등-기준으로-문자열을-나눔.">a.split()처럼 괄호 안에 아무값도 넣지 않으면, 공백(스페이스, 탭, 엔터 등) 기준으로 문자열을 나눔.</h1>
<h1 id="만약-b.split처럼-괄호-안-특정-값이-있을-경우-괄호-안의-값을-구분자로-문자열을-나눔.">만약 b.split(’:’)처럼 괄호 안 특정 값이 있을 경우, 괄호 안의 값을 구분자로 문자열을 나눔.</h1>
<h1 id="위처럼-나눈-값은-리스트에-하나씩-들어감.-life-is-too-short나-a-b-c-d가-리스트.">위처럼 나눈 값은 리스트에 하나씩 들어감. [‘Life’, ‘is’, ‘too’, ‘short’]나 [‘a’, ‘b’, ‘c’, ‘d’]가 리스트.</h1>
<h1 id="이스케이프-문자escape-character-원래-가지고-있던-문자열의-출력하는-기능을-벗어나-다른-특정한-기능을-하는-문자.">6&gt; 이스케이프 문자(escape character): 원래 가지고 있던 문자열의 출력하는 기능을 벗어나 다른 특정한 기능을 하는 문자.</h1>
<h1 id="백슬래시-기호가-붙은-특수한-문자.">(백슬래시) 기호가 붙은 특수한 문자.</h1>
<h1 id="n--다음-줄로-이동개행">1) \n : 다음 줄로 이동(개행)</h1>
<h1 id="r-해당-줄의-처음으로-이동">2) \r :해당 줄의 처음으로 이동</h1>
<h1 id="t--8칸-공백">3) \t : ‘8칸’ 공백</h1>
<h1 id="or----or--문자">4) ’ or " : ’ or " 문자</h1>
<h1 id="문자">5) \ : \문자</h1>
<h1 id="n">1)\n</h1>
<h1 id="printhellonworld">print(“Hello\nWorld”)</h1>
<h1 id="출력결과">출력결과:</h1>
<h1 id="hello---다음-줄로-개행줄-바꿈">Hello  # 다음 줄로 개행(줄 바꿈)</h1>
<h1 id="world">World</h1>
<h1 id="r">2) \r</h1>
<h1 id="printhellorhi">print(“Hello\rHi”)</h1>
<h1 id="출력결과-1">출력결과:</h1>
<h1 id="hillo--hello-출력-후-맨-앞으로-이동해-hi를-덮어씀">Hillo # Hello 출력 후 ‘맨 앞으로 이동해 Hi를 덮어씀’</h1>
<h1 id="한글과-영어를-섞어쓸-땐-결과가-다를-수-있는데-영어는-글자당-1byte-한글은-2byte-라서임.">한글과 영어를 섞어쓸 땐 결과가 다를 수 있는데, 영어는 글자당 1byte 한글은 2byte 라서임.</h1>
<h1 id="t">3) \t</h1>
<h1 id="printhellotworld">print(“Hello\tWorld”)</h1>
<h1 id="출력결과-2">출력결과:</h1>
<h1 id="hello---world--문자사이-8칸이아닌-앞-글자-포함-8칸-확보.이경우-hello공백-합해-8칸">Hello   World # 문자사이 8칸이아닌 ‘앞 글자 포함 8칸’ 확보.(이경우 ‘Hello+공백’ 합해 8칸)</h1>
<h1 id="section">4) ’</h1>
<h1 id="printhello-world">print("‘Hello World’")</h1>
<h1 id="출력결과-3">출력결과:</h1>
<h1 id="hello-world">‘Hello World’</h1>
<h1 id="section-1">4-2) "</h1>
<h1 id="printhello-world-1">print("“Hello World”")</h1>
<h1 id="출력결과-4">출력결과:</h1>
<h1 id="hello-world-1">“Hello World”</h1>
<h1 id="section-2">6) \</h1>
<h1 id="printcprogram-filespython35scripts">print(“C:\Program Files\Python35\Scripts\”)</h1>
<h1 id="출력결과-5">출력결과:</h1>
<h1 id="cprogram-filespython35scripts----문자.">C:\Program Files\Python35\Scripts\  # \ 문자.</h1>
<h1 id="문자열-곱하기-응용-1-print-10---출력-----------이렇게-문자열을-곱하기면-문자열이-곱한-수-만큼-반복됨.">7) 문자열 곱하기 응용 1# print("-"*10)  # 출력:---------- 이렇게 문자열을 곱하기면 ‘문자열이 곱한 수 만큼’ 반복됨.</h1>
<p>print("\nHello Harry! "*3)</p>
<h1 id="출력결과-6">출력결과:</h1>
<h1 id="hello-harry-hello-harry-hello-harry---문자열이-3번-나옴.">Hello Harry! Hello Harry! Hello Harry!  # 문자열이 3번 나옴.</h1>
<h1 id="문자열-곱하기-응용-2-multistring.py">8) 문자열 곱하기 응용 2# <a href="http://multistring.py">multistring.py</a></h1>
<p>print("=" * 50)<br>
print(“My Program”)<br>
print("=" * 50)</p>
<h1 id="출력결과-프로그램을-실행시킬때-출력되는-화면-제일-위쪽에-프로그램-제목이-이처럼-표시됨.">출력결과: 프로그램을 실행시킬때 출력되는 화면 제일 위쪽에 프로그램 제목이 이처럼 표시됨.</h1>
<h1 id="section-3">==================================================</h1>
<h1 id="my-program">My Program</h1>
<h1 id="section-4">==================================================</h1>

