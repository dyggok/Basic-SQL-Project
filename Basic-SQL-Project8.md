# Basic-SQL-Project8

1. **test** veritabanınızda **employee** isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

```sql
CREATE TABLE employee (
	id SERIAL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(50),
	birthday DATE
);
```

2. Oluşturduğumuz **employee** tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```sql
insert into Employee (first_name, last_name, email, birthday) values ('Clemmie', 'Bastable', 'cbastable0@bbb.org', '1964-12-09');
insert into Employee (first_name, last_name, email, birthday) values ('Boone', 'Sturt', 'bsturt1@weather.com', '1969-08-10');
insert into Employee (first_name, last_name, email, birthday) values ('Merline', 'Leffek', 'mleffek2@plala.or.jp', '1994-10-15');
insert into Employee (first_name, last_name, email, birthday) values ('Bondy', 'Chivrall', 'bchivrall3@1und1.de', '1998-10-11');
insert into Employee (first_name, last_name, email, birthday) values ('Elnore', 'Billingsly', 'ebillingsly4@loc.gov', '1977-06-21');
insert into Employee (first_name, last_name, email, birthday) values ('Bud', 'Beenham', 'bbeenham5@dion.ne.jp', '1972-08-31');
insert into Employee (first_name, last_name, email, birthday) values ('Yasmeen', 'Agney', 'yagney6@cbslocal.com', '1985-03-10');
insert into Employee (first_name, last_name, email, birthday) values ('Sig', 'Harler', 'sharler7@cyberchimps.com', null);
insert into Employee (first_name, last_name, email, birthday) values ('Orella', 'Cattonnet', 'ocattonnet8@youtu.be', '1981-10-10');
insert into Employee (first_name, last_name, email, birthday) values ('Gordy', 'McGurn', null, '1996-08-09');
insert into Employee (first_name, last_name, email, birthday) values ('Saidee', 'Mowsdale', null, '1961-09-14');
insert into Employee (first_name, last_name, email, birthday) values ('Genia', 'Cardillo', 'gcardillob@va.gov', '1973-10-31');
insert into Employee (first_name, last_name, email, birthday) values ('Casandra', 'Oade', 'coadec@discovery.com', '1963-07-18');
insert into Employee (first_name, last_name, email, birthday) values ('Donal', 'Kilpin', 'dkilpind@boston.com', '2015-08-28');
insert into Employee (first_name, last_name, email, birthday) values ('Demetris', 'Ram', 'drame@engadget.com', null);
insert into Employee (first_name, last_name, email, birthday) values ('Lida', 'Rundall', null, '2015-11-06');
insert into Employee (first_name, last_name, email, birthday) values ('Jorry', 'Goalby', 'jgoalbyg@naver.com', '2018-03-22');
insert into Employee (first_name, last_name, email, birthday) values ('Feodor', 'Giovanardi', 'fgiovanardih@ftc.gov', '1962-12-23');
insert into Employee (first_name, last_name, email, birthday) values ('Kai', 'Corbet', 'kcorbeti@virginia.edu', '1994-07-03');
insert into Employee (first_name, last_name, email, birthday) values ('Hadleigh', 'Downton', null, '1987-05-17');
insert into Employee (first_name, last_name, email, birthday) values ('Ellswerth', 'Smowton', 'esmowtonk@i2i.jp', null);
insert into Employee (first_name, last_name, email, birthday) values ('Johnathan', 'Orsay', 'jorsayl@wired.com', '1982-02-23');
insert into Employee (first_name, last_name, email, birthday) values ('Kenneth', 'Jersch', null, '1972-11-19');
insert into Employee (first_name, last_name, email, birthday) values ('Shirlee', 'Alennikov', 'salennikovn@histats.com', '2011-03-04');
insert into Employee (first_name, last_name, email, birthday) values ('Anna-maria', 'Terney', 'aterneyo@mapy.cz', '2008-04-22');
insert into Employee (first_name, last_name, email, birthday) values ('Benni', 'Arnowitz', 'barnowitzp@reference.com', '1968-09-17');
insert into Employee (first_name, last_name, email, birthday) values ('Roseanna', 'Peerless', null, null);
insert into Employee (first_name, last_name, email, birthday) values ('Holly-anne', 'Wainer', 'hwainerr@devhub.com', '1967-04-21');
insert into Employee (first_name, last_name, email, birthday) values ('Cullan', 'Fideler', 'cfidelers@accuweather.com', '1987-06-15');
insert into Employee (first_name, last_name, email, birthday) values ('Chrotoem', 'Maestro', 'cmaestrot@yandex.ru', '1989-04-10');
insert into Employee (first_name, last_name, email, birthday) values ('Muhammad', 'Barbe', null, '2018-01-28');
insert into Employee (first_name, last_name, email, birthday) values ('Desi', 'Doxsey', null, '1975-08-11');
insert into Employee (first_name, last_name, email, birthday) values ('Urbain', 'Counter', 'ucounterw@typepad.com', '2009-03-10');
insert into Employee (first_name, last_name, email, birthday) values ('Audra', 'MacIver', 'amaciverx@imdb.com', null);
insert into Employee (first_name, last_name, email, birthday) values ('Jephthah', 'Greneham', 'jgrenehamy@aboutads.info', '2002-12-24');
insert into Employee (first_name, last_name, email, birthday) values ('Tabatha', 'Pealing', 'tpealingz@free.fr', '2008-12-01');
insert into Employee (first_name, last_name, email, birthday) values ('Essie', 'McDill', null, '2018-10-15');
insert into Employee (first_name, last_name, email, birthday) values ('Sophia', 'Vooght', 'svooght11@taobao.com', '1995-06-02');
insert into Employee (first_name, last_name, email, birthday) values ('Leonore', 'Wallbanks', 'lwallbanks12@stanford.edu', '1972-06-27');
insert into Employee (first_name, last_name, email, birthday) values ('Danyette', 'Fairhead', 'dfairhead13@indiatimes.com', '2004-06-13');
insert into Employee (first_name, last_name, email, birthday) values ('Katrinka', 'Sprott', 'ksprott14@xinhuanet.com', '2010-06-16');
insert into Employee (first_name, last_name, email, birthday) values ('Merle', 'Crinion', 'mcrinion15@barnesandnoble.com', '1960-10-10');
insert into Employee (first_name, last_name, email, birthday) values ('Bartolomeo', 'O''Fearguise', 'bofearguise16@istockphoto.com', '2014-09-29');
insert into Employee (first_name, last_name, email, birthday) values ('Moishe', 'Fishlock', 'mfishlock17@ted.com', '1999-04-21');
insert into Employee (first_name, last_name, email, birthday) values ('Boigie', 'Speir', 'bspeir18@w3.org', '1998-02-06');
insert into Employee (first_name, last_name, email, birthday) values ('Rebeka', 'Atteridge', null, '1989-02-06');
insert into Employee (first_name, last_name, email, birthday) values ('Cherilynn', 'Axtonne', null, '1977-08-03');
insert into Employee (first_name, last_name, email, birthday) values ('Amberly', 'Myring', 'amyring1b@tiny.cc', null);
insert into Employee (first_name, last_name, email, birthday) values ('Kylie', 'Mayoral', 'kmayoral1c@prnewswire.com', '1966-06-07');
insert into Employee (first_name, last_name, email, birthday) values ('Junie', 'De Meis', null, '1968-09-27');
```

3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

   * id'ye göre update işlemi yapalım;

     ```sql
     UPDATE employee
     SET first_name = 'Barbara',
     	last_name = 'Sugarman',
     	email = 'barbara@sugarman.com'
     WHERE id = 2;
     ```

   * isme göre update işlemi yapalım;

     ```sql
     UPDATE employee
     SET first_name = 'Chen',
     	last_name = 'Colde',
     	email = 'chen@colde.com'
     WHERE first_name = 'Kai';
     ```

   * soyisime göre update işlemi yapalım;

     ```sql
     UPDATE employee
     SET last_name = 'Star',
     	email = 'boone1@star.com'
     WHERE last_name = 'Sturt';
     ```

   * email'e göre update işlemi yapalım ;

     ```sql
     UPDATE employee
     SET email = 'audra_maciver@gmail.com',
     	birthday = '1996-09-05'
     WHERE email = 'amaciverx@imdb.com';
     ```

   * doğum yılına göre update işlemi yapalım;

     ```sql
     UPDATE employee
     SET birthday = '1975-05-11'
     WHERE birthday is null;
     ```

4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

   * id'ye göre delete işlemi yapalım;

     ```sql
     DELETE FROM employee
     WHERE id = 3;
     ```

   * isme göre delete işlemi yapalım;

     ```sql
     DELETE FROM employee
     WHERE first_name = 'Barbara';
     ```

   * soya göre delete işlemi yapalım;

     ```sql
     DELETE FROM employee
     WHERE last_name = 'Harler';
     ```

   * email'e göre delete işlemi yapalım; 

     ```sql
     DELETE FROM employee
     WHERE email is null;
     ```

   * doğum yılına göre delete işlemi yapalım; 

     ```sql
     DELETE FROM employee
     WHERE birthday = '1966-06-07';
     ```

     