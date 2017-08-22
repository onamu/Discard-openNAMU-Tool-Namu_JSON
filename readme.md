## 개요
나무위키에서 배포하는 JSON을 오픈나무에 맞게 컨버팅하는 스크립트입니다.

PS. 메모리 엄청 잡아먹습니다. (12GB 이상)

### 되는 것
 * 나무위키의 JSON파일을 읽어서 파이썬 dict형식으로 변환하기
 * 사전형으로 변환한 파일을 읽어서 오픈나무가 받아들일 수 있는 형식으로 변환하기
 * 문서 편집자의 종류 구별하기 (리그베다 위키, 나무위키, 익명)

### 안되는 것
 * 나무위키에서의 편집 로그 반영 (JSON 파일에 해당 데이터가 없습니다)

### 의존성
 * 파이썬 3.3 이상 (3.6 권장)
 * [pymysql](https://pypi.python.org/pypi/PyMySQL)

### 사용법
1. 빈 디텍토리를 하나 만듭니다.
2. 그 디텍토리에 나무위키 JSON파일의 이름을 namuwikidata.json으로 바꾸고 집어 넣습니다.
3. set.json에 db 관련 내용을 기제 합니다.
4. 그 디렉토리에서 파이썬 스크립트를 실행시킵니다.