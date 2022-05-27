# PSQL COMMANDS


<pre><code>psql -U postgres -p 5433</code></pre>
***

Yeni db olusturmak icin;
<pre><code>CREATE DATABASE testdb</code></pre>

Yeni tablo olusturmak icin;
<pre><code>CREATE TABLE users
(id SERIAL PRIMARY KEY,
username VARCHAR(50) NOT NULL,
birthday DATE);
</code></pre>

Tablo listesi icin
<pre><code>\dt</code></pre>

Tablo detayi icin
<pre><code>\d+ users</code></pre>

Sutun guncelleme icin
<pre><code>ALTER TABLE users RENAME COLUMN birthday TO date;</code></pre>

Tablo detayi icin
<pre><code>\d+ users</code></pre>