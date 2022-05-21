`SELECT * FROM actor WHERE first_name LIKE 'P%' `
> - '%' karakteri sifir,bir veya daha fazla karakteri temsil eder. Wildcard olarak isimlendirilir.
> - '_' karakteri bir karakteri temsil eder.
> - 'ILIKE' case - insensitive versiyondur.
***
`SELECT * FROM actor WHERE first_name LIKE '%Pen%' `
`SELECT * FROM actor WHERE first_name LIKE 'P_n%' `