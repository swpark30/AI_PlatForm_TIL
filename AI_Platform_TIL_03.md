# AI_Platform_TIL_03







## CLOVA OCR

- Optical Character Recognition : 광학 문자 인식
- 이미지 속 글자 위치를 찾고 어떤 글자인지 자동으로 알아내는 기술
- 글자 영역 검출 및 인식 기술
- 방법1
  - 지정된 형식 없이 이미지에서 텍스트 추출
- 방법2
  - 템플릿을 만들고 원하는 영역을 지정한 뒤, 필요한 글자만 빠르게 추출하는 기능
    - 예 : 영수증

- API 사용 방법

  - 이미지 파일 전송하고 텍스트 반환 받아서 JSON 파싱해서 사용

- 일반적인 활용 사례

  - 문서파일 / 인쇄물 판독

  - 우편번호 추출을 통한 우편물 관리

  - 문자 자동 번역

  - 명함 관리

  - 차량번호 자동 인식

    

OCR 키 : eUhtbndWeWlJbmNvdGh3TWNhRUdQdXN3VXliS21kdk8=



주소 : https://jmetakcg50.apigw.ntruss.com/custom/v1/17425/72a2f6aee9aaf69939b7ffeb7d35ebe61bbe3ff668befee52229baaedfad2135/general



OCR 예제

1. API 호출 결과 출력
   - OCRService 서비스 클래스 생성
   - ocrGeneral() 메소드 추가
2. 



OCR Template

- 템플릿으로 등록해 놓은 형식에 맞는 이미지를 전송하면 형식에 맞는 텍스트를 추출해서 반환
- 템플릿 작성
  - 이미지 업로드
  - 추출할 영역 지정 : 필드로 저장 (여러 개 지정)
  - 설정/ 테스트 진행 / 외부 애플리케이션 연동 / 서비스 배포



1. 도메인 생성
2. 템플릿 빌더 : 템플릿 생성
3. 템플릿 작성
4. 콘솔에 출력



ocr 탬플릿 : U0hkQkJkcm5URmhwZ3NPTXBQZVhtQlhxY0liRVRUS1o=



주소 : https://jmetakcg50.apigw.ntruss.com/custom/v1/17436/28c8240a6837a8762f55c73dbd9d512a2b8c8eca9e8308bfb05042564a318690/infer



OCR Template 예제

1. 





## 음성 변환 서비스



### CLOVA Speech Recognition (CSR)

- 사람의 목소리를 인식하여 텍스트로 변환해주는 음성 인식 API 서비스
- 서비스 신청
- 언어별 지원
  - Kor : 한국어
  - Jpn : 일본어
  - Chn : 중국어
  - Eng : 영어
- 전송 : 음성 파일 전송
- 응답 : 텍스트 반환 (JSON 파싱)