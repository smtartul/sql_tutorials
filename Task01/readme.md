# Expectations and Request
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
#
>  film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.
><pre><code>SELECT title,description FROM film
</code></pre>
#
> film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.
> <pre><code>SELECT * FROM film WHERE length>60 AND length<75 
</code></pre>
#
> film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.
> <pre><code>SELECT * FROM film WHERE rental_rate=0.99 AND (replacement_cost=12.99 OR replacement_cost=28.99)
</code></pre>
#
> customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?
> <pre><code>SELECT last_name FROM customer WHERE first_name='Mary'
</code></pre>
#
> film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.
> <pre><code>SELECT * FROM film WHERE length<=50 AND (rental_rate!=2.99 AND rental_rate!=4.99)
</code></pre>




