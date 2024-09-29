Q1)
Select country.name as "country name", airport.name as "airport name" from country inner join airport on airport.iso_country = country.iso_country where country.name = "Finland"and scheduled_service = "yes";
![EXE$Q1.png](EXE%24Q1.png)


Q2)
select screen_name,airport.name from game inner join airport on location = ident;
![Ex4Q2.png](Ex4Q2.png)


Q3)
select screen_name,country.name from game inner join airport on location = ident inner join country on airport.iso_country=country.iso_country
![Ex4Q3.png](Ex4Q3.png)

Q4)

select airport.name, screen_name from airport left join game on ident = location where airport.name like "%Hels%";
![Ex4Q4.png](Ex4Q4.png)

q5)
select name, screen_name from goal left join goal_reached on goal.id = goal_id left join game on game.id = game_id;
![Ex4Q5.png](Ex4Q5.png)

 