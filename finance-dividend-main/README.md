# 📝 실전 배당금 프로젝트

## 1️⃣ 프로젝트 소개
> 크롤링을 통해 주식 데이터를 가져와 배당금을 알아보는 프로젝트입니다.

## 2️⃣ Tech Stack
- Language : `Java`
- Build : `gradle`
- DataBase : `MySQL`, `H2 DataBase`
- JDK : `JDK 11`
- Library : `Lombok`, `spring-web`, `logback`, `Jsoup`, `Jwt`

## 3️⃣ API 명세서
### 🎯 배당금 API
✅ GET /finance/dividend/{companyName}
- 특정 회사의 배당금 내역 조회
- 회사 이름과 배당금 지급 내역을 보여줌

✅ GET /company/autocomplete?keyword=O
- 배당금 검색 - 자동완성

✅GET /company
- 회사 리스트 조회

✅ POST /company
- 배당금 저장
- {ticker : "GOOD"} ticker 파라미터로 받아주세요
- DB에 {ticker : "GOOD", companyName : "좋은회사"} 이렇게 저장합니다.

✅ DELETE /company?ticker=GOOD
- 배당금 삭제

## 4️⃣ 회원 API
- ✅ 회원가입
- ✅ 로그인
- ✅ 로그아웃
