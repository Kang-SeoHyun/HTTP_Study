# ๐ฆ์ธํฐ๋ท ๋คํธ์ํฌ๐ฆ

## ๐์ธํฐ๋ท ํต์ ๐  
ํด๋ผ์ด์ธํธ๋ ์๋ฒ ์ฌ์ด์ ์ธํฐ๋ท(๋ง)์ด ์๋ค.  
![image](https://user-images.githubusercontent.com/77817094/173189929-45d6f0f5-2859-48b4-b7dc-1b0b43ea0391.png)  
์ด ์ธํฐ๋ท๋ง์ ํด์ณ์ ์๋ฒ๊น์ง ์ ๋๋ฌํ๋ ๋ฒ์ ์๋ ค๋ฉด IP๋ฅผ ์์์ผํจ.
> IP (Internet Protocol)  

## ๐IP๐  
ํด๋ผ์ด์ธํธ๋ ์๋ฒ๊ฐ IP์ฃผ์๋ฅผ ๋ถ์ฌ๋ฐ์์ผํ๋ค.  
IP๋ ์ง์ ํ IP์ฃผ์์ ํจํท(packet)ํํ๋ก ๋ฐ์ดํฐ๋ฅผ ์ ๋ฌํ๋ค.  
<pre>
ํจํท์๋ ์ถ๋ฐ์ฃผ์(IP address), ๋์ฐฉ์ฃผ์๋ฑ์ด ์ ์ฅ๋์ด์์.
</pre>  
IPํ๋กํ ์ฝ์ ์ํด ์ถ๋ฐ์ง์์ ๋ชฉ์ ์ง๋ก ๋ธ๋๋ค์ ํตํด์ ๋๋ฌ๋จ.  
* ํจํท ์ ๋ฌ ๊ณผ์   
![image](https://user-images.githubusercontent.com/77817094/173190097-81f6d0a8-b2b5-4c14-9c86-e64205e1ebd5.png)  
    > ์์ฒญ๊ณผ ์๋ต์ ๋ค๋ฅธ ๋ฃจํธ๋ก ์ ๋ฌ๋  ์ ์์.  

* IP ํ๋กํ ์ฝ์ ํ๊ณ  
![image](https://user-images.githubusercontent.com/77817094/173190176-f7c630c7-394b-426f-8680-546dbfe6de57.png)    
    > ํจํท์ ๋ฃ์ด์ผ๋๋ ๋ฐ์ดํฐ ์์ด ๋๋ฌด ํฌ๋ฉด ๋์ด์ ๋ณด๋ด๋๋ฐ ํจํท๋ค์ด ๋ค๋ฅธ ๋ธ๋๋ฅผ ํ๋ฉด ์์๋๋ก ์์ค๊ณ  ๋ฉ๋๋ก ์ฌ ์๋ ์๋ค. 
    ๊ฒ์ํ๋ฉด์ ๋ธ๋๋ ๋ฃ๊ณ  ๊ทธ๋ฌ๋ฉด ๊ตฌ๋ณ์ ์ด๋ป๊ฒ ํ๋์ง? 

โผ ๋ฐ๋ผ์ IP๋ง์ผ๋ก๋ ์ด๋ฌํ ๋ฌธ์ ๋ค์ ํด๊ฒฐํ  ์ ์๋ค ๋ฐ๋ผ์ ์ด๋ฅผ ์ํด TCP๊ฐ ๋์๋ค.  

## ๐TCP, UDP๐  
> TCP (Transmission Control Protocol)  
> UDP (User Datagram Protocol)  

์ธํฐ๋ท ํ๋กํ ์ฝ ์คํ์ 4๊ณ์ธต  
|๊ณ์ธต|์ข๋ฅ|
|------|---|
|์ดํ๋ฆฌ์ผ์ด์ ๊ณ์ธต|HTTP, FTP|
|์ ์ก ๊ณ์ธต|TCP, UDP|
|์ธํฐ๋ท ๊ณ์ธต|IP|
|๋คํธ์ํฌ ์ธํฐํ์ด์ค ๊ณ์ธต|LAN ์ฅ๋น|  

ํ๋กํ ์ฝ ๊ณ์ธต  
![image](https://user-images.githubusercontent.com/77817094/173210414-d7df2037-04c9-46f4-8241-7fd84ca27ec8.png)  
-> ethernet frame์๋ mac์ฃผ์๊ฐ์ ๋ฌผ๋ฆฌ์ ์ธ ์ฃผ์๊ฐ ํฌํจ๋์ด ์์.

* IP ํจํท ์ ๋ณด   
![image](https://user-images.githubusercontent.com/77817094/173210562-0a123b9d-22e0-4e40-92c5-183b796f339f.png)   
* TCP/IP ํจํท ์ ๋ณด   
![image](https://user-images.githubusercontent.com/77817094/173210567-aa0e9c99-353e-4833-b1a4-a5a653c34c11.png)   
> ์ ์ก ์ ์ด, ์์ ๋ฑ๊ณผ ๊ด๋ จ๋ ์ ๋ณด๋ฅผ ์ถ๊ฐํจ์ผ๋ก์ IP์ ๋ฌธ์ ๋ค์ ๋ณด์ ํ  ์ ์๋ค.  

โTCP๋โ  
์ ์ก ์ ์ด ํ๋กํ ์ฝ๋ก ํ์ฌ ๋๋ถ๋ถ ์ฌ์ฉํ๋ค. 
1. ์ฐ๊ฒฐ์งํฅ (TCP 3 way handshake)  
    > ์ฐ๊ฒฐ์ ํ๊ณ  ๋ฉ์ธ์ง ๋ณด๋.  
2. ๋ฐ์ดํฐ ์ ๋ฌ ๋ณด์ฆ  
    > ์๋ฒ์์ ๋ฐ์ดํฐ ์ ๋ฐ์ผ๋ฉด ํด๋ผ์ด์ธํธํํ ์๋ตํจ.
3. ์์ ๋ณด์ฅ
    > 1,2,3 ์ผ๋ก ๋ณด๋๋๋ฐ 1,3,2๋ก ๋์ฐฉํ๋ฉด ๋๋ผ์ด๋ฒ์์ ์ต์ ํํ๋์ง 3๋ฒ(์๋ชป๋ ๋ถ๋ถ)๋ถํฐ ๋ค ๋ฒ๋ฆฌ๊ณ  ํด๋ผ์ด์ธํธํํ 2๋ฒ๋ถํฐ ๋ค์๋ณด๋ด๋ผํจ.

* TCP 3 way handshake  
    ![image](https://user-images.githubusercontent.com/77817094/173210742-31fe2851-722e-4a0c-bd80-991fe556bc66.png)   
    1. ํด - ๋ฉ์ธ์ง๋ณด๋(syn)
    2. ์ - ์๊ฒ ์ด(ack) ๋ฉ์ธ์ง๋ณด๋(syn)
    3. ํด - ์๊ฒ ์ด(ack)   
    -> ์์๋ 3๋ฒ ack์ ํจ๊ป ๋ฐ์ดํฐ ์ ์กํจ.  

โUDP๋โ  
TCP์ 1,2,3 ๊ธฐ๋ฅ ์์ ๋์  ๋จ์ํ๊ณ  ๋น ๋ฆ.  
๋ฐฑ์ง์ํ์ด๋ฏ๋ก ํ์ํ๋ฉด UDP ํ๋กํ ์ฝ ์์ ์ ํ๋ฆฌ์ผ์ด์์์ ๊ธฐ๋ฅ์ ํ์ฅํด ๋ณผ ์ ์๋ค.  

๋ฐฑ์ง?
<pre>
IP์ PORT๋ ์ฒดํฌ์ฌ ์ ๋๊ฐ ์ถ๊ฐ๋ ์ ๋.  
* PORT: ํ๋์ IP์์ ์ฌ๋ฌ ์ ํ๋ฆฌ์ผ์ด์์ด ์๋๋  ๋ ํ๋ก๊ทธ๋จ์ ๊ตฌ๋ถํ๊ธฐ ์ํด ์ฌ์ฉ  
* ์ฒดํฌ์ฌ:  ๋ฉ์ธ์ง์ ๋ํด์ ๋ง๋์ง ๊ฒ์ฆ ํด์ฃผ๋ ๋ฐ์ดํฐ
</pre>

UDP ์ฐ๋ ์ด์ ?  
<pre>
TCP๋ ์ ๋ขฐํ  ์ ์์ง๋ง ์ฉ๋์ด ์ปค์ ๋ ๋๋ฆผ.  
๊ทผ๋ฐ ์ด๋ฏธ TCP๊ฐ ์ ๋ น์ ํด๋ฒ๋ ค์ ๋ฐ๊พธ๊ธฐ ์ด๋ ค์.  
๊ทธ๋์ UDP์ ์์ ๋์ ์ต์ ํ ํ๋ ํ์.  
๊ทผ๋ฐ ์๋๊ฐ ๋ฐ๋๋ฉด์ UDP๋ง์ด ์. (HTTP3์์ UDP์)
</pre>

## ๐PORT๐  
์ถ๋ฐ, ๋์ฐฉ์ง ์ฃผ์ : IP - ์ํํธ  
์ถ๋ฐ, ๋์ฐฉ์ง ์ดํ๋ฆฌ์ผ์ด์ ๊ตฌ๋ถ : port - ๋ช๋ ๋ชํธ  
* ๊ตฌ๋ถํ๋ ๋ฐฉ๋ฒ  
![image](https://user-images.githubusercontent.com/77817094/173211354-90dc3aaa-7137-466e-9a41-0aa4724f9dd3.png)  
    -> ํ์ ๋ฐ์ค๊ฐ port์.  

* PORT ํ ๋น์ ์ฃผ์ํ  ์   
![image](https://user-images.githubusercontent.com/77817094/173211403-2ec12f9e-8b62-41c3-a519-70c7ac9cff86.png)    

## ๐DNS๐
> DNS (Domain Name System)  

![image](https://user-images.githubusercontent.com/77817094/173211657-cd82bf80-03ab-4c30-8ceb-1556f1162d53.png)  

* DNS๊ฐ ํ๋์ผ  
   DNS ์๋ฒ์ ๋๋ฉ์ธ ๋ช์ ์ ์ฅํด ๋ ์ ์์. (Like ์ ํ๋ฒํธ๋ถ)  

* DNS๊ฐ ํ์ํ ์ด์   
   IP๋ ๊ธฐ์ตํ๊ธฐ๋ ์ด๋ ต๊ณ  ๋ณ๊ฒฝ๋  ์ ์๋ค.  
