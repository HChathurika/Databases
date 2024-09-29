q1)
select name from country where iso_country in (select iso_country from airport where name like "Satsuma%");
![Ex5Q1.png](Ex5Q1.png)

q2)
select name from airport where iso_country in (select iso_country from country where country.name = "Monaco");
![Ex5Q2.png](Ex5Q2.png)


q3)
Select screen_name from game where id in(select game_id from goal_reached where goal_id in(select id from goal where name ="CLOUDS"));
![Ex5Q3.png](Ex5Q3.png)


q4)
Select country.name from country where iso_country not in (select airport.iso_country from airport);
![Ex5Q4.png](Ex5Q4.png)


q5)
Select country.name from country where iso_country not in (select airport.iso_country from airport);
![Ex5Q5.png](Ex5Q5.png)