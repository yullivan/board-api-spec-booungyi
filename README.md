# 게시판 API specification(스펙) 정의

# 게시판의 기능 설계

### 생성 | POST

- POST
    - Requestbody

### 조회 | GET

- GET
    - RequstParam , Pathveriable

### 수정 | PUT

- PUT
    - Pathveriable , RequestBody

### 삭제 | DELET

- DELET
    - Pathveriable

## 게시판의 기능

# 1)게시판 (Board)

- 게시판의 구조
  -
      - name
      - id

### 생성,조회,수정,삭제

# 2)게시글 (Post)

- 게시글의 구조
  - 
      - id
      - name (작성자)
      - Board id (어떤 게시판의 글인지)
      - date (작성시간)
      - comment (댓글)
      - title (제목)
      - content (게시글의 내용)

### 게시글의 기능

생성, 조회,수정,삭제

# 3)댓글(Comment)

- 댓글의 구조
  -
      - id (댓글의 id) 
      - contenct(댓글 내용)
      - date (작성 시간) 
      - name (작성자) 
      - Post id(게시글의 id)

### 생성, ### 조회,수정,삭제

[//]: # ( 4.게시글의 조회수)

[//]: # ( 5.게시글의 추천수)





HTTP Method 어떤 메서드를 사용할까
EndPoint(URL): 클라이언트가 호출할 URL

list.stream().map().toList();