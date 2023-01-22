# SQL-HCKERRANK-PROBLEMS
## Weather Observation Station 2

Query the following two values from the STATION table:

The sum of all values in LAT_N rounded to a scale of  decimal places.
The sum of all values in LONG_W rounded to a scale of  decimal places.
![image](https://user-images.githubusercontent.com/101393263/213937138-c1d2dc29-0e4c-4015-bf33-f5ad6c581f49.png)
where LAT_N is the northern latitude and LONG_W is the western longitude.

Output Format

Your results must be in the form:

lat lon
where  is the sum of all values in LAT_N and  is the sum of all values in LONG_W. Both results must be rounded to a scale of  decimal places.

USE MYSQL to solve this problem
SELECT CONCAT(ROUND(SUM(LAT_N), 2), ' ', ROUND(SUM(LONG_W), 2)) AS 'lat lon'
FROM STATION;

or 
SELECT ROUND(SUM(LAT_N), 2) AS LAT_N_SUM, ROUND(SUM(LONG_W), 2) AS LONG_W_SUM
FROM STATION;

