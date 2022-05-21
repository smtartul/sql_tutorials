# HAVING USAGE
WHERE sorgulari satir bazli olup gruplanmis sorgulari HAVING ile yapiyoruz.

<pre><code>SELECT customer_id,SUM(amount) FROM payment GROUP BY customer_id 
HAVING SUM(amount) >100 ORDER BY SUM(amount) DESC
</code></pre>
> Her bir customer_id karsilik gelen toplam satis tutarinin 100 uzerinde olanlari azalan sekilde siralamis olduk.
***
