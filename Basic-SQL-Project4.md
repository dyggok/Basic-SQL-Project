# Basic-SQL-Project4

Aşağıdaki sorgu senaryoları dvdrental örnek veri tabanı üzerinden gerçekleştirilmiştir.

1. **film** tablosunda bulunan **replacement_cost** sütununda bulunan birbirinden farklı değerleri sıralayınız.

```sql
SELECT DISTINCT replacement_cost FROM film;
```

2. **film** tablosunda bulunan **replacement_cost** sütununda birbirinden farklı kaç tane veri vardır?

```sql
SELECT COUNT(DISTINCT replacement_cost) FROM film;
```

3. **film** tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?

```sql
SELECT COUNT(title) FROM film WHERE title LIKE 'T%'
AND rating = 'G';
```

4. **country** tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

```sql
SELECT COUNT(country) FROM country WHERE country LIKE '_____';
```

ya da  şu şekilde yazılır;

```sql
SELECT COUNT(country) FROM country WHERE LENGTH(country) = 5;
```

5. **city** tablosundaki şehir isimlerinin kaçtanesi 'R' veya r karakteri ile biter?

```sql
SELECT COUNT(city) FROM city WHERE city ILIKE '%r'
```