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
|zip_code|バイナリデータ|dljdlkjljfd|BLOB|
|atomic_weight||0.0000001|FLOAT|
|comments|||BLOB|
|quantity||整数|INTEGER|
|tax_rate|税率||DEC|
|book_title|本のタイトル||VARCHAR|
|gender||M||
|phone_number|||INTEGER(10)|
|state|||CHAR(2)|
|anniversary|DATE|||
|games_won|ゲーム勝利数|3||
|meeting_time|ミーティングの時間と日付||DATE & TIME|





