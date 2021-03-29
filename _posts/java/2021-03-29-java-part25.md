---


---

<h2 id="객체지향-프로그래밍-object-oriented">[객체지향 프로그래밍] (Object Oriented)</h2>
<h5 id="클래스의-생성자constructor">클래스의 생성자(Constructor)</h5>
<p><em>Animal.java</em></p>
<pre><code>public class Animal {
    String name;

    public void setName(String name) {
        this.name = name;
    }
}
</code></pre>
<p><em>Dog.java</em></p>
<pre><code>public class Dog extends Animal {
    public void sleep() {
        System.out.println(this.name+" zzz");
    }
}
</code></pre>
<p><em>HouseDog.java</em></p>
<pre><code>public class HouseDog extends Dog {
    public void sleep() {
        System.out.println(this.name+" zzz in house");
    } 

    public void sleep(int hour) {
        System.out.println(this.name+" zzz in house for " + hour + " hours");
    } 

    public static void main(String[] args) {
        HouseDog houseDog = new HouseDog();
        houseDog.setName("happy");
        houseDog.sleep();
        houseDog.sleep(3);
    }
}
</code></pre>
<p>HouseDog클래스의 main메소드를 다음처럼 수정 후 실행</p>
<pre><code>    public static void main(String[] args) {
        HouseDog dog = new HouseDog();
        System.out.println(dog.name);
    }
</code></pre>
<p>name객체변수에 아무값도 설정하지 않았기때문에 null출력</p>
<p>HouseDog클래스는 코딩하기에 따라 객체변수 name에 값을 설정할 수도, 안할 수도 있다. 그렇다면 name객체변수에 값을 무조건 설정해야만 객체가 생성될 수 있도록 강제할 수 있는 방법은?<br>
<strong>생성자(Constructor)</strong> 이용</p>
<p>클래스 가장 상단에 다음 메소드 추가</p>
<pre><code>    public HouseDog(String name) {
        this.setName(name);
    } 
</code></pre>
<p>위 메소드처럼 메소드명이 클래스명과 동일하고 리턴 자료형이 없는 메소드가 <code>생성자(Constructor)</code></p>
<p><em>생성자의 규칙</em></p>
<ol>
<li>클래스명과 메소드명 동일</li>
<li>리턴타입을 정의하지 않는다</li>
</ol>
<p>생성자는 객체가 생성될때 호출<br>
객체가 생성될때는 new키워드로 객체가 만들어질 때<br>
즉, 생성자는 다음과 같이 new키워드가 사용될 때 호출</p>
<pre><code>new 클래스명(입력항목, ...)
</code></pre>
<p>생성자는 메소드와 마찬가지로 입력을 받을 수 있다</p>
<p>우리가 만든 생성자는 다음과 같이 입력값으로 문자열을 필요로 하는 생성자</p>
<pre><code>public HouseDog(String name) {
    this.setName(name);
} 
</code></pre>
<p>다음과 같이 new 키워드로 객체를 만들때 문자열을 전달해야만 한다</p>
<pre><code>HouseDog dog = new HouseDog("happy");  
// 생성자 호출 시 문자열을 전달해야 한다
</code></pre>
<p>만약 다음처럼 코딩시 컴파일 오류발생</p>
<pre><code>HouseDog dog = new HouseDog();
</code></pre>
<p>오류발생 이유는 객체 생성방법이 생성자의 규칙과 맞지않기 때문. 생성자가 선언된 경우 생성자의 규칙대로만 객체를 생성할 수 있다</p>
<p>다음은 생성자가 적용된 완성된 HouseDog클래스</p>
<pre><code>public class HouseDog extends Dog {
    public HouseDog(String name) {
        this.setName(name);
    } 

    public void sleep() {
        System.out.println(this.name+" zzz in house");
    } 

    public void sleep(int hour) {
        System.out.println(this.name+" zzz in house for " + hour + " hours");
    } 

    public static void main(String[] args) {
        HouseDog dog = new HouseDog("happy");
        System.out.println(dog.name);
    }
}
</code></pre>
<p>결과:</p>
<pre><code>happy
</code></pre>
<p>이렇듯 생성자 사용시 이득은  <code>setName("happy")</code>같은 필수적인 행동을 객체생성시 제어할 수 있게 된다</p>
<h3 id="default-생성자">default 생성자</h3>
<pre><code>public class Dog extends Animal {
    public void sleep() {
        System.out.println(this.name + " zzz");
    }
}
</code></pre>
<pre><code>public class Dog extends Animal {
    public Dog() {
    }

    public void sleep() {
        System.out.println(this.name + " zzz");
    }
}
</code></pre>
<p>첫번 째 코드와 두번 째 코드의 차이점은? 두번째 코드는 생성자가 구현. 생성자의 입력항목이 없고 생성자 내부에 아무내용이 없는 위같은 생성자가 default 생성자</p>
<p>위같은 디폴트 생성자 구현시  <code>new Dog()</code>로 Dog객체가 만들어 질때 위 디폴트 생성자 실행</p>
<p>만약 클래스에 생성자가 없다면 컴파일러는 자동으로 위와같은 디폴트 생성자를 추가. 하지만 사용자가 작성한 생성자가 하나라도 구현되어 있다면 컴파일러는 디폴트 생성자를 추가하지 않는다</p>
<p>※ 이러한 이유로 위에서 살펴본 HouseDog클래스에 name을 입력으로 받는 생성자를 만든 후  <code>new HouseDog()</code>는 사용할 수 없게 되는 것(HouseDog클래스에 이미 생성자를 만들었기 때문에 컴파일러는 디폴트 생성자를 자동으로 추가하지 않는다)</p>
<h3 id="생성자-오버로딩">생성자 오버로딩</h3>
<p>하나의 클래스에 여러 입력항목이 다른 생성자를 만들 수 있다<br>
즉, 다음 같은 것이 가능</p>
<pre><code>public class HouseDog extends Dog {
    public HouseDog(String name) {
        this.setName(name);
    }

    public HouseDog(int type) {
        if (type == 1) {
            this.setName("yorkshire");
        } else if (type == 2) {
            this.setName("bulldog");
        }
    }

    public void sleep() {
        System.out.println(this.name+" zzz in house");
    } 

    public void sleep(int hour) {
        System.out.println(this.name+" zzz in house for " + hour + " hours");
    } 

    public static void main(String[] args) {
        HouseDog happy = new HouseDog("happy");
        HouseDog yorkshire = new HouseDog(1);
        System.out.println(happy.name);
        System.out.println(yorkshire.name);
    }
}
</code></pre>
<p>위 HouseDog클래스는 두 생성자가 구현되어 있다<br>
String자료형을 입력으로 받는 생성자, int자료형을 입력으로 받는 생성자<br>
두 생성자 차이는 입력항목으로 입력항목이 다른 생성자를 여러개 만들 수 있는데 이를 생성자 오버로딩(Overloading)이라 한다 (※ 메소드 오버로딩과 마찬가지 개념)</p>
<p>이제 HouseDog객체는 다음 같이 두 방법으로 생성가능</p>
<pre><code>HouseDog happy = new HouseDog("happy");
HouseDog yorkshire = new HouseDog(1);
</code></pre>
<p>결과:</p>
<pre><code>happy
yorkshire
</code></pre>

