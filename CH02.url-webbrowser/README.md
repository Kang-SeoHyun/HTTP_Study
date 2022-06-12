# 🚁URI와 웹 브라우저 요청 흐름🚁

## 🏝URI🏝  
> URI (Uniform Resource Identifier)    

❓URI❓  
* Uniform: 리소스 식별하는 통일된 방식  
* Resource: 자원, URI로 식별할 수 있는 모든 것(제한 없음)  
* Identifier: 다른 항목과 구분하는데 필요한 정보

❓URI URL URN❓    
URI = URL(위치) + URN(이름)  
![image](https://user-images.githubusercontent.com/77817094/173212123-0125e9ff-4ec2-44f2-88d5-fde49b1a52a5.png)   
* URL : Uniform Resource Locator  
    * 리소스가 있는 위치를 지정  
* URN : Uniform Resource Name  
    * 리소스에 이름을 부여  
* URN 이름만으로 실제 리소스를 찾을 수 있는 방법이 보편화 되지 않음  
    * 그러한 이유로 URN은 잘 사용안함  
    ![image](https://user-images.githubusercontent.com/77817094/173212323-a0c2a421-22de-46c3-acea-363a3e83043a.png)  
    ->어떤 책의 isbn URN    

❓URL❓  
전체 문법  
![image](https://user-images.githubusercontent.com/77817094/173212402-a3a1f4f2-1419-4e2b-815b-270a4d9e6c25.png)  

* scheme  
    > 주로 프로토콜 사용
    > > 프로토콜: 어떤 방식으로 자원에 접근할 것인가 하는 약속 규칙  
    > > ex) http, https, ftp 등등  
    > > > http는 80 포트, https는 443 포트를 주로 사용, 포트는 생략 가능  
    > > >https는 http에 보안 추가 (HTTP Secure)  

* userinfo
    > 거의 사용하지 않음.  

* host
    > 호스트명 
    > > 보통 도메인명이나 ip주소 넣음

* port 
    > 생략가능
    > > 생략시 http는 80포트, https는 443포트.

* path
    > 리소스가 있는 경로, 계층적 구조
    > > ex) /home/file1.jpg

* query  
    > key = value 형태  
    > ?로 시작, &로 파라미터 추가할 수 있음.
    > > query parameter, query string 등으로 불림

* fragment  
    > 내부 북마트 등에 사용  
    > > 서버로 전송되는 정보는 아님.  

## 🏝웹 브라우저 요청 흐름🏝  

🧹웹 브라우저가 하는 일
1. DNS 서버 조회  
    ![image](https://user-images.githubusercontent.com/77817094/173214798-e24685b8-f748-41b8-88ce-5cd66e2615ca.png)  

2. HTTP 요청 메세지 생성  
    ![image](https://user-images.githubusercontent.com/77817094/173214837-a6be1f3d-cb2d-4a9d-9713-a36b472a19a4.png)  

3. HTTP 메세지 전송  
    ![image](https://user-images.githubusercontent.com/77817094/173214899-7860db8d-63ae-4068-ae04-119fa7d42cb0.png)   
    -> 전송 흐름도  
    ![image](https://user-images.githubusercontent.com/77817094/173214942-24128dfc-3c6f-4872-ab6c-f19bb83c718b.png)   
    -> 전송 데이터안에 요청 메세지 들어감  

> 이렇게 해서 웹 브라우저가 인터넷 망으로 던짐.  
> 그럼 여러 노드들을 통해서 서버에 도착을 하겠쥬?  

🧹서버가 하는 일  

4. TCP/IP 패킷 벗기고 HTTP 메세지 보고 해석함.  
    ![image](https://user-images.githubusercontent.com/77817094/173215138-ed74490f-4d13-49c2-b788-7832ad03ddf3.png)  

5. HTTP 응답 메세지 생성  
    ![image](https://user-images.githubusercontent.com/77817094/173215148-5e3f2dde-7feb-4560-bb06-054b7bcbf827.png)  
    -> '200 ok'는 정상 응답이란 뜻  

6. TCP/IP 패킷 입혀서 웹 브라우저로 다시 전달  
    ![image](https://user-images.githubusercontent.com/77817094/173215223-3e08e143-a215-4986-84ed-507a32a883cb.png)    

> 마찬가지로 웹 브라우저가 응답 패킷받으면 TCP/IP 패킷을 벗기고 전송데이터를 보겠쥬? 

🧹웹 브라우저가 하는 일  

7. HTTP 메세지 열면 응답 메세지가 있고 HTML 렌더링을 함  
    ![image](https://user-images.githubusercontent.com/77817094/173215292-ea8ed1ea-9f2a-4c3d-a9dd-1331d720b39e.png)    

8. 우리가 보는 화면    
    ![image](https://user-images.githubusercontent.com/77817094/173215338-b58f4dc7-f79b-4a42-b740-e745a45d8445.png)
