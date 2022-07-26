# AI_Platform_TIL_02





포즈인식 (Pose Estimation)

1. 기본(API 호출 결과 확인)
   - PoseEstimationService 서비스 생성
   - poseEstimate() 메소드 추가
   - API 자바 코드 복사
   - 컨트롤러에 추가
   - index.jsp에 추가
   - 결과 확인 
     - 콘솔에 JSON 문자열 출력하고 Json Viewer에서 전체 구조 확인



객체 탐지 (Object Detection)

1. 기본(API 호출 결과 확인)
   - ObjectDetectionService 서비스 생성
   - objectDetect() 메소드 추가
   - API 코드 복사
   - 결과를 콘솔에 출력
   - 컨트롤러에 추가 
   - index.jsp에 추가
   - 결과 확인 
     - 콘솔에 JSON 문자열 출력하고 Json Viewer에서 전체 구조 확인
2. JSON 결과 파싱
   - ObjectVO 생성
     - String name
     - double x1, y1, x2, y2
   - jsonToVOList() 메소드 추가
     - JSON 형태의 문자열 파싱해서 VO에 저장
     - 리스트에 추가 : objectList





한글로 변환

- Naver Papago 사용하여 한글로 번역

- 입력한 텍스트를 인공신경망 기반 번역 알고리즘을 통해 여러 나라의 언어로 자동 번역

- Papago Text Translation 서비스 추가

- 객체 탐지 서비스에 추가

  - 객체 탐지 결과가 영어로 반환

  - 객체 탐지 결과를 한글로 변환해서 한글로 출력되도록 작성

    