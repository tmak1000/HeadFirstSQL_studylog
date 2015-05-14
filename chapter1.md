#chapter1 Memo

##page1~

* p5. 
name|
-> last_name|first_name|birthday|profession|status|location|e-mail|interests|seeking|

|shop|オープン日|入店時間|特徴|苦情|テーブル数|
|---|---|---|---|---|---|
|ダンカンズドーナッツ|4/25|am 8:56|ジャム入り|油っこい|5|

*markdownでは横に余計な数があると、テーブルとして表示されない。

* create database gregs_list; 
  use gregs_list;
  * コマンドは大文字、データベース名は小文字

```
 CREATE TABLE doughnut_list
(
	doughnut_name VARCHAR(10),
	doughnut_tyep VARCHAR(6)
);
```

```
CREATE TABLE my_contacts
(
	last_name VARCHAR(30),
	first_name VARCHAR(20),
	email VARCHAR(50),
	birthday DATE,
	profession VARCHAR(50),
	location VARCHAR(50),
	status VARCHAR(20),
	interests VARCHAR(100),
	seeking VARCHAR(100)
);
```

|烈名|説明|例|最適なデータ型の選択|
|---|---|---|---|
|zip_code|バイナリデータ|dljdlkjljfd|BLOB|
|---|---|---|---|
|atomic_weight||0.0000001|FLOAT|
|---|---|---|---|
|comments|||BLOB|
|---|---|---|---|
|quantity||整数|INTEGER|
|---|---|---|---|
|tax_rate|税率||DEC|
|---|---|---|---|
|book_title|本のタイトル||VARCHAR|
|---|---|---|---|
|gender||M||
|---|---|---|---|
|phone_number|||INTEGER(10)|
|---|---|---|---|
|state|||CHAR(2)|
|---|---|---|---|
|anniversary|DATE|||
|---|---|---|---|
|games_won|ゲーム勝利数|3||
|---|---|---|---|
|meeting_time|ミーティングの時間と日付||DATE & TIME|

* answer 

|烈名|説明|例|最適なデータ型の選択|
|---|---|---|---|
|zip_code|バイナリデータ|dljdlkjljfd|VARCHAR(10)|
|atomic_weight||0.0000001|DEC(10,6)|
|comments|||BLOB|
|quantity||整数|INT|
|tax_rate|税率||DEC(5,3)|
|book_title|本のタイトル||VARCHAR|
|gender||M|CHAR(1)|
|phone_number|||CHAR(10)|
|state|||CHAR(2)|
|anniversary|DATE||DATE|
|games_won|ゲーム勝利数|3|INT|
|meeting_time|ミーティングの時間と日付||DATETIME|

```
CREATE TABLE my_contacts
(
        last_name VARCHAR(30),
        first_name VARCHAR(20),
        email VARCHAR(50),
        birthday DATE,
        profession VARCHAR(50),
        location VARCHAR(50),
        status VARCHAR(20),
        interests VARCHAR(100),
        seeking VARCHAR(100)
	gender CHAR(1)
);
=>
CREATE DATABASE gregs_list;
USE gregs_list;
CREATE TABLE my_contacts
(
        last_name VARCHAR(30),
        first_name VARCHAR(20),
        email VARCHAR(50),
        birthday DATE,
        profession VARCHAR(50),
        location VARCHAR(50),
        status VARCHAR(20),
        interests VARCHAR(100),
        seeking VARCHAR(100),
        gender CHAR(1)
);

DROP TABLE my_contacts;


excercise

1.DATE,DATETIME,DEC,INT
2.DROP TABLE
3.CHAR
4.DATE
5.USE DATABASE
6.INT
7.BLOB
8.CREATE DATABASE
9.CREATE TABLE
10.DATETIME
11.DEC
12.DESC 
13.CREATE TABLE

INSERT INTO my_contacts
(last_name,first_name,email,gender,birthday,
profession,location,status,interests,seeking)
VALUES('アンダーソン','ジリアン','jill_anderson@brakneckpizza.com',
'F','1980-09-05',
'テクニカルライター','カリフォルニア州パロアルト','独身','カヤック乗り、爬虫類','恋人、友達')	
;

INSERT INTO my_contacts
(first_name,email,
profession,location)
VALUES('パット','patpost@brakneckpizza.com',
'郵便局員','ニュージャージ州プリンストン')
;

SELECT * FROM my_contacts;

CREATE TABLE my_contacts
(
	last_name VARCHAR(30) NOT NULL,
	first_name VARCHAR(20) NOT NULL
)
;


```


