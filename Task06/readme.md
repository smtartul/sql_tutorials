# Expectations and Request
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
***
1. <pre><code> SELECT AVG(rental_rate) FROM film</code></pre>
    > film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
***
2. <pre><code>SELECT COUNT(rental_rate) FROM film WHERE title LIKE 'C%'</code></pre>
    > film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
***
3. <pre><code>SELECT MAX(length) FROM film WHERE rental_rate=0.99</code></pre>
    > film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
***
4. <pre><code>SELECT COUNT(DISTINCT replacement_cost ) FROM film WHERE length>150</code></pre>
    > film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
***
