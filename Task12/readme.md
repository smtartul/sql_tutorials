# Expectations and Request
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
***
> film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
<pre><code>SELECT COUNT(*) FROM film 
WHERE length>
(
SELECT AVG(length) FROM film
) 
</code></pre>
***
> film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?

<pre><code>SELECT COUNT(*) FROM film 
WHERE rental_rate =
(
SELECT MAX(rental_rate) FROM film
)
</code></pre>
***
> film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.

<pre><code>SELECT title,rental_rate,replacement_cost FROM film 
WHERE rental_rate=(SELECT MIN(rental_rate) FROM film) 
AND replacement_cost=(SELECT MIN(replacement_cost) FROM film)

</code></pre>
***
> payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

<pre><code>SELECT first_name,last_name FROM customer WHERE customer_id=ANY
(SELECT customer_id FROM payment WHERE amount=
(SELECT MAX(amount) FROM payment))
</code></pre>
***