# ๐URI์ ์น ๋ธ๋ผ์ฐ์  ์์ฒญ ํ๋ฆ๐

## ๐URI๐  
> URI (Uniform Resource Identifier)    

โURIโ  
* Uniform: ๋ฆฌ์์ค ์๋ณํ๋ ํต์ผ๋ ๋ฐฉ์  
* Resource: ์์, URI๋ก ์๋ณํ  ์ ์๋ ๋ชจ๋  ๊ฒ(์ ํ ์์)  
* Identifier: ๋ค๋ฅธ ํญ๋ชฉ๊ณผ ๊ตฌ๋ถํ๋๋ฐ ํ์ํ ์ ๋ณด

โURI URL URNโ    
URI = URL(์์น) + URN(์ด๋ฆ)  
![image](https://user-images.githubusercontent.com/77817094/173212123-0125e9ff-4ec2-44f2-88d5-fde49b1a52a5.png)   
* URL : Uniform Resource Locator  
    * ๋ฆฌ์์ค๊ฐ ์๋ ์์น๋ฅผ ์ง์   
* URN : Uniform Resource Name  
    * ๋ฆฌ์์ค์ ์ด๋ฆ์ ๋ถ์ฌ  
* URN ์ด๋ฆ๋ง์ผ๋ก ์ค์  ๋ฆฌ์์ค๋ฅผ ์ฐพ์ ์ ์๋ ๋ฐฉ๋ฒ์ด ๋ณดํธํ ๋์ง ์์  
    * ๊ทธ๋ฌํ ์ด์ ๋ก URN์ ์ ์ฌ์ฉ์ํจ  
    ![image](https://user-images.githubusercontent.com/77817094/173212323-a0c2a421-22de-46c3-acea-363a3e83043a.png)  
    ->์ด๋ค ์ฑ์ isbn URN    

โURLโ  
์ ์ฒด ๋ฌธ๋ฒ  
![image](https://user-images.githubusercontent.com/77817094/173212402-a3a1f4f2-1419-4e2b-815b-270a4d9e6c25.png)  

* scheme  
    > ์ฃผ๋ก ํ๋กํ ์ฝ ์ฌ์ฉ
    > > ํ๋กํ ์ฝ: ์ด๋ค ๋ฐฉ์์ผ๋ก ์์์ ์ ๊ทผํ  ๊ฒ์ธ๊ฐ ํ๋ ์ฝ์ ๊ท์น  
    > > ex) http, https, ftp ๋ฑ๋ฑ  
    > > > http๋ 80 ํฌํธ, https๋ 443 ํฌํธ๋ฅผ ์ฃผ๋ก ์ฌ์ฉ, ํฌํธ๋ ์๋ต ๊ฐ๋ฅ  
    > > >https๋ http์ ๋ณด์ ์ถ๊ฐ (HTTP Secure)  

* userinfo
    > ๊ฑฐ์ ์ฌ์ฉํ์ง ์์.  

* host
    > ํธ์คํธ๋ช 
    > > ๋ณดํต ๋๋ฉ์ธ๋ช์ด๋ ip์ฃผ์ ๋ฃ์

* port 
    > ์๋ต๊ฐ๋ฅ
    > > ์๋ต์ http๋ 80ํฌํธ, https๋ 443ํฌํธ.

* path
    > ๋ฆฌ์์ค๊ฐ ์๋ ๊ฒฝ๋ก, ๊ณ์ธต์  ๊ตฌ์กฐ
    > > ex) /home/file1.jpg

* query  
    > key = value ํํ  
    > ?๋ก ์์, &๋ก ํ๋ผ๋ฏธํฐ ์ถ๊ฐํ  ์ ์์.
    > > query parameter, query string ๋ฑ์ผ๋ก ๋ถ๋ฆผ

* fragment  
    > ๋ด๋ถ ๋ถ๋งํธ ๋ฑ์ ์ฌ์ฉ  
    > > ์๋ฒ๋ก ์ ์ก๋๋ ์ ๋ณด๋ ์๋.  

## ๐์น ๋ธ๋ผ์ฐ์  ์์ฒญ ํ๋ฆ๐  

๐งน์น ๋ธ๋ผ์ฐ์ ๊ฐ ํ๋ ์ผ
1. DNS ์๋ฒ ์กฐํ  
    ![image](https://user-images.githubusercontent.com/77817094/173214798-e24685b8-f748-41b8-88ce-5cd66e2615ca.png)  

2. HTTP ์์ฒญ ๋ฉ์ธ์ง ์์ฑ  
    ![image](https://user-images.githubusercontent.com/77817094/173214837-a6be1f3d-cb2d-4a9d-9713-a36b472a19a4.png)  

3. HTTP ๋ฉ์ธ์ง ์ ์ก  
    ![image](https://user-images.githubusercontent.com/77817094/173214899-7860db8d-63ae-4068-ae04-119fa7d42cb0.png)   
    -> ์ ์ก ํ๋ฆ๋  
    ![image](https://user-images.githubusercontent.com/77817094/173214942-24128dfc-3c6f-4872-ab6c-f19bb83c718b.png)   
    -> ์ ์ก ๋ฐ์ดํฐ์์ ์์ฒญ ๋ฉ์ธ์ง ๋ค์ด๊ฐ  

> ์ด๋ ๊ฒ ํด์ ์น ๋ธ๋ผ์ฐ์ ๊ฐ ์ธํฐ๋ท ๋ง์ผ๋ก ๋์ง.  
> ๊ทธ๋ผ ์ฌ๋ฌ ๋ธ๋๋ค์ ํตํด์ ์๋ฒ์ ๋์ฐฉ์ ํ๊ฒ ์ฅฌ?  

๐งน์๋ฒ๊ฐ ํ๋ ์ผ  

4. TCP/IP ํจํท ๋ฒ๊ธฐ๊ณ  HTTP ๋ฉ์ธ์ง ๋ณด๊ณ  ํด์ํจ.  
    ![image](https://user-images.githubusercontent.com/77817094/173215138-ed74490f-4d13-49c2-b788-7832ad03ddf3.png)  

5. HTTP ์๋ต ๋ฉ์ธ์ง ์์ฑ  
    ![image](https://user-images.githubusercontent.com/77817094/173215148-5e3f2dde-7feb-4560-bb06-054b7bcbf827.png)  
    -> '200 ok'๋ ์ ์ ์๋ต์ด๋ ๋ป  

6. TCP/IP ํจํท ์ํ์ ์น ๋ธ๋ผ์ฐ์ ๋ก ๋ค์ ์ ๋ฌ  
    ![image](https://user-images.githubusercontent.com/77817094/173215223-3e08e143-a215-4986-84ed-507a32a883cb.png)    

> ๋ง์ฐฌ๊ฐ์ง๋ก ์น ๋ธ๋ผ์ฐ์ ๊ฐ ์๋ต ํจํท๋ฐ์ผ๋ฉด TCP/IP ํจํท์ ๋ฒ๊ธฐ๊ณ  ์ ์ก๋ฐ์ดํฐ๋ฅผ ๋ณด๊ฒ ์ฅฌ? 

๐งน์น ๋ธ๋ผ์ฐ์ ๊ฐ ํ๋ ์ผ  

7. HTTP ์๋ต ๋ฉ์ธ์ง ํด์์ ํด์ HTML ๋ ๋๋ง์ ํจ  
    ![image](https://user-images.githubusercontent.com/77817094/173215292-ea8ed1ea-9f2a-4c3d-a9dd-1331d720b39e.png)    

8. ์ฐ๋ฆฌ๊ฐ ๋ณด๋ ํ๋ฉด    
    ![image](https://user-images.githubusercontent.com/77817094/173215338-b58f4dc7-f79b-4a42-b740-e745a45d8445.png)
