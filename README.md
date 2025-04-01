# Chair shopping site(portfolio)
의자 쇼핑몰 사이트 입니다.<br>
데이터베이스 설계, 프론트, 백 개발을 통해 API를 제작하고 암호화 하는 등 React외에도 Express를 통해 백엔드 작업을 경험했습니다.
  
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
- React query를 통해 axios 데이터를 불러오거나 수정, 생성, 삭제 구현(API 관리)
- admin 페이지 제작(레이아웃 분리, refresh 토큰 관리)
- Typescript 환경에서 제작 경험 및 type 관리
- 페이지네이션 제작
- multer를 이용한 파일 업로드 제작
- Scss 사용 경험

## 문제 해결 경험
1. 옵션 제작을 하면서 테이블 설계, 프론트 제작에서 모두 문제를 직면했었습니다. 옵션을 상품 테이블에 같이 포함시켜야할지 따로 테이블로 제작해야할지 고민이 되었었습니다.<br>
결국 옵션과 재고량을 다른 테이블을 통해 분해하여 제작해야 추후에도 개수 제한없이 옵션을 추가하거나 개수를 제한하는 등 유지보수나 확장성에서 더 이로울 것이라고 판단하여 테이블을 분리하였습니다.<br>
이외에도 프론트엔드와 백엔드 간에 데이터를 전달하는 과정에서 겪는 데이터 형식 문제를 경험하면서, 두 분야가 서로 데이터 형식을 지정해야 추후 유지보수 측면에서 더 효율성있게 개발이 가능할 것이라는 것을 알 수 있었습니다.<br>

2. Refresh 토큰과 Access 토큰을 제작하는 작업을 진행하던중, admin 토큰을 저장하고 관리하는 부분에서 고민이 있었는데 admin 계정은 DB가 아닌 따로 파일로 해결하는 것이 더 보안적인 측면에서 더 안전할 것 같다고 판단되어 변경하였습니다.  또한 admin과 사용자들이 로그인을 하기 위한 방법에서 고민이있었는데, 워드프레스에서처럼 관리자는 일반적인 로그인 페이지가 아닌 다른 페이지에서 로그인하는 것이 관리자 입장에서도 관리하기 편할 것이라고 판단하여 다른 페이지에서 로그인하도록 제작했습니다.<br>
특히 admin 전용 refresh토큰과 access 토큰을 제작하고 프론트에서 처리하는 작업이 어려웠는데 해당 부분은 현재 쿠키의 상태에 따라서 user 로그인 상태인지, admin 로그인 상태인지 구분시켜 토큰을 이용하도록 구현했습니다.

3. 파일 업로드 기능 구현 중 API를 이용해 프론트엔드에서 전달한 데이터를 받고자 했지만 받을 수 없었습니다. 업로드한 데이터를 위한 미들웨어가 필요했기 때문이였고, multer라는 미들웨어를 이용해 파일 데이터를 전달 받을 수 있었습니다.<br>
그러나 업로드한 파일을 직접 DB에 저장하는 것은 DB 서버에 부하를 주게 되기 때문에  다른 곳에 바이너리 데이터를 저장할 수 있는 공간이 필요했습니다. 원래라면 AWS를 이용한 저장공간에 넣어야했지만 AWS를 이용하지 않고 구현해보고자 했습니다. 그렇게 파일을 서버에 저장하게 되었고, 이 과정에서 파일을 조회하는데 어려움을 겪었습니다. 
    
## 프로젝트 사용 영상
### 메인 사이트
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/c562cedf-6919-4a2d-b14b-6407f910ddd9

### 관리자 사이트
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/4252706d-6c66-4984-b5af-e7cdd0d829f6
