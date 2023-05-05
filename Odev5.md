## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

* film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
* film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
* customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.

---

```sql
1. SELECT title,length FROM film 
   WHERE title ilike '%n'
   ORDER BY length DESC
   LIMIT 5;
```
```sql
2. SELECT title FROM film
   WHERE title ILIKE '%n'
   ORDER BY length
   OFFSET 5
   LIMIT 5;
```
```sql
3. SELECT last_name FROM customer
   WHERE store_id = 1
   ORDER BY last_name DESC
   LIMIT 4;
```