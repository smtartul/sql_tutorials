

<pre><code>SELECT *
FROM film
WHERE length NOT BETWEEN 100 AND 140
</code></pre>
> Not;Burada dikkat edilmesi gereken nokta 100 ve 140 sınır değerleri aralığa dahildir.
#
<pre><code>SELECT *
FROM film
WHERE length IN (30,60,90,120);
</code></pre>
> length=30 OR length=60 OR ...
#