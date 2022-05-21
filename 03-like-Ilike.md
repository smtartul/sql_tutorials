# LIKE & ILIKE 
<pre><code>SELECT * FROM actor WHERE first_name LIKE 'P%' </code></pre>
> - '%' karakteri sifir,bir veya daha fazla karakteri temsil eder. Wildcard olarak isimlendirilir.
> - '_' karakteri bir karakteri temsil eder.
> - 'ILIKE' case - insensitive versiyondur.
***
<pre><code>SELECT * FROM actor WHERE first_name LIKE '%Pen%' </code></pre>
<pre><code>SELECT * FROM actor WHERE first_name LIKE 'P_n%' </code></pre>