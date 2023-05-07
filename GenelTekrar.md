## Bu çalışmamamızda şimdiye kadar üzerine konuştuğumuz tüm konuları 5 farklı senaryo üzerinden tekrar etmeye çalıştık. Aşağıda ilgili senaryoları bulabilirsiniz.

* film tablosundan 'K' karakteri ile başlayan en uzun ve replacenet_cost u en düşük 4 filmi sıralayınız.
* film tablosunda içerisinden en fazla sayıda film bulunduran rating kategorisi hangisidir?
* cutomer tablosunda en çok alışveriş yapan müşterinin adı nedir?
* category tablosundan kategori isimlerini ve kategori başına düşen film sayılarını sıralayınız.
* film tablosunda isminde en az 4 adet 'e' veya 'E' karakteri bulunan kç tane film vardır?

---

```sql
1. SELECT title,length,replacement_cost FROM film
   WHERE title LIKE 'K%'
   ORDER BY length DESC,replacement_cost ASC
   LIMIT 4;
```
```sql
2. SELECT COUNT(*),rating FROM film
   GROUP BY rating
   ORDER BY COUNT(*) DESC
   LIMIT 1;
```
```sql
3. SELECT SUM(amount),
   customer.first_name, 
   customer.last_name FROM payment
   JOIN customer ON customer.customer_id = payment.customer_id
   GROUP BY payment.customer_id,customer.first_name, customer.last_name
   ORDER BY SUM(amount) DESC;
```
```sql
4. SELECT COUNT(*),category.name FROM category
   JOIN film_category 
   ON film_category.category_id = category.category_id
   JOIN film ON film.film_id = film_category.film_id
   GROUP BY category.name;
```
```sql
5. SELECT COUNT(*) FROM film
   WHERE title ILIKE '%e%e%e%e%'
   ORDER BY COUNT(*);
```
