
마크다운이란?
====

>2004년 **존크루버**라는 사람 에게서 만들어졌으며 마크다운은 특수기호와 문자를 이용한 매우 간단한 구조의 문법을 사용하여 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있는 마크업 언어이다.

# 마크단어의 장단점
## 1.장점
```
1. 간결하다.
2. 별도의 도구없이 작성가능하다.
3. 다양한 형태로 변환이 가능하다.
4. 텍스트로 저장되기 때문에 용량이 적어 보관이 용이하다.
5. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다.
6. 지원하는 프로그램과 플랫폼이 다양하다.
```
## 2.단점
```
1. 표준이 없다.
2. 뷰어의 속도가 느리다.
3. 표준이 없기 때문에 도구에 따라서 변환방식이나 생성물이 다르다.
4. 모든 HTML 마크업을 대신하지 못한다.
```
마크타운 문법
====
1 제목
----
**입력**
```
# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
```
**출력**
># 제목 1
>## 제목 2
>### 제목 3
>#### 제목 4
>##### 제목 5
>###### 제목 6
`# 제목1 과 ## 제목2는 ===, ---로 표현할 수 있음`     

**입력**
```
제목 1
===
제목 2
---
```
**출력**

>제목 1
>===
>제목 2
>---
---

2 강조
---
**입력**
```
*강조* _강조_
**강조** __강조__
~~강조~~
```
**출력**
>*강조* _강조_   
>**강조** __강조__   
>~~강조~~

3 BlockQuote
---
**입력**
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
**출력**
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

**BlockQuote안에서는 다른 마크다운 요소를 포함할 수 있다.**
> # 제목 1
> + 목록   
> **강조**   
>    ```
>   코드블록
>   ```
4 목록
---
#### 1) 순서있는 목록
**입력**
```
1. 첫번째
3. 세번째
2. 두번째
```
**출력**
>1. 첫번째
>3. 세번째
>2. 두번째
---
*내림차순으로 정리하여 나옴*

#### 2) 순서없는 목록
**입력**
```
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
```
**출력**
>* 빨강
>  * 녹색
>   * 파랑
>
>+ 빨강
>  + 녹색
>    + 파랑
>
>- 빨강
>  - 녹색
>    - 파랑
---
*+, -, * 혼합하여사용 가능*
```
* 1단계
  - 2단계
    + 3단계
      + 4단계
```
---
* 1단계
  - 2단계
    + 3단계
      + 4단계
---
5 코드블럭
---
*1) 들여쓰기이용(tap)*   
**입력**
```
This is a normal paragraph:

    This is a code block.
    
end code block.
```
**출력**   
This is a normal paragraph:

    This is a code block.
    
end code block.

**주의**) 한 줄 이상 띄어 써야한다.

*2) ``` 이용  
**입력**
<pre>
<code>
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>
**출력**
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

*3)`<pre>,<code>{code}</code></pre>`이용*   
**입력**
```
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}

</code>
</pre>
```
**출력**
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>
6 수평선
---
**입력**
```
* * *

***

*****

- - -

---------------------------------------
```
**출력**
* * *

***

*****

- - -

---------------------------------------
7 링크
---
*1) 참조링크* 

**코드**
```
[link keyword][id]

[id]: URL "Optional Title here"
```
**입력**
```
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
```
**출력**
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
*2) 외부링크*

**코드**
```
[Title](link)
```
**입력**
```
[Google](https://google.com, "google link")
```
**출력**   
[Google](https://google.com, "google link")

8 이미지
---
**코드**
```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```