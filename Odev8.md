* test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
* Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
* Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
* Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

---
```sql
1. CREATE TABLE employee(
	id SERIAL PRIMARY KEY,
	name VARCHAR(50) NOT NULL,
	birthday DATE,
	email VARCHAR(100)
    );
```
```sql
2. 
insert into employee (name, birthday, email) values ('Laurene', '1976-11-04', 'lbrazenor0@arstechnica.com');
insert into employee (name, birthday, email) values ('Caz', '1999-08-29', 'cdyer1@amazonaws.com');
insert into employee (name, birthday, email) values ('Chucho', null, 'cben2@bloglovin.com');
insert into employee (name, birthday, email) values ('Geri', '2019-12-27', 'gartois3@pinterest.com');
insert into employee (name, birthday, email) values ('Roddie', '2006-07-05', null);
insert into employee (name, birthday, email) values ('Paddy', '1977-06-25', 'pbatecok5@dropbox.com');
insert into employee (name, birthday, email) values ('Erny', '1999-12-16', 'esiebert6@seesaa.net');
insert into employee (name, birthday, email) values ('Cahra', '1940-11-18', 'chebborn7@mail.ru');
insert into employee (name, birthday, email) values ('Mateo', '1999-03-17', 'mkillshaw8@seesaa.net');
insert into employee (name, birthday, email) values ('Geri', '1965-11-02', 'gbrownstein9@chicagotribune.com');
insert into employee (name, birthday, email) values ('Jess', null, null);
insert into employee (name, birthday, email) values ('Jennie', '1973-03-10', 'jyorathb@t.co');
insert into employee (name, birthday, email) values ('Bliss', '1985-12-04', 'bpowlandc@alibaba.com');
insert into employee (name, birthday, email) values ('Karena', null, 'kelvinsd@statcounter.com');
insert into employee (name, birthday, email) values ('Kennie', null, 'kfatkine@t.co');
insert into employee (name, birthday, email) values ('Buffy', null, 'breahf@alexa.com');
insert into employee (name, birthday, email) values ('Merwyn', '1934-08-13', 'mwhittetg@google.com.hk');
insert into employee (name, birthday, email) values ('Judith', '1953-09-10', 'jbardwellh@diigo.com');
insert into employee (name, birthday, email) values ('Nyssa', null, 'nturonei@imdb.com');
insert into employee (name, birthday, email) values ('Falito', '1999-03-13', 'fpamplinj@mlb.com');
insert into employee (name, birthday, email) values ('Robbin', '1987-11-02', 'ringersonk@redcross.org');
insert into employee (name, birthday, email) values ('Nichole', '1986-07-12', 'nschildl@newyorker.com');
insert into employee (name, birthday, email) values ('Cissiee', '1999-03-21', null);
insert into employee (name, birthday, email) values ('Bea', '1981-01-19', 'bsaintsburyn@walmart.com');
insert into employee (name, birthday, email) values ('Miller', null, 'mpawlatao@opera.com');
insert into employee (name, birthday, email) values ('Donnie', '1951-08-03', 'ddjorevicp@seesaa.net');
insert into employee (name, birthday, email) values ('Buck', '1949-01-26', 'bmullaneyq@kickstarter.com');
insert into employee (name, birthday, email) values ('Abdel', '1978-02-11', 'azanicchir@pen.io');
insert into employee (name, birthday, email) values ('Craggie', '1999-11-09', 'cclissolds@yolasite.com');
insert into employee (name, birthday, email) values ('Ronna', '1996-05-14', 'rgomersalt@kickstarter.com');
insert into employee (name, birthday, email) values ('Russ', '1931-08-27', 'rharbordu@unblog.fr');
insert into employee (name, birthday, email) values ('Kelcy', '1930-07-27', 'kaudibertv@google.com.au');
insert into employee (name, birthday, email) values ('Nora', null, 'nwilhelmyw@123-reg.co.uk');
insert into employee (name, birthday, email) values ('Sigmund', '1989-07-29', 'sdrewesx@bluehost.com');
insert into employee (name, birthday, email) values ('Issiah', '1931-08-25', 'iweinsy@miitbeian.gov.cn');
insert into employee (name, birthday, email) values ('Lincoln', '1949-03-29', 'lhedonz@mozilla.org');
insert into employee (name, birthday, email) values ('Ernesta', '1932-10-23', null);
insert into employee (name, birthday, email) values ('Lettie', '1981-09-08', null);
insert into employee (name, birthday, email) values ('Nonna', '1929-01-14', 'nconklin12@unesco.org');
insert into employee (name, birthday, email) values ('Catlee', '1975-09-23', null);
insert into employee (name, birthday, email) values ('Clarisse', '2016-06-24', 'cclendinning14@surveymonkey.com');
insert into employee (name, birthday, email) values ('Gannon', '1981-04-29', 'galliband15@ifeng.com');
insert into employee (name, birthday, email) values ('Jeannette', null, 'jfrostdicke16@amazonaws.com');
insert into employee (name, birthday, email) values ('Clayborn', '1982-08-13', null);
insert into employee (name, birthday, email) values ('Benedict', null, 'bchung18@ihg.com');
insert into employee (name, birthday, email) values ('Davin', '2022-01-11', null);
insert into employee (name, birthday, email) values ('Aloin', '1995-01-31', 'alardiner1a@go.com');
insert into employee (name, birthday, email) values ('Henryetta', '2009-09-15', 'hblodget1b@wikimedia.org');
insert into employee (name, birthday, email) values ('Ursa', '1962-11-06', null);
insert into employee (name, birthday, email) values ('Gerta', '2013-03-19', 'gbowditch1d@theatlantic.com');
insert into employee (name, birthday, email) values ('Velvet', '1926-10-25', 'vlenham1e@people.com.cn');
insert into employee (name, birthday, email) values ('Krysta', null, 'kriply1f@java.com');
insert into employee (name, birthday, email) values ('Brandy', null, 'bsnooks1g@blog.com');
insert into employee (name, birthday, email) values ('Raye', '1965-02-24', 'rsaxton1h@mlb.com');
insert into employee (name, birthday, email) values ('Margaret', '2007-09-29', 'mnarrie1i@studiopress.com');
insert into employee (name, birthday, email) values ('Vyky', '1985-08-19', 'vtawton1j@goodreads.com');
insert into employee (name, birthday, email) values ('Kaye', null, 'kdummett1k@xinhuanet.com');
insert into employee (name, birthday, email) values ('Kizzee', null, 'kwhymark1l@reference.com');
insert into employee (name, birthday, email) values ('Erik', '1932-11-11', null);
insert into employee (name, birthday, email) values ('Carin', '1955-12-19', null);
insert into employee (name, birthday, email) values ('Lilian', null, 'ldebrick1o@1688.com');
insert into employee (name, birthday, email) values ('Georgeanna', null, 'gkubala1p@over-blog.com');
insert into employee (name, birthday, email) values ('Dennie', '2002-02-08', 'ddrohane1q@altervista.org');
insert into employee (name, birthday, email) values ('Claudian', '2006-07-06', 'cbrainsby1r@instagram.com');
insert into employee (name, birthday, email) values ('Gradeigh', '1950-02-16', 'gcammiemile1s@google.es');
insert into employee (name, birthday, email) values ('Milton', '1946-08-30', 'msuddaby1t@pcworld.com');
insert into employee (name, birthday, email) values ('Hestia', '1968-10-03', 'hklammt1u@unicef.org');
insert into employee (name, birthday, email) values ('Cedric', '1967-08-22', 'cchelam1v@google.ru');
insert into employee (name, birthday, email) values ('Hasty', null, 'hcallaway1w@globo.com');
insert into employee (name, birthday, email) values ('Sylvan', '2014-04-04', 'sslocom1x@mapquest.com');
insert into employee (name, birthday, email) values ('Ilse', '2023-03-10', 'ibelsher1y@mashable.com');
insert into employee (name, birthday, email) values ('Jarret', '1988-04-10', 'jlatey1z@webeden.co.uk');
insert into employee (name, birthday, email) values ('Cy', null, 'cwasselin20@redcross.org');
insert into employee (name, birthday, email) values ('Miguela', '1969-01-29', 'mpretorius21@networksolutions.com');
insert into employee (name, birthday, email) values ('Yolande', '1998-05-31', 'yhudleston22@ibm.com');
insert into employee (name, birthday, email) values ('Anthia', '1936-02-13', 'adensun23@networkadvertising.org');
insert into employee (name, birthday, email) values ('Elston', '1997-10-18', 'ebyham24@cdbaby.com');
insert into employee (name, birthday, email) values ('Debbie', '1968-01-24', 'delcy25@msn.com');
insert into employee (name, birthday, email) values ('Orel', null, 'omarconi26@indiatimes.com');
insert into employee (name, birthday, email) values ('Lynde', null, null);
insert into employee (name, birthday, email) values ('Tamma', '2000-08-27', 'tfishbie28@shareasale.com');
insert into employee (name, birthday, email) values ('Konstanze', null, 'kabramovic29@aol.com');
insert into employee (name, birthday, email) values ('Hildagard', '1941-08-07', 'hhobden2a@opensource.org');
insert into employee (name, birthday, email) values ('Stern', '1961-01-20', 'sroderham2b@constantcontact.com');
insert into employee (name, birthday, email) values ('Norbie', null, 'nfrowing2c@springer.com');
insert into employee (name, birthday, email) values ('Edmund', '1971-08-03', 'echapling2d@friendfeed.com');
insert into employee (name, birthday, email) values ('Tanner', '1945-10-09', null);
insert into employee (name, birthday, email) values ('Tabby', '2008-05-29', 'tsothcott2f@jigsy.com');
insert into employee (name, birthday, email) values ('Kelley', '1935-03-02', 'kduddan2g@wunderground.com');
insert into employee (name, birthday, email) values ('Andrej', '1986-08-20', 'abernat2h@virginia.edu');
insert into employee (name, birthday, email) values ('Edgard', null, 'epilbury2i@wordpress.com');
insert into employee (name, birthday, email) values ('Quinn', '1924-10-03', 'qcantrell2j@plala.or.jp');
insert into employee (name, birthday, email) values ('Matthieu', null, null);
insert into employee (name, birthday, email) values ('Yorke', '1946-10-31', 'ynorkutt2l@jugem.jp');
insert into employee (name, birthday, email) values ('Abram', '1990-01-31', 'agurner2m@shutterfly.com');
insert into employee (name, birthday, email) values ('Elonore', '2007-11-04', 'eeakle2n@ehow.com');
insert into employee (name, birthday, email) values ('Gun', '1937-04-09', 'gjanssens2o@paypal.com');
insert into employee (name, birthday, email) values ('Heindrick', null, 'hyeldon2p@ebay.com');
insert into employee (name, birthday, email) values ('Janeen', null, 'jelham2q@ibm.com');
insert into employee (name, birthday, email) values ('Anallise', '1931-11-20', 'agrimsley2r@reference.com');
```
```sql 
1. UPDATE employee
   SET birthday = '1996-01-24'
   WHERE id = 3;
2. UPDATE employee
   SET email = 'erik@gmail.com'
   WHERE id = 56;
3. UPDATE employee
   SET birthday = '2002-02-12' , email = 'default@gmail.com'
   WHERE name ILIKE 'm%u';
4. UPDATE employee
   SET email = 'jess@gmail.com'
   WHERE name ILIKE 'J__s';
5. UPDATE employee
   SET email = 'default@gmail.com'
   WHERE email Is NULL ;
```
```sql
1. DELETE FROM employee
   WHERE birthday Is NULL ;
2. DELETE FROM employee
   WHERE name LIKE 'L%n';
3. DELETE FROM employee
   WHERE email = 'default@gmail.com';
4. DELETE FROM employee
   WHERE id > 40;
5. DELETE FROM employee
   WHERE name ILIKE 'a%';
```