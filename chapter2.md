#chapter2
```
飲み物あてクイズ
ライムフィズ、エラー、帰ってこない、ホットゴールド、オーマごっしゅ、エラー、エラー

SELECT * FROM my_contacts
WHERE location = 'Grover's Mill';

1: SELECT * FROM my_contacts
WHERE location = 'Grover¥'s Mill';

2:SELECT * FROM my_contacts
WHERE location = 'Grover''s Mill';


キスオンザリップス

SELECT drink_name FROM easy_drinks
WHERE
main = 'チェリージュース';

SELECT drink_name FROM easy_drinks
WHERE
amount1  = 2 AND  main = 'チェリージュース';

SELECT drink_name FROM easy_drinks
WHERE
second = 'あんず果汁';

SELECT drink_name FROM easy_drinks
WHERE
amount1 = 2 AND amount2 = 7;

SELECT drink_name FROM easy_drinks
WHERE
directions = '氷の上に注いで、ストローを付ける。'

ブルフロッグ

SELECT drink_name FROM easy_drinks
WHERE
amount1  = 1.5 AND  main = 'アイスティー';

SELECT drink_name FROM easy_drinks
WHERE
second = 'レモネード';

SELECT drink_name FROM easy_drinks
WHERE
drinkname = 'ブルフロッグ';

SELECT drink_name FROM easy_drinks
WHERE
directions = '氷の上に注いでライムを一切れ加える。'

SELECT email FROM my_contacts WHERE professyon = 'コンピュータプログラマ';

SELECT last_name,first_name, location FROM my_contacts WHERE birthday = '1989/10/12';

SELECT last_name,first_name,email  FROM my_contacts WHERE location = 'youga' AND status = 'single' AND gender = 'F';


SELECT * FROM my_contacts WHERE last_name = 'アン' AND locaton = 'サンフランシスコ' AND gender = 'F';


CREATE TABLE(
       drink_name VARCHAR(20) NOT NULL,
       cost DEC(3,2) NOT NULL,
       carbs DEC(3,2) NOT NULL,
       color VARCHAR(5) NOT NULL,
       ice CHAR(1) NOT NULL,
       calories INT NOT NULL
);

CREATE TABLE drink_info (
       drink_name VARCHAR(20),
       cost DEC(3,2),
       carbs DEC(3,2),
       color VARCHAR(5),
       ice CHAR(1),
       calories INT
);

INSERT INTO drink_info VALUES('ブラックソーン',3,8.4,'黄','Y',33);
INSERT INTO drink_info VALUES('オーマイゴッシュ',3.5,8.6,'橙','Y',12);

SELECT drink_name FROM drink_info
WHERE cost >= 3.5
AND calories < 50;

SELECT drink_name FROM drink_info
WHERE ice = 'Y'
AND color ='黄'
AND carories > 33;

SELECT drink_name,color FROM drink_info
WHERE ice = 'Y'
AND carbs < 4;

SELECT cost FROM drink_info
WHERE calories > 80;

SELECT ice FROM drink_info
WHERE drink_name = 'グレイハウンド'
OR drink_name = 'キスオンザリップス'; 

SELECT drink_name FROM drink_info 
WHERE drink_name >= 'ブ'　
AND
drink_name <= 'プ';

SELECT drink_name FROM easy_drinks WHERE main = 'orangejuice' OR main = 'applejuice';

SELECT drink_name FROM drink_info
WHERE calories = NULL;

New Jersey
New York,
Elsie,
Head First,
WHERE location Like 'spl%',
Blender ,
WHERE state Like 'M%' OR state LIKE 'A%',
John joshua,
WHERE word Like '_i%';

SELECT drink_name FROm drink_info 
WHERE calories BETWEEN 30 AND 60;

SELECT drink_name FROm drink_info 
WHERE calories < 30 OR calories > 60;

SELECT drink_name FROm drink_info 
WHERE drink_name BETWEEN 'カ' AND 'ブ';

SELECT drink_name FROM drink_info
WHERE NOT carbs BETWEEN 3 AND 5;

SELECT date_name from black_book
WHERE NOT date_name LIKE 'ア%' 
AND NOT date_name LIKE 'い%';

SELECT drink_name from easy_drinks
WHERE amount1 >= 1.5;

SELECT drink_name from easy_drinks
WHERE ice = 'N';

SELECT drink_name from easy_drinks
WHERE calories >= 20;

SELECT drink_name from easy_drinks
WHERE main IN ('チェリージュース','トニックウォーター');

SELECT drink_name from easy_drinks
WHERE calories > 0;

SELECT drink_name from easy_drinks
WHERE carbs < 3 OR carbs > 5;

SELECT drink_name from black_book
WHERE date_name NOT BETWEEN 'ア' AND 'イ';

CREATE TABLE clown_info(
       name VARCHAR(10),
       last_seen VARCHAR(20),
       appearance VARCHAR(30),
       activites VARCHAR(20)
);


INSERT INTO clown_info VALUES('エルシー','シニアセンター','赤い髪','ゴム風船');
INSERT INTO clown_info VALUES('ピックルス','パーティ','黄色いシャツ','巨大な足');
INSERT INTO clown_info VALUES('','','','');
INSERT INTO clown_info VALUES('','','','');
INSERT INTO clown_info VALUES('','','','');
INSERT INTO clown_info VALUES('','','','');

INSERT INTO clown_info VALUES('','','','');
INSERT INTO clown_info VALUES('','','','');

DELETE FROM clown_info WHERE name = 'ジッポ' AND activities IN ('ダンス','歌');

p133
1,2.4,

p136

DELETE FROM drink_info WHERE drink_name = 'キスオンザリップス';
INSERT INTO drink_info VALUES('キスオンザリップス',5.5,42.5,'紫','Y',170); 

DELETE FROM drink_info WHERE color = '黄';
INSERT ...

!DELETE を使用する際には、その前にSELECT文で確認してから行えば安全。

ex
SELECT * FROM clown_info
WHERE
activities = 'dance';

INSERT INTO clown_info
VALUES
('zippo','milstonemole','Female,suits in orage,buggy pants',dance,sing);

DELETE FROM clown_info
WHERE 
activities = 'dance';

UPDATE doughnut_rating
SET 
type = 'グレーズド'
WHERE type = 'プレーングレーズド';

UPDATE clown_info 
SET = 'buggy pants'
WHERE name = 'snaggles';

UPDATE clown_info 
SET last_seen = 'bawlmart'
WHERE name = 'Bonzo';

UPDATE clown_info 
SET activities = 'ride small car'
WHERE name = 'sniffles';

UPDATE clown_info 
SET last_seen = 'dickson park'
WHERE name = 'Mr.Hobo';

UPDATE drink_info
SET cost = cost + 1
WHERE 
drink_name = 'blue moon'
OR 
drink_name = 'Ohmygosh'
OR
drink_name = 'limefiz';



```


