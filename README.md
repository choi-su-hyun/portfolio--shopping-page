# Chair shopping site(portfolio)
의자를 판매하는 쇼핑몰 사이트 개발 
데이터베이스 설계, 프론트, 백 개발을 통해 React와 Express를 경험했습니다. React 위주로 처음으로 작업해보았던 포트폴리오 입니다.
  
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
9. CSS
    
## 참여 인원
제작자 1 명 (개인 포트폴리오)

## 데이터베이스 설계
![chair-shopping-ERD](https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/bb124ce3-5363-4074-9c91-7da1f0a72633)

## 해당 프로젝트로 배운 내용
- React.js를 통한 로그인,회원가입, 로그아웃 구현(+ Express.js로 로그인, 회원가입, 로그아웃 API 제작)
- axios를 이용한 글 생성, 수정, 삭제 API 사용 및 제작
- Redux를 통한 저장소 사용(Thunk를 통한 비동기 데이터 사용)
- MySQL을 이용한 데이터베이스 제작 후 백엔드와 연동
- bcrypt를 통한 비밀번호 암호화
- cookie를 이용하여 로그인 상태 유지
- jwt 토큰을 통해 유저 정보 확인 및 보안 유지
- refresh 토큰과 access 토큰 제작
- custom hook 사용
- react daum postcode 사용을 통한 우편번호 구현
- React query를 통해 axios 데이터를 불러오거나 수정, 생성, 삭제 구현
- admin 페이지 제작(레이아웃 분리, refresh 토큰 관리)
- Typescript를 통한 type 관리
- 페이지네이션 제작
- multer를 이용한 파일 업로드 제작

## 문제 해결 경험
옵션 제작을 하면서 테이블 설계, 프론트 제작에서 모두 문제를 직면했었습니다. 결국 옵션과 재고량을 따로 테이블을 통해 분해하여 제작하고 프론트에서는 옵션명, 재고량의 객체를 담은 배열 형태로 전송하게 되었고, 이 옵션을 테이블에 저장하는 과정에서 많은 고민을 하게 되었습니다.
생성부분에서는 큰 고민이 없었지만 문제는 수정과 삭제 부분이였습니다. 
결국 일어날 수 있는 상황을 if문으로 작성하여 각각의 상황에 필요한 옵션명들을 분류했고, 그 분류한 값들을 통해 해당하는 재고량과 옵션명을 옵션 테이블에 저장함으로써 해결했습니다. 하지만 또 이 작업을 하게 된다면 차라리 프론트에서 옵션 만큼은 수정, 삭제 부분에서는 api를 따로 만들어주는 것이 좋을 것 같다고 생각이 들었습니다.

또한 refresh 토큰과 access 토큰을 제작하는 부분에서 admin 부분과 일반적인 user 부분을 구분하는 쪽에서 고민이 있었는데 admin 계정은 DB가 아닌 따로 파일로 해결하는 것이 더 안전할 것 같다고 판단되어 변경하였고, admin은 워드프레스에서 처럼 다른 페이지에서 로그인 하는 것이 관리자 입장에서도 관리하기 편할 것이라고 생각하여 다른 페이지에서 로그인하도록 제작했습니다.
특히 admin용 refresh와 access 토큰을 제작하고 프론트에서 처리하는 작업이 어려웠는데 해당부분은 현재 쿠키의 상태에 따라서 user로그인 상태인지, admin로그인 상태인지 구분시켜 토큰을 이용하도록 구현했습니다.
    
## 프로젝트 사용 영상
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/c562cedf-6919-4a2d-b14b-6407f910ddd9

