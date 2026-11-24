SSR 홈페이지 HTML 뼈대

파일 구성
- index.html
- assets/ssr-hero.jpg
- quote/index.html (견적서 메뉴, /quote/)
- quote/customer/index.html (일반 고객용 표준 CSV 견적서, /quote/customer/)
- quote/staff/index.html (직원용 얼마에요 CSV 견적서, /quote/staff/)
- quote/request/index.html (견적 요청서 작성 프로그램, /quote/request/)

사용 방법
1. 폴더를 웹서버 또는 호스팅에 업로드
2. 업무 서비스 주소와 문구는 public/index.html에서 수정

현재 구성
- 전자결재 화면과 어울리는 좌측 메뉴·상단 바로가기·흰색 업무 대시보드
- 기존 SSR 로봇 이미지를 활용한 환영 배너
- PC·모바일 반응형 레이아웃
- 얼마에요 4.0 ERP, 전자결재, 웹메일, 일정 및 메신저, 디지털 견적 바로가기
- 얼마에요 4.0 ERP, 전자결재, 일정 및 메신저, 디지털 견적 링크는 새 창에서 열림
- 디지털 견적 바로가기에서 /quote/ 견적 메뉴로 이동
- 견적 메뉴에서 고객용 견적서, 직원용 얼마에요 견적서, 견적 요청서를 선택
- 직원용 경로는 정적 공개 페이지이며 로그인·접근제어 연동 전에는 보안되지 않음
- 견적 공급자 상호 기본값은 (주)에스에스알이며 직접 수정 가능
- 연락처·주소·실제 회사 로고는 기본 배포본에 아직 등록되지 않음
- 공급자 프로필 저장은 현재 브라우저별 localStorage 방식이며 직원 공용 저장소가 아님
