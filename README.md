# City_Population
Given the CITY and COUNTRY tables, query the sum of the populations of all cities where the CONTINENT is 'Asia'.  Note: CITY.CountryCode and COUNTRY.Code are matching key columns.


SELECT SUM(a.POPULATION) 
FROM CITY a 
JOIN COUNTRY b
ON a.COUNTRYCODE = b.CODE
WHERE b.CONTINENT = 'Asia'
    ;
