## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

* film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
* film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
* customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir? 
* city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.

---

```sql
1. SELECT rating FROM film
   GROUP BY rating;
```
```sql
2. SELECT replacement_cost,COUNT(*) FROM film
   GROUP BY replacement_cost
   HAVING COUNT(*) > 50;
```
```sql
3. SELECT store_id,COUNT(*) FROM customer
   GROUP BY store_id;
```
```sql
4. SELECT country_id,COUNT(city) FROM city
   GROUP BY country_id
   ORDER BY COUNT(city) DESC
   LIMIT 1;
```