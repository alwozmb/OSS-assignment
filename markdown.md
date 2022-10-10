# 1. 마크다운(Markdown) 태그
## 1-1. 마크다운(Markdown) 태그

### 마크다운이란?
마크다운(markdown)은 일반 텍스트 기반의 경량 마크업 언어다. 일반 텍스트 서식이 있는 문서를 작성하는 데 사용되며, 일반 마크업 언어에 비해 문법이 쉽고 간단한 것이 특징이다. HTML과 리치 텍스트(RTF) 등 서식 문서로 쉽게 변환되기 때문에 응용 소프트웨어와 함께 배포되는 README.md 파일이나 온라인 게시물 등에 많이 사용된다.

### 마크다운 에디터
윈도우 메모장도 상관없으나 보다 사용이 직관적인 깃헙(Github), 비트버킷(Bitbucket), 워드프레스, 슬랙(Slack), 트렐로(Trello) 등의 서비스에서 작성할 수 있다.


# 2. 마크다운(Markdown) 문법
## 2-1. 헤더
'#'의 개수에 따라 h1부터 h6까지 헤더의 크기를 표현할 수 있다.
```
# 헤더 크기 (h1)
## 헤더 크기 (h2)
### 헤더 크기 (h3)
#### 헤더 크기 (h4)
##### 헤더 크기 (h5)
###### 헤더 크기 (h6)
```
![헤더 크기](https://user-images.githubusercontent.com/110728160/194856071-38a87af2-1923-4f58-bcf0-daf8cfd20f3f.png)


## 2-2. 글씨 모양
'*'의 개수와 '~'의 사용에 따라 글씨 모양을 표현할 수 있다.
```
It is *Italic*
It is **bold**
It is ***Italic and bold***   
It is ~~canceled~~ 
```
It is *Italic*   
It is **bold**   
It is ***Italic and bold***      
It is ~~canceled~~    


## 2-3. 인용문
'>'으로 인용문을 표현해 줄 수 있다.
```
> 1번 인용문
>> 2번 인용문
>>> 3번 인용문
```
> 1번 인용문
>> 2번 인용문
>>> 3번 인용문


## 2-4. 목록
* **숫자가 없는 리스트**를 작성할 땐 아래처럼 **띄어쓰기 두 칸 혹은 Tab 키**를 사용하여 표현한다.
```
* 구매 목록
  * 음식
    * 치킨
    * 피자
    * 떡볶이
  * 책
```
* 구매 목록
  * 음식
    * 치킨
    * 피자
    * 떡볶이
  * 책

* **숫자가 있는(순서가 있는) 리스트**를 작성할 땐 **Tab + 숫자 키**를 사용하여 표현한다. 
```
* 계란찜 만드는 법
  1. 계란 풀기
  100. 물과 소금 넣기 //중간에 순서에 맞지 않는 숫자를 넣더라도 순서대로 표시된다.
  3. 전자레인지에 3분
```
* 계란찜 만드는 법
  1. 계란 풀기
  100. 물과 소금 넣기
  3. 전자레인지에 3분


## 2-5. 코드블럭
백틱(`) 세 개를 위아래로 사용하여 코드블럭을 만들 수 있다.

``` Java
System.out.println("Hello, World!");
```
![image](https://user-images.githubusercontent.com/110728160/194866439-68fda398-e11c-4c92-a85e-1caf6684ce81.png)


## 2-6. 링크
```
[경로 설명](주소)로 링크를 첨부할 수 있다.
[naver](www.naver.com)
[my_github](https://github.com/alwozmb)
```
[naver](www.naver.com) // 클릭하면 네이버로 이동      
[my_github](https://github.com/alwozmb) // 클릭하면 내 깃허브 주소로 이동


## 2-7. 이미지
```
'![이미지 설명](경로)'로 이미지를 첨부할 수 있다.
![깃허브로고](https://user-images.githubusercontent.com/110728160/194865498-a78c340f-970f-4228-8e09-5e16d33cfbe2.png)
```
![깃허브로고](https://user-images.githubusercontent.com/110728160/194865498-a78c340f-970f-4228-8e09-5e16d33cfbe2.png)
