# CapstoneDesign
* 데이터 크롤링과 얼굴인식을 이용한 개인정보 영상 검출 시스템.
* [데모 발표 링크](https://youtu.be/Z-rEd8UgH2U)

## [제목/주제]
데이터 크롤링과 얼굴인식을 이용한 디지털 개인정보(성범죄) 영상 검출 시스템.

## [배경 및 문제]
- 디지털성범죄 영상물 유통사례 적발 4,584건 (2018.7.31. 방송통신위원회)
- 카메라 등을 이용 불법촬영 범죄 꾸준한 증가 (2019.12.30. 여성가족부)
(’12) 2,400건 → (’13) 4,823건 → (’14) 6,623건 → (’15) 7,623건 → (’16) 5,185건 → (’17) 6,470건
-피해를 최소화하기 위해 영상의 유출을 막기위한 빠른 조치의 필요성이 대두됨.
-피해자가 자신의 영상이 어디에 유출되었는지 직접 찾기 어려움.
<기대 효과>
1 ) 리벤지 포르노(디지털성범죄)영상 노출 이후에 빠른 후속조치가 이루어 질 수 있도록 커뮤니티, SNS에서 최대한 빠르게 본인의 얼굴 등이 노출되었다고 의심되는 영상, 사진 등을 찾을 수 있음. 
2 ) 유출에 따른 피해를 최소화하는 시스템을 개발함으로써, 개인정보의 무단 활용을 방지함. 
3 ) 궁극적으로 데이터 수집을 통한 빠른 후속 대처 및 법적 대응에 용이하게 함.

## [목표]
영상 내 얼굴과 같은 개인정보를 인식함으로써, 개인정보 유출로 인한 피해 방지 기술 연구/개발




## [팀 구성]
<소프트웨어 공학과>
팀명 : 811호
	팀 리더 : 이충헌(151779)
	팀원: 김태준(164160), 김병수(181526)

## [아키텍쳐] 
![image](https://user-images.githubusercontent.com/61380786/116859257-a6b6a380-ac3a-11eb-984e-1c1fdec75402.png)



## [요구 사항]
********* 
R001	데이터 수집	특정 사이트 크롤링.    
R002	데이터 저장	크롤링된 데이터 저장.    
R003	얼굴인식	얼굴인식 딥러닝 학습.    
R004	매칭 시스템	피해자의 데이터 매칭 및 비교    
R005	웹 클라이언트	키워드와 사진으로 검색 등 종합적으로 사용할 수 있는 시스템


### R001 데이터 수집
정의 : 사진 및 영상 데이터 수집.  
내용 : 크롤링을 통한 사진 및 영상 데이터 수집. 
  -크롤링 기법을 이용하여 개인정보 영상이 유출 되었을 거라고 예상되는 사이트에서 데이터 수집.
***********  
  

### R002 데이터 저장
정의 : 데이터 저장
내용 : 크롤링 된 데이터를 서버에 저장.
  -크롤링 된 데이터의 URL을 DB에 저장.
***********  

### R003 얼굴인식
정의 : 얼굴 인식을 위한 딥러닝 학습.
내용 : 얼굴인식 모델 학습
  -한국인 얼굴 데이터셋을 이용하여 모델을 학습시킴.
***********  
  

### R004 매칭 시스템
정의 : 피해자 이미지 매칭.
내용 : 데이터와 입력 이미지 비교.
  -학습된 AI를 이용하여 피해자의 이미지를 수집한 데이터와 비교
***********  
  


### R005 웹 클라이언트
정의 : 웹 클라이언트
내용 : 사용자가 쉽게 접근할 수 있는 UI 개발.
  -웹 서버 기반 클라이언트 개발
  

## [간트 차트]       
![image](https://user-images.githubusercontent.com/61380786/116859237-a0282c00-ac3a-11eb-9ac7-98fa21a68cfd.png)


 ## [사용 기술]
 *****
 ![image](https://user-images.githubusercontent.com/61380786/120881210-8a779f00-c60a-11eb-8e1f-16fccb962851.png)        
 ![image](https://user-images.githubusercontent.com/61380786/120881215-906d8000-c60a-11eb-9f56-f9526ce801f6.png)
 
 
## [검출 시스템 도식]
*****
![image](https://user-images.githubusercontent.com/61380786/120881461-2950cb00-c60c-11eb-914e-e8a6630abf85.png)


 
 ## [구현 결과]
 *****
 #### - 홈
 ![image](https://user-images.githubusercontent.com/61380786/120881235-ada24e80-c60a-11eb-85b5-22820c30c65a.png)
 #### - 입력
  ![image](https://user-images.githubusercontent.com/61380786/120881251-beeb5b00-c60a-11eb-9051-d11add5959f6.png)
 #### - 결과 페이지
  ![image](https://user-images.githubusercontent.com/61380786/120881244-ba26a700-c60a-11eb-80c3-50995faa143f.png)





