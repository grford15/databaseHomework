Answer 1 :

marvel=# SELECT * FROM movies;
 id |                title                | year | show_time
----+-------------------------------------+------+-----------
  1 | Iron Man                            | 2008 | 23:00
  2 | The Incredible Hulk                 | 2008 | 18:05
  3 | Iron Man 2                          | 2010 | 21:25
  4 | Thor                                | 2011 | 14:40
  5 | Captain America: The First Avenger  | 2011 | 13:25
  6 | Avengers Assemble                   | 2012 | 22:45
  7 | Iron Man 3                          | 2013 | 19:00
  8 | Thor: The Dark World                | 2013 | 19:50
  9 | Batman Begins                       | 2005 | 13:45
 10 | Captain America: The Winter Soldier | 2014 | 16:00
 11 | Guardians of the Galaxy             | 2014 | 16:50
 12 | Avengers: Age of Ultron             | 2015 | 23:55
 13 | Ant-Man                             | 2015 | 18:40
 14 | Captain America: Civil War          | 2016 | 16:15
 15 | Doctor Strange                      | 2016 | 12:20
 16 | Guardians of the Galaxy 2           | 2017 | 22:25
 17 | Spider-Man: Homecoming              | 2017 | 22:25
 18 | Thor: Ragnarok                      | 2017 | 16:30
 19 | Black Panther                       | 2018 | 15:00
(19 rows)

Answer 2:

marvel=# SELECT name FROM people;
         name          

 Angelina Blyth
 Steven Bonner
 Matthew Bryce
 Stephan Constantial
 Roddy Daly
 Adri Forczek
 David Fulton
 Derek Leach
 Craig McDowall
 Tara McKeaney
 Cambel Millar
 Farheen Mulla
 Jack Murning
 Richard Phillips-Kerr
 Joe Pollock
 Alan Russell
 Greg Rutherford
 Harjit Singh
 Debi Skea
 Cleyra Uzcategui
 Peter Whittle


 Answer 3:

 marvel=# UPDATE people SET name = ('Campbell Miller') WHERE name = 'Cambel Millar';
UPDATE 1

Answer 4:

marvel=# SELECT FROM people where name = 'Greg Rutherford';
--
(1 row)

Answer 5:

marvel=# DELETE FROM movies where title = 'Batman Begins';
DELETE 1

Answer 6:

marvel=# INSERT INTO people (name) VALUES ('Colin Bell');
INSERT 0 1

Answer 7:

marvel=# DELETE FROM people WHERE name = 'Alan Russell';
DELETE 1

Answer 8:

marvel=# INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '00:00');
INSERT 0 1

Answer 9:

marvel=# UPDATE movies SET show_time = '20:00' WHERE show_time = '16:50';
UPDATE 1

Extension -

marvel=# DELETE FROM movies WHERE id = 17 OR id = 18;
DELETE 2
