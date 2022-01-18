#Challenges
#1
Select * FROM city where name = 'washington';
Select Count(name) From city WHERE CountryCode = 'USA';

#2
Select name, population, LifeExpectancy From Country Where name LIKE 'Arg%';

#3
Select name, LifeExpectancy From Country Where LifeExpectancy = (
Select MAX(LifeExpectancy) From Country) ORDER BY name LIMIT 1;

#4
Select * from Country;
SELECT * FROM City JOIN Country ON city.countrycode = country.code WHERE City.name = 'Madrid';

#5
select * FROM countrylanguage;
SELECT name, language, region FROM countrylanguage JOIN country 
ON country.code = countrylanguage.countrycode Where country.region = 'southeast asia';

#6
SELECT * FROM city ORDER BY ID ASC Limit 25;

#7
Select Count(Country.name) AS 'Number of chinese Cities' FROM City Join Country ON city.countrycode = country.code WHERE Country.Name = 'China';

#8
SELECT Name, Population FROM country Where population IS NOT NULL AND population > 0 order by population LIMIT 10; 

#9
SELECT count(country.name) AS 'Total Number Of Countries' FROM country; 

#10
SELECT name, SurfaceArea From Country Order by SurfaceArea DESC LIMIT 10;

#11
Select City.name, city.population From city WHERE CountryCode = 'JPN' ORDER BY population DESC LIMIT 5;

#12
Select country.name, country.code, headofstate FROM country Where country.headofstate = 'Elisabeth II';

#13
#Dunno

#14
Select Distinct language AS 'Every Unique Language' From CountryLanguage;

#15
Select name, GNP FROM country ORDER BY GNP DESC LIMIT 10;

#16
Select name, count(name) as numOfLang
From countrylanguage Join country ON countrylanguage.countrycode = country.code group by country.name order by numOfLang desc limit 10;

#17
##Percentages unsure

#18
Select name, LifeExpectancy FROM Country Where LifeExpectancy > 0 ORDER BY LifeExpectancy ASC LIMIT 1;

#19
SELECT Name, count(NAME) as numofstate
From country order by numofstate ASC LIMIT 3;
##not quite working

#20
## ran out of time# SQLAnswers
SQLAnswers Challenge
