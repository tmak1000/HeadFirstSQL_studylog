#chapter4

SELECT * FROM fish_info WHERE location LIKE 'ニュージャージー州%';

SELECT * FROM fish_records WHERE state = 'ニュージャージー州';

テーブル設計の方法
１：テーブルで記述したい物事を一つ取り上げます。
２：テーブル使用時に知っている必要がある、その１つの物事に関する情報の一覧を作ります。
３：その一覧を使って、物事についての情報を断片に分断し、それを用いてテーブルを編成できるようにします。

テーブルに何を入れるか考える方法
1:あなたのテーブルが記述する１つの物事は何ですか？
２：その１つのもの後を取得するために、どのようなテーブルを使いますか？
３：クエリを短くて容量を得たものにするため、列は原始的なデータを含んでいますか？

interests
ran,soccer

　primary key is not null
　primary key needs values
　primary key is simple
  primary key is not changed

SHOW CREATE TABLE my_contacts;


 CREATE TABLE `my_contacts` (
  contact_id INT NOT NULL AUTO_INCREMENT,
  `last_name` varchar(30) DEFAULT NULL,
  `first_name` varchar(20) DEFAULT NULL,
  `email` varchar(50) DEFAULT NULL,
  `birthday` date DEFAULT NULL,
  `profession` varchar(50) DEFAULT NULL,
  `location` varchar(50) DEFAULT NULL,
  `status` varchar(20) DEFAULT NULL,
  `interests` varchar(100) DEFAULT NULL,
  `seeking` varchar(100) DEFAULT NULL,
  `gender` char(1) DEFAULT NULL,
  PRIMARY_KEY (contact_id)

) ;

CREATE TABLE person(
       person_id INT NOT NULL AUTO_INCREMENT,
       first_name VARCHAR(20) NOT NULL,
       last_name VARCHAR(20) NOT NULL,
       PRIMARY KEY(person_id)
);

INSERT INTO person VALUES(1,'jan','blady');

