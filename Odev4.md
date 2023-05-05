## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

* film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
* film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
* film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
* country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
* city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

---

```sql
1. SELECT DISTINCT replacement_cost FROM film;
```
```sql
2. SELECT COUNT(DISTINCT replacement_cost) FROM film;
```
```sql
3. SELECT title, rating FROM film
   WHERE title LIKE 'T%' AND rating = 'G';
```
```sql
4. SELECT city FROM city
   WHERE city ILIKE '%r';
```