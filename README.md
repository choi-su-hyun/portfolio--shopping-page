# Chair shopping site(portfolio)
의자 쇼핑몰 사이트 입니다.<br>
데이터베이스 설계, 프론트, 백 개발을 통해 React와 Express를 경험했습니다.<br>
React 위주로 처음으로 작업해보았던 포트폴리오 입니다.
  
**Front Github**  
[https://github.com/choi-su-hyun/chair-shopping-front](https://github.com/choi-su-hyun/chair-shopping-front)
  
**Back Github**  
[https://github.com/choi-su-hyun/chair-shopping-back](https://github.com/choi-su-hyun/chair-shopping-back)

## 사용 기술
1. React.js
2. Redux
3. React Query
4. Typescript
5. Express.js
6. Node.js
7. MySQL
8. HTML
9. SCSS
    
## 참여 인원
제작자 1 명 (개인 포트폴리오)

## 데이터베이스 설계
![chair-shopping-ERD](https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/bb124ce3-5363-4074-9c91-7da1f0a72633)

## 해당 프로젝트로 배운 내용
- React.js를 통한 로그인, 회원가입, 로그아웃 구현(+ Express.js로 로그인, 회원가입, 로그아웃 API 제작)
- axios를 이용한 글 생성, 수정, 삭제 API 사용 및 제작
- Redux를 통한 저장소 사용(Thunk로 비동기 데이터 사용 경험)
- MySQL을 이용한 데이터베이스 제작 후 백엔드와 연동
- bcrypt를 통한 비밀번호 암호화
- cookie를 이용하여 로그인 상태 유지
- jwt 토큰을 통해 유저 정보 확인 및 보안 유지
- Refresh 토큰과 Access 토큰 제작
- Custom hook 사용
- react daum postcode 사용을 통한 우편번호 구현
- React query를 통해 axios 데이터를 불러오거나 수정, 생성, 삭제 구현(API 관리)
- admin 페이지 제작(레이아웃 분리, refresh 토큰 관리)
- Typescript 환경에서 제작 경험 및 type 관리
- 페이지네이션 제작
- multer를 이용한 파일 업로드 제작
- Scss 사용 경험

## 문제 해결 경험
1. 옵션 제작을 하면서 테이블 설계, 프론트 제작에서 모두 문제를 직면했었습니다. 옵션을 상품 테이블에 같이 포함시켜야할지 따로 테이블로 제작해야할지 고민이 되었었습니다.<br>
결국 옵션과 재고량을 다른 테이블을 통해 분해하여 제작하는 것이 데이터를 관리하는 면에서 더 편할 것 같다고 판단하여 테이블을 분리하였습니다.<br>
프론트에서는 옵션 명, 재고량의 객체를 담은 배열 형태로 전송하게 되었습니다. 또한 이 옵션을 테이블에 저장하는 과정에서도 많은 고민을 하게 되었습니다.<br>
생성부분에서는 큰 고민이 없었지만, 문제는 수정과 삭제 부분이었습니다. 배열 내에서 어떤 옵션을 수정하거나 삭제했는지 구분이 필요했는데 배열이다보니 완벽한 구분이 어렵겠다고 판단하였습니다.<br>
결국 일어날 수 있는 상황들(삭제/수정/추가 되어야할 옵션을)을 조건문을 통해 옵션 명들을 분류했고, 그 분류한 값들을 통해 해당하는 재고량과 옵션 명을 옵션 테이블에 저장함으로써 해결했습니다.<br>
하지만 또 이 작업을 하게 된다면 차라리 프론트에서 옵션만큼은 수정, 삭제 기능의 페이지에서만 api 를 따로 만들어주는 것이 좋을 것 같다는 생각이 들었습니다.

2. Refresh 토큰과 Access 토큰을 제작하는 작업에서 admin 토큰을 저장하고 관리하는 부분에서 고민이 있었는데 admin 계정은 DB가 아닌 따로 파일로 해결하는 것이 더 안전할 것 같다고 판단되어 변경하였습니다.<br>
또한 admin과 사용자들이 로그인을 하기 위한 방법에서 고민이있었는데, 워드프레스에서처럼 관리자는 일반적인 로그인 페이지가 아닌 다른 페이지에서 로그인하는 것이 관리자 입장에서도 관리하기 편할 것이라고 판단하여 다른 페이지에서 로그인하도록 제작했습니다.<br>
특히 admin 전용 refresh토큰과 access 토큰을 제작하고 프론트에서 처리하는 작업이 어려웠는데 해당 부분은 현재 쿠키의 상태에 따라서 user 로그인 상태인지, admin 로그인 상태인지 구분시켜 토큰을 이용하도록 구현했습니다.

3. 이외에도 useEffect 관련 문제나 React Query의 데이터 최신화 문제, MySQL 비동기 문제 등 다양한 문제들을 겪었으며, 이때 검색도 중요했지만, 차근차근 실행 경로를 따라가는 것도 굉장히 중요하다는 것을 알 수 있었습니다. (공책에 적어 가며 최대한 구조를 이해하며 접근하여 해결했습니다)
    
## 프로젝트 사용 영상
### 메인 사이트
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/c562cedf-6919-4a2d-b14b-6407f910ddd9

### 관리자 사이트
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/4252706d-6c66-4984-b5af-e7cdd0d829f6
