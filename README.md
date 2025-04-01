# jobinterview

**목차**

- [Rest Api란?](#rest-api란)
- [Rest api Method 종류](#rest-api-method-종류)
- [Restful의 특징](#restful의-특징)
- [Rest와 Restful의 차이](#rest와-restful의-차이)
- [Status Code 종류](#status-code-종류)
- [iOS에서 REST API 사용 방식](#ios에서-rest-api-사용-방식)

---

## Rest Api란?

- 정보를 주고 받는 형식
- 자원을 이름과 상태로 구분하여 전달
- 요청의 의도와 목적을 쉽게 파악할 수 있음

---

## Rest api Method 종류

- **GET** : 조회
- **POST** : 정보 추가
- **DELETE** : 삭제
- **PUT** : 수정 - 전체
- **PATCH** : 수정 - 부분

---

## Restful의 특징

- URI는 자원을 표현
- HTTP Method로 동작(행위)을 표현
- 무상태성 (Stateless): 요청 간에 서버가 클라이언트의 상태를 저장하지 않음
- 계층 구조 (Layered System): 클라이언트는 중간 서버를 거쳐도 상관 없음

---

## Rest와 Restful의 차이

- **REST**: 아키텍처 스타일 (원칙, 설계 철학)
- **RESTful**: REST 원칙을 잘 지켜서 구현한 API

---

## Status Code 종류

- **200 OK** : 요청 성공
- **201 Created** : 리소스 생성 성공
- **204 No Content** : 성공했지만 반환할 데이터 없음
- **400 Bad Request** : 클라이언트 요청 오류
- **401 Unauthorized** : 인증 필요
- **403 Forbidden** : 접근 권한 없음
- **404 Not Found** : 리소스 없음
- **500 Internal Server Error** : 서버 에러

---

## iOS에서 REST API 사용 방식

- `URLSession`: 가장 기본적인 네트워킹 API
- `Alamofire`: Swift 기반의 네트워킹 라이브러리 (간편하고 코드 가독성 좋음)
- 응답 데이터 처리: `Codable`을 활용한 JSON 디코딩
- 비동기 처리: `async/await`, `completion handler`, `Combine` 등
