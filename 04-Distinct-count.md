# DISTINCT & COUNT
<pre><code>SELECT DISTINCT rental_rate FROM film</code></pre>
> ilgili sutundaki benzersiz verileri gosterir.
***
<pre><code>SELECT DISTINCT first_name,last_name FROM actor</code></pre>
***
<pre><code>SELECT COUNT(*) FROM actor WHERE first_name='Penelope'</code></pre>
> sorgu sonucu ortaya cikan verilerin sayisini gosterir.
***
<pre><code>SELECT COUNT(DISTINCT first_name) FROM actor</code></pre>

