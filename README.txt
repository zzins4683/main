SSR 홈페이지 HTML 뼈대

파일 구성
- index.html
- assets/ssr-hero.jpg
- robot-monitor/index.html (로봇 원격 모니터링 UI 시안, /robot-monitor/)
- quote/index.html (견적서 메뉴, /quote/)
- quote/customer/index.html (일반 고객용 표준 CSV 견적서, /quote/customer/)
- quote/staff/index.html (직원용 얼마에요 CSV 견적서, /quote/staff/)
- quote/request/index.html (견적 요청서 작성 프로그램, /quote/request/)

사용 방법
1. 폴더를 웹서버 또는 호스팅에 업로드
2. 업무 서비스 주소와 문구는 public/index.html에서 수정

현재 구성
- 전자결재 화면과 어울리는 접을 수 있는 좌측 메뉴와 흰색 업무 대시보드
- 기존 SSR 로봇 이미지를 활용한 환영 배너
- PC·모바일 반응형 레이아웃
- 모바일 첫 화면 인트로는 실제 SSR 정문 사진을 문짝으로 사용하고, 고해상도 로봇 이미지 기반 접근 연출과 바닥 안개를 표시
- 명함 인쇄용 홈페이지 QR: public/assets/ssr-business-card-qr.svg (벡터) 및 .png, 연결 주소 https://ssr.ai.kr/
- 얼마에요 4.0 ERP, 전자결재, 웹메일, 네이버웍스, 디지털 견적, 부캉이 게임 바로가기
- 외부 업무 서비스와 부캉이 게임은 새 창에서 열림
- 디지털 견적 바로가기에서 /quote/ 견적 메뉴로 이동
- 모바일 인트로는 문이 먼저 열리고 로봇 이미지가 점점 다가온 다음 흰색 전환으로 대시보드 표시
- 로봇 동작은 정지 이미지 레이어와 CSS 발걸음 효과를 이용한 10초 웹 애니메이션이며, 별도의 실사 MP4 영상은 아님
- 견적 메뉴에서 고객용 견적서, SSR 견적, 견적 요청서를 선택
- SSR 견적의 ID/PW 화면은 진입 흐름을 보여주는 데모이며 입력값을 검증하거나 저장하지 않음
- SSR 견적과 다른 정적 페이지는 서버 측 로그인·접근제어가 적용되기 전까지 공개 상태임
- SSR 견적 공급자 정보와 회사 로고·직인은 SSR 기본값으로 고정
- 견적 브랜드 이미지: public/quote/assets/ssr-logo.jpg, public/quote/assets/ssr-stamp.png
- 고객용·직원용·상세 견적 페이지에서 분류별 CSV 여러 개를 함께 가져올 수 있으며 파일별 갑지 항목과 상세 내역으로 반영
- 공급자 프로필 저장은 현재 브라우저별 localStorage 방식이며 직원 공용 저장소가 아님
- 로봇 모니터링 페이지는 관리자가 설치·등록한 대상 PC만 원격 접속하는 UI 시안이며, 실제 원격 연결·PLC 통신은 아직 구현되지 않음
- 로봇 상태·알람·JOB 예시 데이터는 데모이며, 실제 연동은 장비별 컨트롤러/PLC 모델 및 읽기 인터페이스 확인 후 개발 필요
