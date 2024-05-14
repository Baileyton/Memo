# Memo

## 
Build system: Gradle - Groovy
JDK: 17

## 기능 설계
GET API 사용해서 메모 전체 목록 조회
POST API 사용해서 메모 신규 생성
PUT API 사용해서 메모 내용 변경하기
DELETE API 사용해서 메모 삭제하기

## API 테이블
| 기능    | URL             | Http Method | Return                |
|:------|:----------------|:------------|:----------------------|
| 메모 생성 | /api/memos      | POST        | MemoResponseDto       |
| 메모 조회 | /api/memos      | GET         | List<MemoResponseDto> |
| 메모 변경 | /api/memos/{id} | PUT         | Long                  |
| 메모 삭제 | /api/memos/{id} | DELETE      | Long                  |