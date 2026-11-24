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
2. 문구와 메뉴 링크 수정
3. 실제 회사 로고 SVG/PNG가 준비되면 .brand 영역 교체
4. 프로젝트 사진을 추가하여 하단 섹션 확장

현재 구성
- 상단 알림바
- 투명 오버레이 내비게이션
- 전체화면 메인 비주얼
- 반응형 PC/모바일
- 회사소개 / 사업영역 / MERCARE / 프로젝트 / 정부지원사업 / 문의 섹션
- 디지털 견적 버튼에서 /quote/ 견적 메뉴로 이동
- 견적 메뉴에서 고객용 견적서, 직원용 얼마에요 견적서, 견적 요청서를 선택
- 직원용 경로는 정적 공개 페이지이며 로그인·접근제어 연동 전에는 보안되지 않음
- 견적 공급자 상호 기본값은 (주)에스에스알이며 직접 수정 가능
- 연락처·주소·실제 회사 로고는 기본 배포본에 아직 등록되지 않음
- 공급자 프로필 저장은 현재 브라우저별 localStorage 방식이며 직원 공용 저장소가 아님
