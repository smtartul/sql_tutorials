# AGGREGATE FUNCTIONS
## AVG
AVG fonksiyonunu kullandığımız sayısal değerlerden oluşan sütunun ortalama değerini alırız.
<pre><code>SELECT AVG(length) FROM film
</code></pre>
## SUM
SUM fonksiyonunu kullandığımız sayısal değerlerden oluşan sütunun toplam değerini alırız.
<pre><code>SELECT SUM(length) FROM film
</code></pre>
## MAX
MAX fonksyionu sayisal degerlerden olusan sutundaki en yuksek degeri alir.
<pre><code>SELECT MAX(length) FROM film
</code></pre>
<pre><code>SELECT ROUND(MAX(length),3) FROM film
</code></pre>
## MIN
MIN fonksyionu sayisal degerlerden olusan sutundaki en dusuk degeri alir.
<pre><code>SELECT MIN(length) FROM film
</code></pre>