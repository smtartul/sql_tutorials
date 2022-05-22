# CREATE

<pre><code>CREATE TABLE author (
    id SERIAL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100),
    birthday DATE
);
</code></pre>

# DROP

Burada IF EXISTS yapısını kullanarak yanlış tablo ismi yazımı durumunda hata mesajı almayı önleriz.


<pre><code>DROP TABLE IF EXIST test
</code></pre>

# INSERT INTO

Mevcut tabloya yeni veri girisi;


<pre><code>INSERT INTO author (first_name,last_name,email,birthday) VALUES 
('Orhan','Pamuk','orhan@pamuk.com','1950-11-22'),
('Halide Edip','Adivar','hedip@adivar.com','1950-11-22'),
('Sabahattin','Ali','sabahattin@ali.com','1950-11-22');

</code></pre>

Kopyalama islemi ise:
<pre><code>CREATE TABLE author2 (LIKE author);
</code></pre>
<pre><code>INSERT INTO author2 SELECT * FROM author WHERE first_name='Orhan';
</code></pre>
***
Mevcut data table yedegi alinir;
<pre><code>CREATE TABLE author3 AS SELECT * FROM author
</code></pre>
