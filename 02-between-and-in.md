

`SELECT * FROM film WHERE length NOT BETWEEN 100 AND 140`

> Not;Burada dikkat edilmesi gereken nokta 100 ve 140 sınır değerleri aralığa dahildir.
***
`SELECT * FROM film WHERE length IN (30,60,90,120)`
> length=30 OR length=60 OR ...
