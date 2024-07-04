# spring-gift-wishlist
## Step1
### 요구 사항
- 상품을 추가하거나 수정하는 경우, 클라이언트로부터 잘못된 값이 전달될 수 있다. 잘못된 값이 전달되면 클라이언트가 어떤 부분이 왜 잘못되었는지 인지할 수 있도록 응답을 제공한다.
   - [x] 상품 이름은 공백을 포함하여 최대 15자까지 입력할 수 있다.
   - [x] 가능한 특수 문자 : ( ), [ ], +, -, &, /, _ 이외의 특수 문자는 사용 불가
   - [x] "카카오"가 포함된 문구는 담당 MD와 협의한 경우에만 사용 가능
### 구현
- @Valid 사용
- GlobalExceptionHandler 구현

## Step2
### 요구 사항
- 사용자가 회원 가입, 로그인, 추후 회원별 기능을 이용할 수 있도록 구현한다
  - 회원은 이메일과 비밀번호를 입력하여 가입한다
  - 토큰을 받으려면 이메일과 비밀번호를 보내야 하며, 가입한 이메일과 비밀번호가 일치하면 토큰 발급됨
  - 트큰을 생성하는 방법에는 여러 가지가 있다. 방법 중 하나를 선택(Jwt 사용)
### 구현
[x] 회원 가입과 로그인 기능 구현
[x] JWT 라이브러리 이용하여 토큰 주고받도록 한다
[x] DB에 users 테이블 생성
[x] 로그인 실패시 403 에러 코드 반환

