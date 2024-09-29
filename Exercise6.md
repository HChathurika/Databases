q1)
select continent, count(*) from country group by continent;
![Ex6Q1.png](Ex6Q1.png)

q2)
select continent, count(*) from country group by continent;
![Ex6Q2.png](Ex6Q2.png)


q3)
select screen_name, count(*) from game, goal_reached where id = game_id group by screen_name;
![Ex6Q3.png](Ex6Q3.png)


q4)
select screen_name from game where co2_consumed in(select min(co2_consumed) from game );
![Ex6Q4.png](Ex6Q4.png)

q5)
select country.name, count(*) from airport, country where airport.iso_country = country.iso_country group by country.iso_country order by count(*) desc limit 50;
![Ex6Q5.png](Ex6Q5.png)

q6)
select country.name from airport, country where airport.iso_country = country.iso_country group by country.iso_country having count(*) > 1000;
![Ex6Q6.png](Ex6Q6.png)


q7)
select name from airport where elevation_ft in ( select max(elevation_ft)from airport);
![Ex6Q7.png](Ex6Q7.png)

q8)
select name from country where iso_country in ( select iso_country from airport where elevation_ft in( select max(elevation_ft) from airport ) );
![Ex6Q8.png](Ex6Q8.png)

Q9)
select count(*) from game, goal_reached where id = game_id and screen_name = "Vesa" group by screen_name;