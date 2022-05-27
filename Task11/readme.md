# Expectations and Request
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
***
> actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.
<pre><code>(SELECT first_name FROM actor) 
UNION
(SELECT first_name FROM customer) 
</code></pre>
<pre><code>(SELECT first_name FROM actor) 
UNION ALL
(SELECT first_name FROM customer) 
</code></pre>
***
> actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.
<pre><code>(SELECT first_name FROM actor) 
INTERSECT
(SELECT first_name FROM customer) 
</code></pre>
<pre><code>(SELECT first_name FROM actor) 
INTERSECT ALL
(SELECT first_name FROM customer) 
</code></pre>
***
> actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
<pre><code>(SELECT first_name FROM actor) 
EXCEPT
(SELECT first_name FROM customer) 
</code></pre>
<pre><code>(SELECT first_name FROM actor) 
EXCEPT ALL
(SELECT first_name FROM customer) 
</code></pre>
***
