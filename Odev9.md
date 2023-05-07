## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

* city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
* customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
* customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

---

```sql
1. SELECT city,country FROM city 
   INNER JOIN country ON city_id = country.country_id;
```
```sql
2. SELECT payment.payment_id,
   customer.first_name,
   customer.last_name     FROM customer
   INNER JOIN payment ON customer.customer_id=payment.customer_id;
```
```sql
3. SELECT rental.rental_id, 
   customer.first_name, 
   customer.last_name FROM customer
   INNER JOIN rental ON rental.customer_id = customer.customer_id;
```