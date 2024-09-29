#week 3, Exercise 2

### Q1
Select * form goal;
![quetion1 ex2.png](quetion1%20ex2.png)

### Q2
select name,type from airport where iso_country = "FI";
![Ex2q2.png](Ex2q2.png)

### Q3
select * from airport where iso_country = "FI" order by name asc;
![Ex3Q3.png](Ex2Q3.png)


### Q4
select name,type from airport where iso_country = "FI" order by type asc;
![Ex2q4.png](Ex2q4.png)


### Q5
select name from country where name like 'F%';
![Ex2Q5.png](Ex2Q5.png)

### Q6
select name from country where name like "%F%";
![Ex2q6.png](Ex2q6.png)


### Q7
select location from game where screen_name = "Vesa";
![Ex2q7.png](Ex2q7.png)


### Q8
select co2_consumed from game where screen_name = "Ilkka";
![Ex2Q8.png](Ex2Q8.png)

### Q9
select DISTINCT co2_budget from game;
![Ex2Q9.png](Ex2Q9.png)


### Q10
select screen_name,co2_budget,co2_consumed,co2_budget-co2_consumed as co2_left from game where screen_name = "Ilkka";
![Ex2Q10.png](Ex2Q10.png)
