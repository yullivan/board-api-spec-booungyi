# 게시판 API specification(스펙) 정의
# 게시판의 기능 설계

# 1)게시판 Board ("/v1/Board")


## 게시판의 기능
### | Post 게시판 생성 
  - Requestbody 파라미터
    - id (게시판의 id) , name(게시판 이름) 
### | GET 게시판 조회 
  - RequstParam 파라미터
    - id (게시판의 id) 
### | PUT 수정 
  - Pathveriable 파라미터
    - id(게시판의 id) , name (게시판 이름) 
### | DELET 삭제 
- Pathveriable 파라미터
  - id (게시판의 id)

# 2)게시글 Post ("/v1/board/post")

- 게시글의 구조
  - 
      - id
      - name (작성자)
      - Board id (어떤 게시판의 글인지)
      - date (작성시간)
      - comment (댓글)
      - title (제목)
      - content (게시글의 내용)

## 게시글의 기능
### | Post 게시글 생성 
  - Requestbody 파라미터
    - id(게시글의 id) 
    - title(게시글의 제목)
    - comment(게시글의 내용)
    - date(작성시간)
    - Board id(어떤 게시판의 글인지)
    - name (작성자) 
### | GET 조회 
- RequstParam , Pathveriable
  - id  
### | PUT 수정 
- Pathveriable , RequestBody
  - id
  - comment
### | DELET 삭제
- Pathveriable
  - id
  - 

# 3)댓글 Comment ("v1/board/post/comment)

- 댓글의 구조
  -
      - id (댓글의 id) 
      - contenct(댓글 내용)
      - date (작성 시간) 
      - name (작성자) 
      - Post id(게시글의 id)
- 
## 댓글의 기능
### | Post 생성
  - Requestbody
  - id
  - contenct
  - date
  - name
  - post id
### | GET 조회
- RequstParam , Pathveriable
  - id , name
### | PUT 수정
 - Pathveriable , RequestBody  
   - id
   - contenct
### | DELET 삭제
- Pathveriable
  -  id


[//]: # ( 4.게시글의 조회수)

[//]: # ( 5.게시글의 추천수)





HTTP Method 어떤 메서드를 사용할까
EndPoint(URL): 클라이언트가 호출할 URL

list.stream().map().toList();