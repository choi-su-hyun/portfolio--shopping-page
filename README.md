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
- Express.js로 로그인, 회원가입, 로그아웃 API 제작
- Redux를 통한 저장소 사용(Thunk로 비동기 데이터 사용 경험)
- MySQL을 이용한 데이터베이스 제작 후 백엔드와 연동
- bcrypt를 통한 비밀번호 암호화
- jwt 토큰을 통해 유저 정보 확인 및 보안 유지
- Refresh 토큰과 Access 토큰 제작
- React query를 통해 axios 데이터를 불러오거나 수정, 생성, 삭제 구현(API 관리)
- multer를 이용한 파일 업로드 제작

## 문제 해결 경험
1. 옵션 제작을 하면서 테이블 설계, 프론트 제작에서 모두 문제를 직면했었습니다. 옵션을 상품 테이블에 같이 포함시켜야할지 따로 테이블로 제작해야할지 고민이 되었었습니다.<br><br>
결국 옵션과 재고량을 다른 테이블을 통해 분해하여 제작해야 추후에도 개수 제한없이 옵션을 추가하거나 개수를 제한하는 등 유지보수나 확장성에서 더 이로울 것이라고 판단하여 테이블을 분리하였습니다.<br><br>
이외에도 프론트엔드와 백엔드 간에 데이터를 전달하는 과정에서 겪는 데이터 형식 문제를 경험하면서, 두 분야가 서로 데이터 형식을 지정해야 추후 유지보수 측면에서 더 효율성있게 개발이 가능할 것이라는 것을 알 수 있었습니다.<br>

2. 초기에는 서버내에서만 access 토큰과 refresh 토큰이 사용 가능한지에 대한 여부를 한번에 검증하여 재 로그인을 유도를 구현했지만, 로직의 복잡성 증가와 가독성이 떨어지는 문제로 인해 확장성이 떨어진다고 생각했습니다.<br>
프론트엔드와 절차를 나누어 토큰 검증이 이루어지도록 변경하여 가독성을 높였습니다.

3. 이미지 파일 업로드 기능 구현 중 일반적인 API를 이용해 프론트엔드에서 전달한 데이터를 받고자 했지만 받을 수 없었습니다. 업로드한 데이터는 multer라는 업로드 데이터를 가져오는 미들웨어를 통해 전달 받을 수 있었습니다.<br><br>
그러나 업로드한 파일을 직접 DB에 저장하는 것은 DB 서버에 부하를 주게 되기 때문에 다른 곳에 바이너리 데이터를 저장할 수 있는 공간이 필요했습니다. 원래라면 AWS를 이용한 저장공간에 넣어야했지만 AWS를 이용하지 않고 구현해보고자 했습니다. 그렇게 파일을 서버의 파일구조로 저장하는 방식으로 구현해보게 되었고, 이 과정에서 파일을 조회하는데 어려움을 겪었습니다.<br><br>
프론트엔드에서 파일구조에 맞게 해당 자원으로 접근하고자 했지만 접근할 수 없었고, 서버에서도 정적인 데이터를 접근할 수 있도록 경로를 만들어주어야 한다는 것을 알 수 있었습니다. 이를 통해 파일 데이터 업로드 및 저장 방법과 프론트엔드에서 서버로 접근하기 위한 API에 대한 이해의 폭을 넓힐 수 있었습니다.
    
## 프로젝트 사용 영상
### 메인 사이트
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/c562cedf-6919-4a2d-b14b-6407f910ddd9

### 관리자 사이트
https://github.com/choi-su-hyun/portfolio--shopping-page/assets/86158560/4252706d-6c66-4984-b5af-e7cdd0d829f6
