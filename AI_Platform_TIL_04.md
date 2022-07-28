# AI_Platform_TIL_04





음성 변환 서비스2 : 텍스트 -> 음성

- 서비스 신청 : CLOVA Voice - Premium



1. API 호출 결과 출력 : Text to Speech

   - TTSService 서비스 클래스 생성
   - tts() : 메소드 추가
     - API 코드 복사
       - 텍스트를 서버에 전송하고 음성 파일 반환 받음 (.mp3 로 저장)
       - Client ID
       - Client Secret
   - 컨트롤러에 추가 : ttsService 객체 사용 
     - /tts
   - index.jsp에 추가
   - 저장된 mp3 파일 위치 확인 / 플레이 확인

   

2. 파일 업로드 / 결과 mp3 플레이

   - @RestController에 추가
   - tts.js / Ajax 사용
   - ttsResult.jsp
   - 파일 업로드 기능 추가
   - 결과 mp3 파일을 `<audio>` 태그로 플레이

3. 

   

### Chatbot

- 시나리오 작성
  - 독서 모임 시나리오
  
  - 주최 : 북클럽 멀티
  
  - 일자 : 2022-08-06 토요일
  
  - 시간 : 15 : 00 ~ 17 : 00
  
  - 소요 시간 : 2시간
  
  - 장소 : 멀티캠퍼스 본관 504호
  
  - 대상 도서 : 지구의 눈물
  
  - 참가비 : 5,000 원 (음료)
  
  - 찾아 오는 길 : 이미지
  
  - 주차 안내 : 이미지
  
  - 문의 : 010-1234-1234
  
  - 이메일 : book@multi.com
  
  - 신청 : https://www.multicampus.com/kr/index
  
    

2. JSON 파싱

   - jsonToString() 메소드 추가
   - 응답 메시지 추출 / 출력

3. 뷰 페이지에서 입력 / 출력 

   - AIRestController / Ajax

   - chatbot.js

   - chatResult.jsp 생성 

     - `<div = "resultBox">` : 답변 출력
     - 폼 
       - 질문 입력

   - 컨트롤러 변경

   - index 변경

     