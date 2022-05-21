# GROUP BY USAGE
Benzersiz alanlar ile ilgili birlesik sorgular yaparken gruplama yapabiliriz.


Burada şuna dikkat etmemiz gerekir, SELECT anahtar kelimesinde bulunan sütunların GROUP BY anahtar kelimesi içerisinde bulunması gerekir.


<pre><code>SELECT rental_rate,MAX(length) FROM film GROUP BY rental_rate
</code></pre>
> Her bir rental_rate karsilik gelen en uzun film sonucunu elde ederiz.
***
<pre><code>SELECT rental_rate,COUNT(*) FROM film GROUP BY rental_rate
</code></pre>
> Her bir rental_rate karsilik gelen film sayisini elde ederiz.
<pre><code>SELECT rating,COUNT(*) FROM film GROUP BY rating
</code></pre>
> Her bir ratinge karsilik gelen film sayisini elde ederiz.


<pre><code>SELECT replacement_cost,rental_rate, MIN(length) FROM film GROUP BY replacement_cost,rental_rate ORDER BY replacement_cost
</code></pre>