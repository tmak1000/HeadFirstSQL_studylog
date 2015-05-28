#chapter6

```
UPDATE my_table

SET new_column = 
CASE
	WHEN column1 = somevalue1
	     THEN newvalue1
	WHEN column2 = somevalue2
	     THEN newvalue2
	ELSE
		newvalue3
END;

UPDATE movie_table
SET category = 
CASE
	WHEN drama = 'T' TEHN 'drama'
	WHEN comedy = 'T' THEN 'comedy'
	ELSE 'other'
END;

P245


```