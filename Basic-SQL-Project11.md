1. **actor** ve **customer** tablolarında bulunan **first_name** sütunları için tüm verileri sıralayalım.

```sql
(
SELECT first_name FROM customer
)
UNION 
(
SELECT first_name FROM actor
);
```

2. **actor** ve **customer** tablolarında bulunan **first_name** sütunları için kesişen verileri sıralayalım.

```sql
(
SELECT first_name FROM customer
)
INTERSECT
(
SELECT first_name FROM actor
);
```

3. **actor** ve **customer** tablolarında bulunan **first_name** sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.

```sql
(
SELECT first_name FROM customer
)
EXCEPT
(
SELECT first_name FROM actor
);
```

4. İlk 3 sorguyu tekrar eden veriler için de yapalım. 

   Bunun için ilk soruda "UNION ALL" koymamız, ikinci soruda "INTERSECT ALL" ve son olarak da "EXCEPT ALL" yapabiliriz.
