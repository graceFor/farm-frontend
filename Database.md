User {
username: String, // 사용자 이름
userCel: Number, // 사용자 전화번호
userId: String, // 사용자 아이디
hashedPassword: String, // 사용자 비밀번호
}

Comment {
content: String // 내용
author: User // 작성자
post: Post, // 어떤 글의 댓글인지
parent: ID?
}

Post{
title: String, // 게시글 제목
content: String(markdown), // 게시글 본문
author: User, // 작성자
recommend: Number, //추천수
views: Number, //조회수
created_at: DateTime, // 생성일자
last_edit: DateTime, // 마지막 수정일자
}
