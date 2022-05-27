# Expectations and Request
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
***
> city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
<pre><code>SELECT city,country FROM city INNER JOIN country ON city.country_id=country.country_id
</code></pre>
***
> customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
<pre><code>SELECT payment_id,first_name,last_name FROM payment
INNER JOIN customer ON payment.customer_id=customer.customer_id
</code></pre>
***
> customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
<pre><code>SELECT rental_id,first_name,last_name FROM rental
INNER JOIN customer ON rental.customer_id=customer.customer_id
</code></pre>
