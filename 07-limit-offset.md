# LIMIT & OFFSET
<b>LIMIT</b><i> Veri sayisinin ust limitini belirtmek icin kullanilir. /take data
*** 
<b>OFFSET</b><i> Baslangictan itibaren kac birim verinin pass gecilecegini belirtir. /skip data
***
<pre><code>SELECT * FROM film
WHERE title LIKE 'B%'
ORDER BY length DESC
OFFSET 6
LIMIT 4;
</code></pre>