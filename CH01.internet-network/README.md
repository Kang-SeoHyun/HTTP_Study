# 🍦인터넷 네트워크🍦

## 🍑인터넷 통신🍑  
클라이언트랑 서버 사이에 인터넷(망)이 있다.  
![image](https://user-images.githubusercontent.com/77817094/173189929-45d6f0f5-2859-48b4-b7dc-1b0b43ea0391.png)  
이 인터넷망을 해쳐서 서버까지 잘 도달하는 법을 알려면 IP를 알아야함.
> IP (Internet Protocol)  

## 🍑IP🍑  
클라이언트랑 서버가 IP주소를 부여받아야한다.  
IP는 지정한 IP주소에 패킷(packet)형태로 데이터를 전달한다.  
<pre>
패킷에는 출발주소(IP address), 도착주소등이 저장되어있음.
</pre>  
IP프로토콜에 의해 출발지에서 목적지로 노드들을 통해서 도달됨.  
* 패킷 전달 과정  
![image](https://user-images.githubusercontent.com/77817094/173190097-81f6d0a8-b2b5-4c14-9c86-e64205e1ebd5.png)  
요청과 응답은 다른 루트로 전달될 수 있음.  

* IP 프로토콜의 한계  
![image](https://user-images.githubusercontent.com/77817094/173190176-f7c630c7-394b-426f-8680-546dbfe6de57.png)    
    > 패킷에 넣어야되는 데이터 양이 너무 크면 끊어서 보내는데 패킷들이 다른 노드를 타면 순서대로 안오고 멋대로 올 수도 있다. 
    게임하면서 노래도 듣고 그러면 구별을 어떻게 하는지? 

‼ 따라서 IP만으로는 이러한 문제들을 해결할 수 없다 따라서 이를 위해 TCP가 나왔다.  

## 🍑TCP, UDP🍑  
> TCP (Transmission Control Protocol)  
> UDP (User Datagram Protocol)  

인터넷 프로토콜 스택의 4계층  
|계층|종류|
|------|---|
|어플리케이션 계층|HTTP, FTP|
|전송 계층|TCP, UDP|
|인터넷 계층|IP|
|네트워크 인터페이스 계층|LAN 장비|  

프로토콜 계층  
![image](https://user-images.githubusercontent.com/77817094/173210414-d7df2037-04c9-46f4-8241-7fd84ca27ec8.png)
-> ethernet frame에는 mac주소같은 물리적인 주소가 포함되어 있음.

* IP 패킷 정보  
![image](https://user-images.githubusercontent.com/77817094/173210562-0a123b9d-22e0-4e40-92c5-183b796f339f.png)  
* TCP/IP 패킷 정보  
![image](https://user-images.githubusercontent.com/77817094/173210567-aa0e9c99-353e-4833-b1a4-a5a653c34c11.png)  
> 전송 제어, 순서 등과 관련된 정보를 추가함으로서 IP의 문제들을 보완 할 수 있다.  

❓TCP란❓  
전송 제어 프로토콜로 현재 대부분 사용한다. 
1. 연결지향 (TCP 3 way handshake)  
    > 연결을 하고 메세지 보냄.  
2. 데이터 전달 보증  
    > 서버에서 데이터 잘 받으면 클라이언트한테 응답함.
3. 순서 보장
    > 1,2,3 으로 보냈는데 1,3,2로 도착하면 드라이버에서 최적화하던지 3번(잘못된 부분)부터 다 버리고 클라이언트한테 2번부터 다시보내라함.

* TCP 3 way handshake
    ![image](https://user-images.githubusercontent.com/77817094/173210742-31fe2851-722e-4a0c-bd80-991fe556bc66.png)  
    1. 클 - 메세지보냄(syn)
    2. 서 - 알겠어(ack) 메세지보냄(syn)
    3. 클 - 알겠어(ack)  
    -> 요새는 3번 ack와 함께 데이터 전송함.  

❓UDP란❓  
TCP의 1,2,3 기능 없음 대신 단순하고 빠름.  
백지상태이므로 필요하면 UDP 프로토콜 위의 애플리케이션에서 기능을 확장해 볼 수 있다.  

백지?
<pre>
IP에 PORT랑 체크섬 정도가 추가된 정도.  
* PORT: 하나의 IP에서 여러 어플리케이션이 작동될 때 프로그램을 구분하기 위해 사용됨.  
* 체크섬:  메세지에 대해서 맞는지 검증 해주는 데이터
</pre>

UDP 쓰는 이유?  
<pre>
TCP는 신뢰할 수 있지만 용량이 커서 넘 느림. 근데 이미 TCP가 점령을 해버려서 바꾸기 어려움. 그래서 UDP에 손을 대서 최적화 하는 형식. 근데 시대가 바뀌면서 UDP많이 씀. (HTTP3에서 UDP씀)
</pre>

## 🍑PORT🍑  
출발, 도착지 주소 : IP - 아파트  
출발, 도착지 어플리케이션 구분 : port - 몇동 몇호  
![image](https://user-images.githubusercontent.com/77817094/173211354-90dc3aaa-7137-466e-9a41-0aa4724f9dd3.png)
-> 회색 박스가 port임.  

* PORT 할당시 주의할 점 
![image](https://user-images.githubusercontent.com/77817094/173211403-2ec12f9e-8b62-41c3-a519-70c7ac9cff86.png)  

## 🍑DNS🍑
> DNS (Domain Name System)  

![image](https://user-images.githubusercontent.com/77817094/173211657-cd82bf80-03ab-4c30-8ceb-1556f1162d53.png)  

* DNS가 하는일  
    DNS 서버에 도메인 명을 저장해 둘 수 있음. (Like 전화번호부)  

* DNS가 필요한 이유  
    IP는 기억하기도 어렵고 변경될 수 있다.  