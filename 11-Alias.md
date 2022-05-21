# ALIAS (AS) USAGE
AS anahtar kelimesi sayesinde sorgular sonucu oluşturduğumuz sanal tablo ve sütunlara geçici isimler verebiliriz.

<pre><code>SELECT COUNT(*) AS "aktor sayisi" FROM actor</code></pre>
> olusturulan sanal tabloya isim verilmis oldu.
***

<pre><code>SELECT CONCAT(first_name,' ',last_name) AS "full name" FROM actor</code></pre>
> iki sutun birlestirilip db de tutulmayan sanal sutuna isim verildi.
***
