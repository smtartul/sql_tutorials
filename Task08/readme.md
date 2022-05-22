# Expectations and Request
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
***
> test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

<pre><code>CREATE TABLE employee (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    email VARCHAR(100),
    birthday DATE
);
</code></pre>
***
> Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

<pre><code>
insert into employee (name, email, birthday) values ('Kazio', 'sarnoll0@infoseek.co.jp', '1972-03-30');
insert into employee (name, email, birthday) values ('Twitterbeat', 'rmocher1@nsw.gov.au', '1952-09-13');
insert into employee (name, email, birthday) values ('Pixoboo', 'ddadley2@e-recht24.de', '1915-08-18');
insert into employee (name, email, birthday) values ('Centizu', 'tcohane3@multiply.com', '1923-07-20');
insert into employee (name, email, birthday) values ('Skyvu', 'rfourman4@linkedin.com', '1939-08-25');
insert into employee (name, email, birthday) values ('Youtags', 'enoe5@amazon.com', '1976-11-05');
insert into employee (name, email, birthday) values ('Eadel', 'emum6@privacy.gov.au', '1986-12-03');
insert into employee (name, email, birthday) values ('Kimia', 'wwaterdrinker7@discovery.com', '1915-09-05');
insert into employee (name, email, birthday) values ('Talane', 'amoses8@japanpost.jp', '1947-05-25');
insert into employee (name, email, birthday) values ('Topicblab', 'bneillans9@mashable.com', '1914-10-28');
insert into employee (name, email, birthday) values ('DabZ', 'scasforda@twitter.com', '2008-04-29');
insert into employee (name, email, birthday) values ('Trudeo', 'ealexsandrovb@theguardian.com', '2006-11-23');
insert into employee (name, email, birthday) values ('Vinder', 'oklejnac@ucoz.com', '2001-06-07');
insert into employee (name, email, birthday) values ('Thoughtmix', 'mthomannd@tripadvisor.com', '1916-02-05');
insert into employee (name, email, birthday) values ('Jamia', 'obramelte@businessweek.com', '1936-04-03');
insert into employee (name, email, birthday) values ('Dynabox', 'kbrabhamf@macromedia.com', '1975-12-10');
insert into employee (name, email, birthday) values ('Browsedrive', 'ctwopennyg@sciencedaily.com', '1920-02-08');
insert into employee (name, email, birthday) values ('Jayo', 'mbosdenh@desdev.cn', '1974-06-23');
insert into employee (name, email, birthday) values ('Gigazoom', 'tjoyei@pcworld.com', '1991-02-03');
insert into employee (name, email, birthday) values ('Divape', 'alavellj@wired.com', '2008-08-01');
insert into employee (name, email, birthday) values ('Wordtune', 'delvyk@omniture.com', '1915-12-31');
insert into employee (name, email, birthday) values ('Jaxbean', 'jnaerupl@sciencedirect.com', '2013-06-13');
insert into employee (name, email, birthday) values ('Lazzy', 'csweetenhamm@samsung.com', '1988-10-13');
insert into employee (name, email, birthday) values ('Photobug', 'tcornboroughn@apache.org', '2015-01-13');
insert into employee (name, email, birthday) values ('Jabbertype', 'hgirdlestoneo@i2i.jp', '2006-11-15');
insert into employee (name, email, birthday) values ('Topicstorm', 'mprantonip@shareasale.com', '2022-01-01');
insert into employee (name, email, birthday) values ('Youspan', 'mcarrq@sfgate.com', '1923-12-11');
insert into employee (name, email, birthday) values ('Tanoodle', 'esulllyr@symantec.com', '1986-03-11');
insert into employee (name, email, birthday) values ('Camimbo', 'vkeelings@topsy.com', '1941-09-24');
insert into employee (name, email, birthday) values ('Trilia', 'elilfordt@independent.co.uk', '1996-10-01');
insert into employee (name, email, birthday) values ('Avamba', 'wgainu@ted.com', '1966-10-30');
insert into employee (name, email, birthday) values ('Twitternation', 'bvernhamv@tuttocitta.it', '1954-03-29');
insert into employee (name, email, birthday) values ('Fliptune', 'aturnbullw@answers.com', '1933-04-28');
insert into employee (name, email, birthday) values ('Rooxo', 'dbraunx@hc360.com', '1918-08-26');
insert into employee (name, email, birthday) values ('Shufflester', 'gimessony@people.com.cn', '2015-02-06');
insert into employee (name, email, birthday) values ('Kayveo', 'nbettesonz@privacy.gov.au', '1942-03-26');
insert into employee (name, email, birthday) values ('Rooxo', 'nfowells10@t.co', '1942-10-22');
insert into employee (name, email, birthday) values ('Rhybox', 'adiplock11@fda.gov', '2002-01-12');
insert into employee (name, email, birthday) values ('Jaxspan', 'ebrokenshire12@flavors.me', '1933-06-08');
insert into employee (name, email, birthday) values ('Tambee', 'jpatterson13@webmd.com', '1964-12-12');
insert into employee (name, email, birthday) values ('Twinte', 'lrevens14@forbes.com', '1973-07-23');
insert into employee (name, email, birthday) values ('Pixoboo', 'kmatveyev15@mediafire.com', '1994-11-30');
insert into employee (name, email, birthday) values ('Oyope', 'kguymer16@wikimedia.org', '1956-08-04');
insert into employee (name, email, birthday) values ('Shufflebeat', 'prelfe17@naver.com', '1973-03-23');
insert into employee (name, email, birthday) values ('Devify', 'amckerrow18@mapquest.com', '2021-06-25');
insert into employee (name, email, birthday) values ('Realfire', 'cfarnill19@prnewswire.com', '1990-01-02');
insert into employee (name, email, birthday) values ('Youtags', 'mfearnyough1a@wufoo.com', '1935-11-20');
insert into employee (name, email, birthday) values ('Livetube', 'cmeconi1b@google.com', '2019-11-27');
insert into employee (name, email, birthday) values ('Blogtags', 'gvalentine1c@yale.edu', '1965-10-18');
insert into employee (name, email, birthday) values ('Tanoodle', 'zlashford1d@prnewswire.com', '1960-10-25');
</code></pre>
***
> Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

1. <pre><code>UPDATE employee SET name='XXX', birthday='2000-01-01', email='xx@yy.com' WHERE id=2
</code></pre>

2. <pre><code>UPDATE employee SET name='XXX' WHERE id BETWEEN 11 AND 15
</code></pre>

3. <pre><code>UPDATE employee SET name='YYY' WHERE name='XXX'
</code></pre>

4. <pre><code>UPDATE employee SET email=NULL WHERE email LIKE '%mapy%'
</code></pre>

5. <pre><code>UPDATE employee SET email=NULL WHERE email LIKE '%.com'
</code></pre>

> Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

1. <pre><code>DELETE FROM employee WHERE id=1
</code></pre>

2. <pre><code>DELETE FROM employee WHERE name='XXX'
</code></pre>

3. <pre><code>DELETE FROM employee WHERE id BETWEEN 5 AND 10
</code></pre>

4. <pre><code>DELETE FROM employee WHERE name LIKE 'A%'
</code></pre>

5. <pre><code>DELETE FROM employee WHERE email LIKE '%gmail%'
</code></pre>