# springbook_website

코드로 배우는 스프링 웹 프로젝트 개정판 책 참고

Oracle SQLDeveloper 필요 

//테이블 tbl_board 필요 

create USER book_ex IDENTIFIED BY book_ex
DEFAULT TABLESPACE USERS
TEMPORARY TABLESPACE TEMP;

//권한 부여 
grant connect, DBA TO BOOK_EX; 


create table tbl_board(
    bno number(10,0),
    title varchar2(200) not null,
    content varchar2(2000) not null,
    writer varchar2(50) not null,
    regdate date default sysdate,
    updatedate date default sysdate
);


//sequence 추가
create sequence seq_board;
