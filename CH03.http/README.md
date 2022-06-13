# 🐱‍🏍HTTP 기본🐱‍🏍

## 🤖모든 것이 HTTP🤖
> HTTP (HyperText Transfer Protocol)

* 지금은 HTTP 시대
    * 이미지, 음성, 영상, Json등등 거의 모든 형태의 데이터가 전송 가능하다.  
    * 심지어 서버간에 데이터를 주고 받을 때도 대부분 HTTP 사용.

* HTTP 역사
    * HTTP/0.9, 1.0 있음  
    * HTTP/1.1 1997년: 가장 많이 사용. 우리에게 가장 중요.  
    * 그 이후는 그냥 성능 개선 하는 정도.

* 기반 프로토콜  
    * TCP : HTTP/1.1, 2  
    * UDP : HTTP/3  
    * TCP가 안정적이지만 속도가 빠른 메커니즘은 아니기때문에 HTTP/3가 나옴.
    
> 확인하는 방법: 브라우저 들어가서 F12입력 -> network에서  
> name에 오른쪽마우스 입력해서 protocol 추가해주면 나옴.  
네이버:  
![image](https://user-images.githubusercontent.com/77817094/173282852-b2924ccb-110c-4f4b-9452-d51bc4a31e5a.png)  
구글:  
![image](https://user-images.githubusercontent.com/77817094/173283158-808e57c6-4dbb-4507-a2fe-a253adfbd0a2.png)  
> > HTTP/2, HTTP/3가 강의 촬영 날 기준보다 더 증가, 발전한 것을 확인 할 수 있다.

* HTTP 특징
    * 클라이언트 서버 구조  
    * 무상태 프로토콜(스테이스리스), 비연결  
    * HTTP 메세지를 통해서 통신  
    * 단순함, 확장 가능    
    * 👇🏻아래에서 자세히👇🏻


## 🤖클라이언트 서버 구조🤖

* 클라이언트 서버 표면적 구조  
    ![image](https://user-images.githubusercontent.com/77817094/173283864-7848df63-8125-4b8b-9a11-d3335f4619af.png)  

* 클라이언트와 서버의 분리.
    <pre>
  * 클라이언트는 사용성, UI에 집중시킴.   
  * 서버는 비지니스 로직이나 데이터를 처리하는 것에 집중시킴.  
  -> 클라이언트랑 서버가 독립적으로 진화할 수 있음. </pre>

## 🤖Stateful, Stateless🤖
