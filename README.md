# 🧮 킹받는계산기

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

단순한 계산기처럼 보이지만, 1회 무료 사용 후 **"결제"를 요구하는 재미있는 컨셉의 웹 계산기**입니다. 
결제창은 실제 결제 시스템(PG)과 유사한 수준의 **프론트엔드 실시간 유효성 검사 로직**을 구현하여 사용자 경험과 UI/UX 디자인을 시뮬레이션하기 위해 제작되었습니다.

🔗 **[Live Demo 보러가기](여기에_GitHub_Pages_주소를_입력하세요)**

---

## ✨ 주요 기능

### 1. 기본 계산기 & 테마 시스템
* 사칙연산을 지원하는 깔끔한 Glassmorphism 디자인의 계산기
* 시스템 환경(OS)을 감지하는 **다크 모드 / 라이트 모드** 지원 및 사용자 설정 로컬 저장(`localStorage`)

### 2. 재미를 더한 결제 시뮬레이션
* 1회 계산 완료 후, 다음 계산 시 결제 모달 팝업 등장
* Apple Pay 및 신용카드 모의 결제 UI 구현 (Thinking 모달 등 시각적 피드백 제공)

### 3. 🛡️ 고도화된 실시간 신용카드 유효성 검증 (Front-end)
* **Luhn 알고리즘**: 수학적 규칙을 통해 입력된 카드 번호의 무결성(오타) 검증
* **BIN 번호 판별 및 동적 로고**: 입력된 카드 앞자리를 분석하여 해당 카드 브랜드(Visa, MasterCard, Amex, Discover, JCB)의 로고를 입력창에 실시간으로 표시
* **만료일(Expiry) 검증**: 현재 시점을 기준으로 과거의 만료일이 입력되면 즉시 차단
* **실시간 에러 하이라이팅**: 카드 번호나 유효기간 등의 규칙이 틀렸을 경우, 입력 칸을 즉시 빨간색으로 변경하여 직관적인 UI 피드백 제공

---

## ⚠️ 보안 및 개인정보 처리 안내 (Notice)

본 프로젝트는 순수한 **프론트엔드(Client-side) 시뮬레이션**입니다.
* **서버 전송 없음**: 사용자가 입력한 모든 카드 정보(번호, CVC, 비밀번호 등)는 외부 서버나 데이터베이스로 **절대 전송되지 않습니다.**
* **즉시 파기**: 입력된 데이터는 오직 브라우저 내에서 자바스크립트를 통한 유효성 검사에만 사용되며, 가상 결제 승인 프로세스 직후 메모리에서 즉시 초기화(삭제)됩니다.
* 안심하고 가짜 카드 번호(테스트 번호)를 입력하여 유효성 검사 로직을 테스트해 보세요!

---

## 🚀 사용 방법 (How to Run)

별도의 빌드나 서버 구축 과정이 필요하지 않은 순수 Vanilla 웹 프로젝트입니다.

1. 저장소를 클론(Clone)하거나 ZIP 파일로 다운로드합니다.
2. 폴더 내의 `index.html` 파일을 더블 클릭하여 웹 브라우저에서 실행합니다.
3. 계산을 1회 수행한 뒤, 다시 계산 버튼(`=`)을 눌러 결제 시스템을 테스트해 봅니다.

---

## 👨‍💻 제작자
* **HANGGOK** * GitHub: [@alexjeon5](https://github.com/alexjeon5)
