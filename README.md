# Arslan's Data Analyst Portfolio

### Introduction
I'm Arslan Saeed, a data enthusiast with a background in Electronics. I have been managing an institute and teaching IT, Mathematics, and Science since 2017. Proficient in SQL, Excel, and Power BI, I am now expanding my skills in Python. With solid knowledge of data cleaning, modeling, visualization, and creating insightful dashboards, I am a quick learner 
and thrive on learning from organization's professionals. My future goal is to leverage data analysis to drive informed decision-making and contribute positively to diverse domains. I am eager to join your firm, where I can apply my expertise in 
data analysis, collaborate with a dynamic team, and continue growing professionally. Let's connect and explore data together!

### SQL Database Management and Table Creation ✨.

```sql
"Creating Department Table"
---------------------------
create table departments (
department varchar(100),
division varchar(100),
primary key (department)
);


---------------------Database Management----------------
CREATE DATABASE traning

DROP DATABASE traning;

BACKUP DATABASE traning
TO DISK= C:\Course\traning.bak;
--OR--
WITH DIFFERENTIAL;

TRUNCATE TABLE test;

DROP TABLE test;

ALTER TABLE test
add COLUMN datatype;

ALTER TABLE test
DROP COLUMN activity;

ALTER TABLE test
RENAME COLUMN ID to emp_ID;
-------------------------------------------------------

"Creating Region Table"
-----------------------
create table regions (
region_id int,
region varchar(20),
country varchar(20),
primary key (region_id)
);

insert into regions values (1, 'Southwest', 'United States');
insert into regions values (2, 'Northeast', 'United States');
insert into regions values (3, 'Northwest', 'United States');
insert into regions values (4, 'Central', 'Asia');
insert into regions values (5, 'East Asia', 'Asia');
insert into regions values (6, 'Quebec', 'Canada');
insert into regions values (7, 'Nova Scotia', 'Canada');

"Creating Employees Table"
--------------------------
create table employees (
employee_id INT,
first_name VARCHAR(50),
last_name VARCHAR(50),
email VARCHAR(50),
hire_date DATE,
department VARCHAR(17),
gender VARCHAR(1),
salary INT,
region_id INT,
primary key (employee_id)
);

insert into employees values (1, 'Berrie', 'Manueau', 'bmanueau0@dion.ne.jp', '2006-04-20', 'Sports', 'F', 154864, 4);
insert into employees values (2, 'Aeriell', 'McNee', 'amcnee1@google.es', '2009-01-26', 'Tools', 'F', 56752, 3);
insert into employees values (3, 'Sydney', 'Symonds', 'ssymonds2@hhs.gov', '2010-05-17', 'Clothing', 'F', 95313, 4);
insert into employees values (4, 'Avrom', 'Rowantree', null, '2014-08-02', 'Phones & Tablets', 'M', 119674, 7);
insert into employees values (5, 'Feliks', 'Morffew', 'fmorffew4@a8.net', '2003-01-14', 'Computers', 'M', 55307, 5);
insert into employees values (6, 'Bethena', 'Trow', 'btrow5@technorati.com', '2003-06-08', 'Sports', 'F', 134501, 3);
insert into employees values (7, 'Ardeen', 'Curwood', 'acurwood6@1und1.de', '2006-02-19', 'Clothing', 'F', 28995, 7);
insert into employees values (8, 'Seline', 'Dubber', 'sdubber7@t-online.de', '2012-05-28', 'Phones & Tablets', 'F', 101066, 3);
insert into employees values (9, 'Dayle', 'Trail', 'dtrail8@tamu.edu', '2003-03-01', 'First Aid', 'F', 82753, 1);
insert into employees values (10, 'Redford', 'Roberti', null, '2008-07-21', 'Clothing', 'M', 72225, 7);
insert into employees values (11, 'Nickey', 'Pointon', 'npointona@vistaprint.com', '2006-12-30', 'Jewelry', 'M', 126333, 7);
insert into employees values (12, 'Leonora', 'Casaroli', 'lcasarolib@plala.or.jp', '2013-07-22', 'Beauty', 'F', 99504, 3);
insert into employees values (13, 'Anetta', 'Arnao', null, '2009-05-23', 'Games', 'F', 38162, 1);
insert into employees values (14, 'Jodi', 'Hook', 'jhookd@booking.com', '2003-10-16', 'Tools', 'F', 126588, 2);
insert into employees values (15, 'Alyson', 'Franzonello', null, '2004-01-01', 'Furniture', 'F', 61256, 6);
insert into employees values (16, 'Merell', 'Yakovliv', 'myakovlivf@ucsd.edu', '2008-08-16', 'Movies', 'M', 78141, 7);
insert into employees values (17, 'Annora', 'Bendelow', 'abendelowg@google.com.hk', '2009-06-12', 'Toys', 'F', 75283, 5);
insert into employees values (18, 'Ronica', 'Armfield', null, '2012-09-14', 'Toys', 'F', 114983, 5);
insert into employees values (19, 'Bernardine', 'Hendricks', 'bhendricksi@privacy.gov.au', '2006-02-04', 'Device Repair', 'F', 158268, 3);
insert into employees values (20, 'Jessey', 'Colum', 'jcolumj@pen.io', '2013-07-08', 'Computers', 'M', 77173, 7);
insert into employees values (21, 'Bernardo', 'Davage', null, '2013-07-11', 'Clothing', 'M', 124949, 6);
insert into employees values (22, 'Cayla', 'Duffer', null, '2007-02-01', 'Grocery', 'F', 78589, 3);
insert into employees values (23, 'Vanda', 'Marwick', 'vmarwickm@upenn.edu', '2014-02-06', 'Automotive', 'F', 103570, 4);
insert into employees values (24, 'Corabel', 'Syversen', 'csyversenn@aboutads.info', '2016-03-03', 'Pharmacy', 'F', 91323, 3);
insert into employees values (25, 'Zane', 'Breem', 'zbreemo@abc.net.au', '2012-07-30', 'Cosmetics', 'M', 56688, 6);
insert into employees values (26, 'Frasquito', 'Cawson', null, '2006-06-24', 'Movies', 'M', 78881, 1);
insert into employees values (27, 'Niles', 'Chawkley', 'nchawkleyq@flavors.me', '2013-09-22', 'Movies', 'M', 156303, 3);
insert into employees values (28, 'Emanuele', 'Sandcraft', 'esandcraftr@toplist.cz', '2015-01-01', 'Garden', 'M', 70827, 2);
insert into employees values (29, 'Cortie', 'Ambrosini', 'cambrosinis@microsoft.com', '2014-05-03', 'Games', 'M', 133847, 4);
insert into employees values (30, 'Benn', 'Dudley', 'bdudleyt@dailymail.co.uk', '2012-08-24', 'Beauty', 'M', 67800, 7);
insert into employees values (31, 'Cleve', 'Conti', 'ccontiu@noaa.gov', '2008-02-27', 'Garden', 'M', 91608, 5);
insert into employees values (32, 'Aldon', 'Paddison', 'apaddisonv@lulu.com', '2013-06-30', 'First Aid', 'M', 109592, 5);
insert into employees values (33, 'Ernestine', 'Sloley', 'esloleyw@rakuten.co.jp', '2011-06-27', 'Device Repair', 'F', 146549, 5);
insert into employees values (34, 'Lucy', 'Olifaunt', 'lolifauntx@dailymotion.com', '2005-02-07', 'Sports', 'F', 165660, 7);
insert into employees values (35, 'Olenolin', 'Blundan', null, '2004-09-29', 'Beauty', 'M', 137691, 3);
insert into employees values (36, 'Anatollo', 'Doyle', null, '2016-04-08', 'Computers', 'M', 98207, 1);
insert into employees values (37, 'Wilfrid', 'Sainer', 'wsainer10@gizmodo.com', '2015-09-30', 'Movies', 'M', 147235, 3);
insert into employees values (38, 'Edna', 'Erwin', null, '2003-04-09', 'Children Clothing', 'F', 91397, 5);
insert into employees values (39, 'Mikael', 'Kybbye', 'mkybbye12@si.edu', '2010-12-07', 'Vitamins', 'M', 52642, 1);
insert into employees values (40, 'Modestine', 'Proctor', 'mproctor13@digg.com', '2015-05-04', 'Tools', 'F', 81889, 7);
insert into employees values (41, 'Jania', 'Gresly', 'jgresly14@ted.com', '2010-09-08', 'Furniture', 'F', 97812, 6);
insert into employees values (42, 'Penelopa', 'Danieli', 'pdanieli15@microsoft.com', '2014-06-23', 'Toys', 'F', 85218, 1);
insert into employees values (43, 'Maurise', 'Bengefield', 'mbengefield16@sohu.com', '2005-07-08', 'Pharmacy', 'F', 63332, 2);
insert into employees values (44, 'Moise', 'Turpey', 'mturpey17@mac.com', '2008-04-15', 'Device Repair', 'M', 33781, 1);
insert into employees values (45, 'Giacopo', 'Mariner', 'gmariner18@noaa.gov', '2005-01-31', 'Grocery', 'M', 130445, 7);
insert into employees values (46, 'Lanny', 'Comolli', 'lcomolli19@posterous.com', '2014-06-19', 'Phones & Tablets', 'F', 34250, 6);
insert into employees values (47, 'Byrann', 'Jaukovic', 'bjaukovic1a@networkadvertising.org', '2011-11-13', 'Books', 'M', 121054, 7);
insert into employees values (48, 'Birgitta', 'Stanbrooke', 'bstanbrooke1b@netvibes.com', '2016-09-12', 'Clothing', 'F', 77259, 1);
insert into employees values (49, 'Portie', 'Ilden', 'pilden1c@usa.gov', '2006-01-20', 'Device Repair', 'M', 69190, 7);
insert into employees values (50, 'Modesty', 'Blagburn', 'mblagburn1d@studiopress.com', '2008-03-16', 'Beauty', 'F', 130580, 1);
insert into employees values (51, 'Norine', 'Steinham', null, '2008-08-22', 'Sports', 'F', 66488, 2);
insert into employees values (52, 'Charla', 'Adamowicz', 'cadamowicz1f@tiny.cc', '2011-03-16', 'Music', 'F', 162206, 2);
insert into employees values (53, 'Alphonse', 'Shedd', 'ashedd1g@illinois.edu', '2014-08-17', 'Cosmetics', 'M', 33272, 4);
insert into employees values (54, 'Verney', 'McQuirk', 'vmcquirk1h@ning.com', '2012-06-17', 'Clothing', 'M', 97156, 2);
insert into employees values (55, 'Norina', 'Yea', 'nyea1i@cnet.com', '2005-06-14', 'Children Clothing', 'F', 45959, 1);
insert into employees values (56, 'Wilek', 'Cossor', 'wcossor1j@merriam-webster.com', '2014-09-17', 'Children Clothing', 'M', 91859, 4);
insert into employees values (57, 'Reuben', 'Hallard', null, '2009-03-14', 'First Aid', 'M', 34572, 5);
insert into employees values (58, 'King', 'Sangra', null, '2012-01-08', 'Grocery', 'M', 53499, 6);
insert into employees values (59, 'Hilario', 'Reily', 'hreily1m@google.co.jp', '2012-03-18', 'Phones & Tablets', 'M', 83332, 5);
insert into employees values (60, 'Orland', 'Backhouse', 'obackhouse1n@yahoo.co.jp', '2007-07-12', 'Beauty', 'M', 162845, 6);
insert into employees values (61, 'Bobby', 'Keppie', null, '2010-10-22', 'Computers', 'M', 123722, 3);
insert into employees values (62, 'Lek', 'Camplin', null, '2007-07-16', 'Children Clothing', 'M', 124190, 6);
insert into employees values (63, 'Fanya', 'Naish', 'fnaish1q@jalbum.net', '2014-02-24', 'Tools', 'F', 140681, 3);
insert into employees values (64, 'Ody', 'Dunks', 'odunks1r@theguardian.com', '2006-10-13', 'Toys', 'M', 92003, 1);
insert into employees values (65, 'Cindi', 'Clyburn', 'cclyburn1s@wikimedia.org', '2007-07-07', 'Games', 'F', 70527, 2);
insert into employees values (66, 'Deb', 'Scarratt', null, '2010-12-24', 'Jewelry', 'F', 112297, 3);
insert into employees values (67, 'Wain', 'Betonia', 'wbetonia1u@princeton.edu', '2005-07-23', 'Tools', 'M', 26578, 3);
insert into employees values (68, 'Wilhelmina', 'Martignon', null, '2013-04-11', 'Jewelry', 'F', 150818, 3);
insert into employees values (69, 'Ivar', 'Burwin', 'iburwin1w@hostgator.com', '2008-07-04', 'Toys', 'M', 67447, 4);
insert into employees values (70, 'Geoff', 'Burrell', 'gburrell1x@paginegialle.it', '2016-05-10', 'Clothing', 'M', 88652, 1);
insert into employees values (71, 'Tobi', 'Lamasna', 'tlamasna1y@gmpg.org', '2012-04-10', 'Vitamins', 'F', 68925, 4);
insert into employees values (72, 'Zebulon', 'Guppey', 'zguppey1z@virginia.edu', '2004-11-30', 'Toys', 'M', 89221, 7);
insert into employees values (73, 'Melonie', 'Tredger', 'mtredger20@pcworld.com', '2006-03-26', 'Computers', 'F', 63128, 3);
insert into employees values (74, 'Margy', 'Bess', 'mbess21@google.fr', '2012-11-10', 'Computers', 'F', 144141, 7);
insert into employees values (75, 'Fiorenze', 'Woodyer', null, '2003-02-17', 'Phones & Tablets', 'F', 51266, 2);
insert into employees values (76, 'Toby', 'Deek', 'tdeek23@wikimedia.org', '2015-07-10', 'Device Repair', 'F', 111363, 2);
insert into employees values (77, 'Maurice', 'Philbrick', null, '2006-01-08', 'Sports', 'M', 67615, 1);
insert into employees values (78, 'Wendel', 'Olczyk', 'wolczyk25@redcross.org', '2010-01-11', 'Games', 'M', 118392, 4);
insert into employees values (79, 'Rora', 'Brumfitt', 'rbrumfitt26@ucoz.ru', '2003-01-12', 'Children Clothing', 'F', 153489, 7);
insert into employees values (80, 'Hester', 'Seakin', 'hseakin27@netlog.com', '2006-11-30', 'Clothing', 'F', 150887, 5);
insert into employees values (81, 'Ivan', 'Hassewell', 'ihassewell28@paginegialle.it', '2004-09-26', 'Device Repair', 'M', 74721, 6);
insert into employees values (82, 'Dani', 'Diter', 'dditer29@huffingtonpost.com', '2006-01-13', 'Camping', 'M', 102516, 2);
insert into employees values (83, 'Elnora', 'Babin', 'ebabin2a@foxnews.com', '2003-02-22', 'First Aid', 'F', 34355, 5);
insert into employees values (84, 'Kippie', 'Petrolli', 'kpetrolli2b@wsj.com', '2008-06-27', 'Clothing', 'M', 128327, 2);
insert into employees values (85, 'Christal', 'Ghest', null, '2006-10-21', 'Pharmacy', 'F', 64957, 5);
insert into employees values (86, 'Doll', 'Blondel', 'dblondel2d@list-manage.com', '2007-03-30', 'Camping', 'F', 136773, 7);
insert into employees values (87, 'Riane', 'Malloch', 'rmalloch2e@reuters.com', '2014-12-17', 'Tools', 'F', 101577, 3);
insert into employees values (88, 'Brandice', 'Tomovic', 'btomovic2f@histats.com', '2008-06-21', 'Music', 'F', 130031, 2);
insert into employees values (89, 'Claudetta', 'Sappson', 'csappson2g@aboutads.info', '2011-08-24', 'Sports', 'F', 157802, 5);
insert into employees values (90, 'Irita', 'Starie', 'istarie2h@answers.com', '2004-10-15', 'Automotive', 'F', 160783, 1);
insert into employees values (91, 'Riley', 'Yellowlea', 'ryellowlea2i@ibm.com', '2007-03-20', 'Camping', 'M', 166569, 5);
insert into employees values (92, 'Port', 'Dancy', 'pdancy2j@nytimes.com', '2011-06-14', 'Clothing', 'M', 86352, 3);
insert into employees values (93, 'Hallsy', 'Theuss', 'htheuss2k@independent.co.uk', '2010-04-05', 'Computers', 'M', 49565, 3);
insert into employees values (94, 'Cati', 'Keat', 'ckeat2l@nih.gov', '2004-07-17', 'Tools', 'F', 103302, 7);
insert into employees values (95, 'Stevana', 'Norton', 'snorton2m@dion.ne.jp', '2014-02-21', 'Pharmacy', 'F', 111122, 4);
insert into employees values (96, 'Cal', 'Lowre', 'clowre2n@marketwatch.com', '2010-12-30', 'Movies', 'F', 47412, 2);
insert into employees values (97, 'Jilleen', 'Toone', null, '2013-04-20', 'Automotive', 'F', 137393, 3);
insert into employees values (98, 'Natalee', 'Arnal', 'narnal2p@reference.com', '2014-03-16', 'Tools', 'F', 125024, 5);
insert into employees values (99, 'Simeon', 'Scarsbrooke', 'sscarsbrooke2q@ted.com', '2011-04-10', 'Jewelry', 'M', 56976, 2);
insert into employees values (100, 'Sashenka', 'Paris', 'sparis2r@si.edu', '2005-10-01', 'Furniture', 'F', 117137, 2);
insert into employees values (101, 'Ev', 'Wessell', 'ewessell2s@earthlink.net', '2013-06-28', 'Grocery', 'M', 164582, 4);
insert into employees values (102, 'Bryna', 'Tarply', 'btarply2t@scientificamerican.com', '2010-08-20', 'Movies', 'F', 71440, 7);
insert into employees values (103, 'Gregoire', 'Clementi', 'gclementi2u@privacy.gov.au', '2003-11-04', 'Garden', 'M', 104006, 1);
insert into employees values (104, 'Dulsea', 'Drennan', null, '2014-12-06', 'Computers', 'F', 128255, 7);
insert into employees values (105, 'Butch', 'Calbert', 'bcalbert2w@cbc.ca', '2014-09-04', 'Books', 'M', 70287, 4);
insert into employees values (106, 'Heath', 'MacRedmond', null, '2004-10-22', 'Phones & Tablets', 'M', 156926, 2);
insert into employees values (107, 'Christine', 'Hessing', 'chessing2y@dailymail.co.uk', '2013-11-07', 'Books', 'F', 149864, 5);
insert into employees values (108, 'Dionysus', 'Dumpleton', 'ddumpleton2z@typepad.com', '2009-12-30', 'Movies', 'M', 145973, 5);
insert into employees values (109, 'Sigismund', 'Von Hindenburg', 'svonhindenburg30@seattletimes.com', '2007-01-28', 'Toys', 'M', 125291, 1);
insert into employees values (110, 'Roarke', 'Sully', 'rsully31@army.mil', '2004-10-26', 'Movies', 'M', 86223, 7);
insert into employees values (111, 'Elihu', 'Epp', null, '2012-11-11', 'Pharmacy', 'M', 55779, 6);
insert into employees values (112, 'Holt', 'Sillars', 'hsillars33@illinois.edu', '2012-10-23', 'Books', 'M', 46099, 1);
insert into employees values (113, 'Myrtice', 'Emmens', null, '2011-11-21', 'Movies', 'F', 36919, 6);
insert into employees values (114, 'Johnnie', 'Waight', 'jwaight35@yahoo.com', '2007-11-28', 'Beauty', 'M', 120362, 6);
insert into employees values (115, 'Peyter', 'Jansey', 'pjansey36@linkedin.com', '2005-12-02', 'Children Clothing', 'M', 23348, 4);
insert into employees values (116, 'Kath', 'Mateescu', 'kmateescu37@google.ca', '2016-02-18', 'Device Repair', 'F', 133361, 6);
insert into employees values (117, 'Cornelle', 'Marty', 'cmarty38@newsvine.com', '2015-11-07', 'Books', 'F', 156858, 4);
insert into employees values (118, 'Roxane', 'Raftery', 'rraftery39@arstechnica.com', '2016-08-05', 'Movies', 'F', 43199, 1);
insert into employees values (119, 'Worth', 'Pavey', null, '2007-04-09', 'Tools', 'M', 86252, 5);
insert into employees values (120, 'Elwin', 'Seakin', 'eseakin3b@tmall.com', '2014-07-09', 'First Aid', 'M', 141261, 1);
insert into employees values (121, 'Collie', 'Morfett', null, '2016-06-17', 'Clothing', 'F', 89961, 4);
insert into employees values (122, 'Josselyn', 'Cardus', 'jcardus3d@technorati.com', '2010-01-19', 'Music', 'F', 162341, 7);
insert into employees values (123, 'Olvan', 'Ladds', null, '2004-04-01', 'Books', 'M', 61102, 3);
insert into employees values (124, 'Remy', 'Sperski', 'rsperski3f@vistaprint.com', '2004-06-19', 'Grocery', 'F', 22796, 1);
insert into employees values (125, 'Valera', 'Southway', 'vsouthway3g@timesonline.co.uk', '2010-05-20', 'Device Repair', 'F', 25114, 6);
insert into employees values (126, 'Roslyn', 'Guiu', 'rguiu3h@com.com', '2003-08-11', 'Automotive', 'F', 157260, 1);
insert into employees values (127, 'Colby', 'Soulsby', 'csoulsby3i@google.co.jp', '2011-06-22', 'Toys', 'M', 104665, 5);
insert into employees values (128, 'Archibald', 'Pavey', null, '2015-04-27', 'Toys', 'M', 59860, 1);
insert into employees values (129, 'Roslyn', 'Frape', 'rfrape3k@chronoengine.com', '2004-04-07', 'Garden', 'F', 91287, 6);
insert into employees values (130, 'Vincents', 'Gullivent', 'vgullivent3l@wikia.com', '2010-07-24', 'Camping', 'M', 57696, 6);
insert into employees values (131, 'Hewet', 'Calafate', 'hcalafate3m@webmd.com', '2016-11-24', 'Phones & Tablets', 'M', 113979, 2);
insert into employees values (132, 'Olivie', 'Issett', 'oissett3n@purevolume.com', '2004-05-31', 'Movies', 'F', 155316, 4);
insert into employees values (133, 'Ezri', 'Foystone', 'efoystone3o@dagondesign.com', '2010-10-26', 'Garden', 'M', 87986, 5);
insert into employees values (134, 'Demott', 'Mouton', null, '2007-09-26', 'Cosmetics', 'M', 22284, 5);
insert into employees values (135, 'Salli', 'Caville', 'scaville3q@miibeian.gov.cn', '2008-10-17', 'Furniture', 'F', 29124, 5);
insert into employees values (136, 'Cordie', 'Broadbear', 'cbroadbear3r@eventbrite.com', '2015-03-02', 'Games', 'M', 124521, 2);
insert into employees values (137, 'Darn', 'Pattisson', 'dpattisson3s@latimes.com', '2013-01-23', 'Decor', 'M', 152418, 7);
insert into employees values (138, 'Clemmie', 'Forber', 'cforber3t@fc2.com', '2014-10-17', 'Garden', 'F', 53101, 6);
insert into employees values (139, 'Kalie', 'Dowthwaite', 'kdowthwaite3u@technorati.com', '2003-11-24', 'First Aid', 'F', 132796, 3);
insert into employees values (140, 'Eugenia', 'Scourgie', 'escourgie3v@imdb.com', '2011-06-29', 'Camping', 'F', 26747, 5);
insert into employees values (141, 'Rozamond', 'Malam', 'rmalam3w@indiatimes.com', '2011-10-10', 'Phones & Tablets', 'F', 140349, 3);
insert into employees values (142, 'Constantine', 'Torrese', 'ctorrese3x@bloglines.com', '2004-09-11', 'Device Repair', 'F', 112819, 3);
insert into employees values (143, 'Dasi', 'Kennefick', 'dkennefick3y@apple.com', '2006-04-30', 'Device Repair', 'F', 29158, 4);
insert into employees values (144, 'Orelia', 'McBoyle', 'omcboyle3z@reddit.com', '2005-11-22', 'Children Clothing', 'F', 78053, 6);
insert into employees values (145, 'Elene', 'Ofen', 'eofen40@e-recht24.de', '2015-09-11', 'Tools', 'F', 43510, 2);
insert into employees values (146, 'Stanfield', 'Bagnall', null, '2015-06-01', 'Clothing', 'M', 92839, 6);
insert into employees values (147, 'Coralie', 'Shea', 'cshea42@php.net', '2004-08-17', 'Children Clothing', 'F', 128326, 2);
insert into employees values (148, 'Jobina', 'Oldacre', 'joldacre43@de.vu', '2007-07-03', 'Beauty', 'F', 119587, 6);
insert into employees values (149, 'Brooks', 'Dinsdale', 'bdinsdale44@kickstarter.com', '2010-01-03', 'Cosmetics', 'F', 119774, 7);
insert into employees values (150, 'Rex', 'Cowlishaw', 'rcowlishaw45@webnode.com', '2008-02-08', 'Games', 'M', 124936, 4);
insert into employees values (151, 'Maximilianus', 'Woonton', 'mwoonton46@ning.com', '2008-12-18', 'Toys', 'M', 90399, 5);
insert into employees values (152, 'Johnette', 'Claworth', 'jclaworth47@google.pl', '2009-12-13', 'Games', 'F', 27750, 3);
insert into employees values (153, 'Damiano', 'Speirs', 'dspeirs48@google.co.jp', '2012-10-02', 'Books', 'M', 94781, 3);
insert into employees values (154, 'Sapphira', 'Stouther', 'sstouther49@photobucket.com', '2007-12-10', 'Device Repair', 'F', 39966, 3);
insert into employees values (155, 'Fleming', 'Gulleford', 'fgulleford4a@nasa.gov', '2004-10-31', 'Games', 'M', 66813, 4);
insert into employees values (156, 'Joleen', 'Rothwell', 'jrothwell4b@fastcompany.com', '2004-10-24', 'Sports', 'F', 29838, 2);
insert into employees values (157, 'Paulie', 'Wadly', 'pwadly4c@nytimes.com', '2015-04-09', 'Pharmacy', 'M', 37829, 5);
insert into employees values (158, 'Tally', 'Bearcroft', 'tbearcroft4d@soup.io', '2004-02-09', 'Device Repair', 'M', 98291, 4);
insert into employees values (159, 'Lindon', 'Anniwell', 'lanniwell4e@ustream.tv', '2011-06-11', 'Games', 'M', 98335, 4);
insert into employees values (160, 'Stella', 'Kershow', 'skershow4f@patch.com', '2012-05-30', 'Device Repair', 'F', 160249, 2);
insert into employees values (161, 'Kathye', 'Kinnett', 'kkinnett4g@cloudflare.com', '2005-10-09', 'Beauty', 'F', 71413, 6);
insert into employees values (162, 'Wynne', 'Fourcade', 'wfourcade4h@uiuc.edu', '2009-12-05', 'Device Repair', 'F', 161532, 5);
insert into employees values (163, 'Stirling', 'MacSweeney', 'smacsweeney4i@sourceforge.net', '2008-11-10', 'Jewelry', 'M', 37157, 5);
insert into employees values (164, 'Benjamin', 'Younie', 'byounie4j@cdbaby.com', '2006-11-13', 'Sports', 'M', 21735, 2);
insert into employees values (165, 'Hillary', 'Coward', null, '2015-07-10', 'Furniture', 'F', 70680, 7);
insert into employees values (166, 'Jacqui', 'Buttwell', null, '2003-07-05', 'Movies', 'F', 45570, 6);
insert into employees values (167, 'Karlis', 'Cromar', 'kcromar4m@accuweather.com', '2011-07-20', 'Clothing', 'M', 113213, 1);
insert into employees values (168, 'Jarad', 'Plenderleith', 'jplenderleith4n@imageshack.us', '2012-05-26', 'Children Clothing', 'M', 31276, 4);
insert into employees values (169, 'Talyah', 'Delgadillo', 'tdelgadillo4o@cnn.com', '2010-07-19', 'Furniture', 'F', 77245, 2);
insert into employees values (170, 'Linnell', 'Haps', 'lhaps4p@blogs.com', '2016-09-25', 'Computers', 'F', 98885, 7);
insert into employees values (171, 'Lurette', 'Holbie', 'lholbie4q@qq.com', '2008-08-16', 'Device Repair', 'F', 142660, 7);
insert into employees values (172, 'Bunny', 'Sawkin', 'bsawkin4r@behance.net', '2013-10-21', 'Garden', 'F', 163361, 1);
insert into employees values (173, 'Bev', 'Kincaid', null, '2008-12-06', 'Clothing', 'M', 65336, 7);
insert into employees values (174, 'Artair', 'Tumbelty', null, '2007-12-01', 'Movies', 'M', 142589, 5);
insert into employees values (175, 'Lockwood', 'Grave', null, '2007-05-14', 'Cosmetics', 'M', 129004, 6);
insert into employees values (176, 'Billie', 'Trebbett', null, '2007-10-04', 'Furniture', 'M', 123320, 7);
insert into employees values (177, 'Michail', 'Huggard', 'mhuggard4w@php.net', '2005-01-07', 'Device Repair', 'M', 164355, 3);
insert into employees values (178, 'Cordelie', 'Giffkins', 'cgiffkins4x@loc.gov', '2012-11-21', 'Music', 'F', 24799, 2);
insert into employees values (179, 'Lanny', 'Northcott', 'lnorthcott4y@nyu.edu', '2016-07-26', 'First Aid', 'M', 159320, 6);
insert into employees values (180, 'Damara', 'Scherer', 'dscherer4z@dion.ne.jp', '2005-01-04', 'Tools', 'F', 44978, 2);
insert into employees values (181, 'Jayme', 'Jimmison', 'jjimmison50@amazon.co.uk', '2009-07-18', 'Camping', 'M', 79893, 1);
insert into employees values (182, 'Jaimie', 'Paulusch', 'jpaulusch51@sakura.ne.jp', '2004-10-10', 'Jewelry', 'F', 36979, 5);
insert into employees values (183, 'Maurita', 'Slegg', 'mslegg52@ning.com', '2007-09-25', 'Beauty', 'F', 59338, 1);
insert into employees values (184, 'Bertie', 'Androletti', 'bandroletti53@salon.com', '2013-02-02', 'Music', 'M', 109859, 3);
insert into employees values (185, 'Nels', 'Helder', 'nhelder54@gnu.org', '2011-07-25', 'Furniture', 'M', 146713, 4);
insert into employees values (186, 'Rory', 'Domel', 'rdomel55@yellowbook.com', '2007-08-30', 'Camping', 'F', 153133, 1);
insert into employees values (187, 'Read', 'Elcoux', 'relcoux56@cam.ac.uk', '2006-01-14', 'Tools', 'M', 41621, 5);
insert into employees values (188, 'Jerry', 'Novis', 'jnovis57@virginia.edu', '2015-12-07', 'Movies', 'F', 59229, 5);
insert into employees values (189, 'Donovan', 'Tynnan', 'dtynnan58@vk.com', '2011-01-03', 'First Aid', 'M', 139035, 2);
insert into employees values (190, 'Averyl', 'Weinmann', 'aweinmann59@google.com.au', '2014-10-12', 'Sports', 'F', 118250, 7);
insert into employees values (191, 'Marjorie', 'Leavey', 'mleavey5a@myspace.com', '2012-08-17', 'Sports', 'F', 130147, 5);
insert into employees values (192, 'Fonzie', 'Barukh', null, '2005-11-25', 'First Aid', 'M', 134991, 2);
insert into employees values (193, 'Fredrick', 'Cleen', 'fcleen5c@studiopress.com', '2010-04-04', 'Beauty', 'M', 106563, 1);
insert into employees values (194, 'Yardley', 'Vynarde', null, '2003-02-28', 'Jewelry', 'M', 26876, 1);
insert into employees values (195, 'Gilly', 'Gerold', 'ggerold5e@alibaba.com', '2005-07-07', 'Cosmetics', 'F', 85248, 6);
insert into employees values (196, 'Marylin', 'Crombleholme', 'mcrombleholme5f@wisc.edu', '2014-04-08', 'Music', 'F', 20776, 6);
insert into employees values (197, 'Ali', 'Arnaudet', 'aarnaudet5g@gizmodo.com', '2005-09-19', 'Decor', 'M', 65696, 4);
insert into employees values (198, 'Orrin', 'Janz', 'ojanz5h@cbsnews.com', '2007-08-09', 'Furniture', 'M', 73510, 5);
insert into employees values (199, 'Gabriel', 'Widocks', 'gwidocks5i@acquirethisname.com', '2012-05-01', 'Cosmetics', 'M', 154376, 5);
insert into employees values (200, 'Marjorie', 'Limeburn', null, '2012-01-06', 'First Aid', 'F', 96108, 3);
insert into employees values (201, 'Harvey', 'Georgins', 'hgeorgins5k@ustream.tv', '2013-11-15', 'First Aid', 'M', 45481, 5);
insert into employees values (202, 'Denney', 'Ducker', 'dducker5l@telegraph.co.uk', '2003-10-27', 'Children Clothing', 'M', 42447, 4);
insert into employees values (203, 'Lindsy', 'Coventry', 'lcoventry5m@example.com', '2015-01-18', 'Maintenance', 'F', 42370, 4);
insert into employees values (204, 'Willabella', 'Bachs', 'wbachs5n@free.fr', '2003-08-18', 'Beauty', 'F', 22053, 2);
insert into employees values (205, 'Cody', 'Monnoyer', 'cmonnoyer5o@amazon.co.uk', '2008-07-23', 'Games', 'F', 47559, 4);
insert into employees values (206, 'Cyndi', 'Danilchenko', null, '2008-05-29', 'Sports', 'F', 71364, 1);
insert into employees values (207, 'Willetta', 'Jaggard', 'wjaggard5q@stumbleupon.com', '2008-03-25', 'Computers', 'F', 43539, 1);
insert into employees values (208, 'Kimberly', 'Creeboe', 'kcreeboe5r@squarespace.com', '2008-04-03', 'Games', 'F', 25346, 1);
insert into employees values (209, 'Tabbi', 'Driuzzi', 'tdriuzzi5s@shinystat.com', '2003-12-22', 'Camping', 'F', 121072, 7);
insert into employees values (210, 'Lucien', 'Shayler', 'lshayler5t@elpais.com', '2004-06-11', 'Garden', 'M', 137410, 7);
insert into employees values (211, 'Michail', 'Leamy', 'mleamy5u@ted.com', '2011-03-07', 'Sports', 'M', 103760, 6);
insert into employees values (212, 'Izabel', 'Lowthorpe', 'ilowthorpe5v@state.gov', '2003-09-07', 'Camping', 'F', 142059, 4);
insert into employees values (213, 'Kristos', 'Stooders', null, '2013-04-22', 'Device Repair', 'M', 54570, 2);
insert into employees values (214, 'Nap', 'Corradetti', null, '2016-07-01', 'Jewelry', 'M', 144262, 6);
insert into employees values (215, 'Alisa', 'Allender', 'aallender5y@delicious.com', '2007-12-06', 'Music', 'F', 161283, 2);
insert into employees values (216, 'Abby', 'Seawright', 'aseawright5z@ask.com', '2011-09-01', 'Jewelry', 'F', 56889, 3);
insert into employees values (217, 'Sileas', 'Rushman', 'srushman60@dion.ne.jp', '2011-02-05', 'Toys', 'F', 118649, 6);
insert into employees values (218, 'Guenevere', 'Conlon', 'gconlon61@loc.gov', '2007-04-19', 'Toys', 'F', 69012, 2);
insert into employees values (219, 'Raquel', 'Seath', 'rseath62@nbcnews.com', '2005-02-02', 'Garden', 'F', 25587, 4);
insert into employees values (220, 'Isabella', 'Dovermann', null, '2012-09-21', 'Tools', 'F', 23582, 7);
insert into employees values (221, 'Curran', 'Ebdin', 'cebdin64@ezinearticles.com', '2007-12-01', 'Decor', 'M', 119684, 2);
insert into employees values (222, 'Lawton', 'Ponceford', 'lponceford65@state.tx.us', '2012-11-14', 'Clothing', 'M', 87108, 6);
insert into employees values (223, 'Levin', 'Churchard', 'lchurchard66@prnewswire.com', '2013-08-21', 'Camping', 'M', 159946, 5);
insert into employees values (224, 'Sutherlan', 'Grevel', null, '2013-09-21', 'Movies', 'M', 72967, 7);
insert into employees values (225, 'Lyn', 'Guppie', 'lguppie68@army.mil', '2003-11-01', 'Phones & Tablets', 'F', 41380, 4);
insert into employees values (226, 'Rustin', 'Simpson', 'rsimpson69@t-online.de', '2003-07-05', 'Tools', 'M', 38719, 3);
insert into employees values (227, 'Harli', 'Crosham', 'hcrosham6a@vkontakte.ru', '2008-11-18', 'Books', 'F', 106026, 5);
insert into employees values (228, 'Roze', 'Jakovijevic', 'rjakovijevic6b@gizmodo.com', '2015-01-12', 'Tools', 'F', 91778, 7);
insert into employees values (229, 'Evangelin', 'Hiddersley', 'ehiddersley6c@icio.us', '2007-05-06', 'Games', 'F', 53354, 7);
insert into employees values (230, 'Sebastian', 'Le feuvre', 'slefeuvre6d@abc.net.au', '2015-05-17', 'Device Repair', 'M', 157861, 1);
insert into employees values (231, 'Say', 'Alliberton', 'salliberton6e@technorati.com', '2014-08-16', 'Toys', 'M', 149707, 4);
insert into employees values (232, 'Adelaida', 'Peebles', 'apeebles6f@hatena.ne.jp', '2010-09-22', 'Movies', 'F', 50306, 7);
insert into employees values (233, 'Jameson', 'Popplestone', 'jpopplestone6g@google.de', '2012-02-24', 'Phones & Tablets', 'M', 126702, 1);
insert into employees values (234, 'Lew', 'Spanswick', 'lspanswick6h@paginegialle.it', '2014-08-06', 'Beauty', 'M', 30453, 7);
insert into employees values (235, 'Cary', 'Kelshaw', 'ckelshaw6i@alexa.com', '2015-09-13', 'Vitamins', 'M', 139145, 6);
insert into employees values (236, 'Morty', 'Buard', null, '2014-02-24', 'Tools', 'M', 100185, 2);
insert into employees values (237, 'Binni', 'Daily', 'bdaily6k@ucla.edu', '2007-06-01', 'Decor', 'F', 38707, 2);
insert into employees values (238, 'Bev', 'Howgate', 'bhowgate6l@amazon.co.jp', '2004-11-01', 'Camping', 'M', 98444, 4);
insert into employees values (239, 'Benedikta', 'Sherwill', 'bsherwill6m@mlb.com', '2005-06-22', 'Games', 'F', 72588, 6);
insert into employees values (240, 'Enrico', 'Hoopper', 'ehoopper6n@storify.com', '2010-11-15', 'Computers', 'M', 88597, 1);
insert into employees values (241, 'Constanta', 'Everett', 'ceverett6o@cargocollective.com', '2010-02-09', 'Music', 'F', 87497, 2);
insert into employees values (242, 'Teri', 'Mottershaw', 'tmottershaw6p@parallels.com', '2006-10-08', 'Games', 'F', 83713, 3);
insert into employees values (243, 'Howey', 'Woodyatt', 'hwoodyatt6q@vistaprint.com', '2013-09-08', 'Books', 'M', 71418, 3);
insert into employees values (244, 'Jaymee', 'Pessolt', 'jpessolt6r@soup.io', '2015-08-19', 'Movies', 'F', 120395, 6);
insert into employees values (245, 'Laure', 'Vedstra', 'lvedstra6s@va.gov', '2016-01-10', 'Tools', 'F', 25037, 4);
insert into employees values (246, 'Eddy', 'McCoole', 'emccoole6t@photobucket.com', '2003-05-28', 'Decor', 'M', 99124, 6);
insert into employees values (247, 'Tammie', 'Grishukov', null, '2011-12-08', 'Automotive', 'F', 160039, 5);
insert into employees values (248, 'Moe', 'Dobrowski', 'mdobrowski6v@comsenz.com', '2009-08-09', 'Jewelry', 'M', 39327, 5);
insert into employees values (249, 'Sterling', 'Pagen', 'spagen6w@privacy.gov.au', '2004-09-02', 'Automotive', 'M', 56095, 7);
insert into employees values (250, 'Jania', 'Larway', 'jlarway6x@skyrock.com', '2009-03-01', 'Music', 'F', 86683, 6);
insert into employees values (251, 'Stacee', 'Insoll', 'sinsoll6y@wordpress.org', '2014-07-13', 'Movies', 'M', 44736, 5);
insert into employees values (252, 'Eimile', 'Abadam', 'eabadam6z@slashdot.org', '2013-09-29', 'Furniture', 'F', 80285, 7);
insert into employees values (253, 'Raina', 'Halleybone', null, '2008-10-21', 'Jewelry', 'F', 101441, 7);
insert into employees values (254, 'Minna', 'Aleksankin', 'maleksankin71@sina.com.cn', '2007-01-21', 'Device Repair', 'F', 30486, 1);
insert into employees values (255, 'Shirleen', 'Remmer', 'sremmer72@accuweather.com', '2006-01-19', 'Cosmetics', 'F', 156449, 1);
insert into employees values (256, 'Neddy', 'Speachley', 'nspeachley73@washington.edu', '2007-04-26', 'Beauty', 'M', 151926, 4);
insert into employees values (257, 'Lois', 'Cianelli', 'lcianelli74@baidu.com', '2003-11-27', 'First Aid', 'F', 29539, 1);
insert into employees values (258, 'Paten', 'De Vuyst', 'pdevuyst75@vk.com', '2011-07-11', 'Grocery', 'M', 159723, 3);
insert into employees values (259, 'Reidar', 'Rudham', 'rrudham76@exblog.jp', '2013-06-30', 'Clothing', 'M', 31785, 7);
insert into employees values (260, 'Arabelle', 'Arch', 'aarch77@marriott.com', '2014-07-01', 'Pharmacy', 'F', 72662, 4);
insert into employees values (261, 'Shae', 'Farman', null, '2007-10-13', 'Children Clothing', 'F', 103608, 3);
insert into employees values (262, 'Elizabeth', 'Gilbart', 'egilbart79@hhs.gov', '2004-11-18', 'Toys', 'F', 55587, 1);
insert into employees values (263, 'Niles', 'Rodenborch', 'nrodenborch7a@reuters.com', '2015-05-27', 'Music', 'M', 29890, 3);
insert into employees values (264, 'Rory', 'Crace', 'rcrace7b@cornell.edu', '2014-10-04', 'Toys', 'M', 33544, 2);
insert into employees values (265, 'Renault', 'Lenchenko', 'rlenchenko7c@upenn.edu', '2016-07-03', 'Pharmacy', 'M', 20542, 7);
insert into employees values (266, 'Jarrett', 'Northfield', 'jnorthfield7d@globo.com', '2011-06-20', 'Phones & Tablets', 'M', 44501, 2);
insert into employees values (267, 'Stacee', 'Pawellek', 'spawellek7e@fotki.com', '2004-04-21', 'First Aid', 'M', 136707, 4);
insert into employees values (268, 'Max', 'Cammish', 'mcammish7f@google.nl', '2007-05-17', 'Device Repair', 'M', 37206, 2);
insert into employees values (269, 'Torrin', 'Stevenson', 'tstevenson7g@businessweek.com', '2008-06-26', 'Pharmacy', 'M', 127915, 7);
insert into employees values (270, 'Elsinore', 'Howle', 'ehowle7h@ebay.co.uk', '2014-05-13', 'Decor', 'F', 24876, 5);
insert into employees values (271, 'Norbie', 'Bleasdille', 'nbleasdille7i@foxnews.com', '2003-01-01', 'First Aid', 'M', 82215, 6);
insert into employees values (272, 'Roxie', 'Revance', 'rrevance7j@unesco.org', '2016-12-16', 'Phones & Tablets', 'F', 42224, 2);
insert into employees values (273, 'Yardley', 'Hames', null, '2016-01-27', 'Decor', 'M', 124800, 4);
insert into employees values (274, 'Lorelle', 'Kelberman', 'lkelberman7l@wired.com', '2004-01-27', 'Automotive', 'F', 119959, 7);
insert into employees values (275, 'Phyllis', 'Millhill', 'pmillhill7m@networkadvertising.org', '2014-06-11', 'Pharmacy', 'F', 88572, 2);
insert into employees values (276, 'Maye', 'Stockow', 'mstockow7n@sakura.ne.jp', '2015-09-22', 'Jewelry', 'F', 116120, 6);
insert into employees values (277, 'Gery', 'Blagburn', 'gblagburn7o@fc2.com', '2009-05-11', 'Tools', 'M', 35337, 5);
insert into employees values (278, 'Murray', 'McCosh', null, '2013-08-27', 'Beauty', 'M', 138181, 7);
insert into employees values (279, 'Spense', 'Phillip', 'sphillip7q@wp.com', '2004-03-13', 'Device Repair', 'M', 130786, 3);
insert into employees values (280, 'Timotheus', 'Curbishley', 'tcurbishley7r@free.fr', '2015-05-14', 'Children Clothing', 'M', 23159, 5);
insert into employees values (281, 'Alfy', 'Waggitt', 'awaggitt7s@plala.or.jp', '2014-03-16', 'Games', 'F', 48229, 4);
insert into employees values (282, 'Dunc', 'Bloxsum', 'dbloxsum7t@csmonitor.com', '2015-11-01', 'Clothing', 'M', 48192, 1);
insert into employees values (283, 'Curtice', 'Muddiman', 'cmuddiman7u@foxnews.com', '2007-11-10', 'Device Repair', 'M', 94233, 6);
insert into employees values (284, 'Hendrik', 'Garbutt', 'hgarbutt7v@google.ru', '2008-10-22', 'Jewelry', 'M', 163794, 2);
insert into employees values (285, 'Nolly', 'McCaig', null, '2010-09-09', 'Pharmacy', 'M', 46367, 3);
insert into employees values (286, 'Kariotta', 'Foystone', 'kfoystone7x@nymag.com', '2008-08-25', 'Clothing', 'F', 57375, 4);
insert into employees values (287, 'Sioux', 'Moorman', null, '2005-03-22', 'Cosmetics', 'F', 99293, 6);
insert into employees values (288, 'Buckie', 'Jodrellec', 'bjodrellec7z@vistaprint.com', '2016-10-10', 'Vitamins', 'M', 30289, 4);
insert into employees values (289, 'Wandis', 'Tigwell', 'wtigwell80@webeden.co.uk', '2014-02-07', 'Grocery', 'F', 151847, 3);
insert into employees values (290, 'Florrie', 'Albery', 'falbery81@latimes.com', '2016-07-02', 'Phones & Tablets', 'F', 111949, 5);
insert into employees values (291, 'Arvy', 'Rivilis', 'arivilis82@nba.com', '2003-03-16', 'Garden', 'M', 76125, 4);
insert into employees values (292, 'Norri', 'Tandey', 'ntandey83@sina.com.cn', '2008-04-26', 'Vitamins', 'F', 158847, 7);
insert into employees values (293, 'Robers', 'Giacomozzo', null, '2008-08-26', 'Toys', 'M', 161949, 5);
insert into employees values (294, 'Odey', 'Grouvel', 'ogrouvel85@simplemachines.org', '2008-11-28', 'Garden', 'M', 96638, 3);
insert into employees values (295, 'Sosanna', 'Giovanardi', 'sgiovanardi86@creativecommons.org', '2008-03-26', 'Phones & Tablets', 'F', 150485, 6);
insert into employees values (296, 'Alfons', 'Smeaton', 'asmeaton87@state.tx.us', '2009-10-23', 'Games', 'M', 112768, 7);
insert into employees values (297, 'Thorpe', 'Praton', null, '2005-08-12', 'Camping', 'M', 69622, 7);
insert into employees values (298, 'Charin', 'Heinicke', 'cheinicke89@arizona.edu', '2005-12-30', 'First Aid', 'F', 42847, 2);
insert into employees values (299, 'Urson', 'Strivens', 'ustrivens8a@amazon.de', '2014-07-17', 'Decor', 'M', 140672, 4);
insert into employees values (300, 'Cassandra', 'Hoston', 'choston8b@jugem.jp', '2003-01-01', 'Beauty', 'F', 106936, 7);
insert into employees values (301, 'Harley', 'Paish', 'hpaish8c@sitemeter.com', '2013-08-31', 'Pharmacy', 'F', 72504, 2);
insert into employees values (302, 'Fergus', 'Chesterton', 'fchesterton8d@harvard.edu', '2008-05-21', 'First Aid', 'M', 67689, 6);
insert into employees values (303, 'Lindy', 'Beining', 'lbeining8e@rambler.ru', '2015-01-03', 'Clothing', 'M', 48814, 2);
insert into employees values (304, 'Sherye', 'Pardy', 'spardy8f@wordpress.org', '2010-11-28', 'Children Clothing', 'F', 110872, 3);
insert into employees values (305, 'Ladonna', 'McCrow', 'lmccrow8g@nhs.uk', '2003-08-10', 'Automotive', 'F', 111775, 2);
insert into employees values (306, 'Cherye', 'Force', 'cforce8h@people.com.cn', '2012-08-04', 'Camping', 'F', 58190, 1);
insert into employees values (307, 'Parnell', 'Davidoff', 'pdavidoff8i@zimbio.com', '2004-03-29', 'Computers', 'M', 155000, 7);
insert into employees values (308, 'Carling', 'Crusham', 'ccrusham8j@cloudflare.com', '2014-06-05', 'Jewelry', 'M', 117960, 7);
insert into employees values (309, 'Kerrin', 'Marchington', null, '2005-06-22', 'Jewelry', 'F', 73350, 4);
insert into employees values (310, 'Archambault', 'Marriner', 'amarriner8l@angelfire.com', '2015-09-12', 'Vitamins', 'M', 123287, 2);
insert into employees values (311, 'Kamillah', 'Branthwaite', 'kbranthwaite8m@scientificamerican.com', '2012-01-12', 'Cosmetics', 'F', 153479, 1);
insert into employees values (312, 'Creigh', 'Divina', 'cdivina8n@tamu.edu', '2003-05-31', 'Furniture', 'M', 133537, 7);
insert into employees values (313, 'Swen', 'Pirrone', 'spirrone8o@live.com', '2012-09-11', 'Computers', 'M', 152304, 7);
insert into employees values (314, 'Phoebe', 'Joddens', 'pjoddens8p@dailymail.co.uk', '2010-01-26', 'Clothing', 'F', 45892, 3);
insert into employees values (315, 'Philis', 'Sutcliffe', 'psutcliffe8q@bloomberg.com', '2007-05-26', 'Device Repair', 'F', 45829, 5);
insert into employees values (316, 'Glynn', 'McCaughey', null, '2013-10-28', 'Clothing', 'M', 61614, 5);
insert into employees values (317, 'Addy', 'Warlock', 'awarlock8s@oracle.com', '2014-03-14', 'Toys', 'F', 101112, 3);
insert into employees values (318, 'Matt', 'Jasik', 'mjasik8t@nytimes.com', '2015-02-07', 'Cosmetics', 'M', 90428, 1);
insert into employees values (319, 'Carmelita', 'Sharram', null, '2016-04-21', 'Pharmacy', 'F', 144217, 1);
insert into employees values (320, 'Dalli', 'Percy', 'dpercy8v@auda.org.au', '2006-06-04', 'First Aid', 'M', 136545, 7);
insert into employees values (321, 'Carline', 'Lissemore', null, '2003-12-06', 'Camping', 'F', 87550, 3);
insert into employees values (322, 'Freeland', 'Brotherheed', 'fbrotherheed8x@nationalgeographic.com', '2015-04-22', 'Tools', 'M', 70638, 5);
insert into employees values (323, 'Meredithe', 'Lissaman', null, '2012-02-02', 'Clothing', 'F', 89695, 4);
insert into employees values (324, 'Ellyn', 'Timewell', 'etimewell8z@sciencedirect.com', '2013-08-12', 'Jewelry', 'F', 154491, 1);
insert into employees values (325, 'Aldo', 'Piet', 'apiet90@github.io', '2007-11-16', 'Pharmacy', 'M', 138055, 1);
insert into employees values (326, 'Rodrique', 'MacEveley', 'rmaceveley91@so-net.ne.jp', '2010-05-02', 'Decor', 'M', 69333, 1);
insert into employees values (327, 'Alexina', 'Ditchfield', 'aditchfield92@sogou.com', '2015-07-08', 'First Aid', 'F', 72540, 3);
insert into employees values (328, 'Haily', 'Cornwell', 'hcornwell93@flavors.me', '2016-06-07', 'Movies', 'F', 26341, 1);
insert into employees values (329, 'Daryl', 'Seedull', 'dseedull94@irs.gov', '2004-10-14', 'First Aid', 'M', 62561, 6);
insert into employees values (330, 'Ned', 'Hanhard', 'nhanhard95@godaddy.com', '2008-12-25', 'Games', 'M', 49877, 2);
insert into employees values (331, 'Aldwin', 'Frear', 'afrear96@marketwatch.com', '2007-12-05', 'Garden', 'M', 51424, 4);
insert into employees values (332, 'Ame', 'Pateman', 'apateman97@ca.gov', '2003-07-13', 'Vitamins', 'F', 21931, 2);
insert into employees values (333, 'Javier', 'Rosendale', 'jrosendale98@ca.gov', '2003-11-12', 'Computers', 'M', 87199, 1);
insert into employees values (334, 'Webb', 'Wellen', null, '2005-10-13', 'Computers', 'M', 152504, 7);
insert into employees values (335, 'Tripp', 'Tibbs', 'ttibbs9a@amazonaws.com', '2009-07-31', 'Books', 'M', 111798, 7);
insert into employees values (336, 'Alverta', 'Duffell', 'aduffell9b@google.co.jp', '2004-08-28', 'Furniture', 'F', 61754, 6);
insert into employees values (337, 'Eden', 'Instock', 'einstock9c@seattletimes.com', '2010-11-28', 'Sports', 'F', 30836, 1);
insert into employees values (338, 'Peggi', 'Chislett', 'pchislett9d@si.edu', '2003-11-16', 'Jewelry', 'F', 59378, 6);
insert into employees values (339, 'Kimberlyn', 'Tomanek', 'ktomanek9e@webmd.com', '2006-08-29', 'Movies', 'F', 27546, 5);
insert into employees values (340, 'Ainsley', 'Scotchmer', 'ascotchmer9f@phpbb.com', '2015-02-27', 'Device Repair', 'F', 114170, 3);
insert into employees values (341, 'Valdemar', 'Regi', 'vregi9g@over-blog.com', '2006-03-19', 'Cosmetics', 'M', 86079, 7);
insert into employees values (342, 'Wandis', 'Durrant', 'wdurrant9h@is.gd', '2014-01-24', 'Children Clothing', 'F', 78689, 1);
insert into employees values (343, 'Maridel', 'Whellans', 'mwhellans9i@hud.gov', '2014-12-05', 'Vitamins', 'F', 24884, 1);
insert into employees values (344, 'Daren', 'Cattermull', null, '2012-11-26', 'Vitamins', 'M', 67549, 4);
insert into employees values (345, 'Paulo', 'Radden', null, '2006-05-09', 'Computers', 'M', 108187, 1);
insert into employees values (346, 'Taite', 'Oats', 'toats9l@google.com.hk', '2016-06-08', 'Children Clothing', 'M', 82106, 3);
insert into employees values (347, 'Efrem', 'Manifould', 'emanifould9m@google.com.br', '2006-09-22', 'Beauty', 'M', 56615, 3);
insert into employees values (348, 'Jacklyn', 'Finlator', 'jfinlator9n@sphinn.com', '2004-01-04', 'Clothing', 'F', 166976, 4);
insert into employees values (349, 'Christoforo', 'Kringe', 'ckringe9o@about.me', '2006-02-20', 'Decor', 'M', 23989, 7);
insert into employees values (350, 'Rafaello', 'Bridson', null, '2005-01-11', 'Movies', 'M', 159463, 4);
insert into employees values (351, 'Giana', 'Lothean', 'glothean9q@ox.ac.uk', '2004-10-05', 'Plumbing', 'F', 144363, 6);
insert into employees values (352, 'Elianora', 'Stepney', null, '2007-04-18', 'Games', 'F', 117128, 1);
insert into employees values (353, 'Garrot', 'Geldart', 'ggeldart9s@smugmug.com', '2006-07-10', 'Beauty', 'M', 28293, 1);
insert into employees values (354, 'Brittaney', 'Bartlomiej', 'bbartlomiej9t@zimbio.com', '2010-06-06', 'Toys', 'F', 124943, 2);
insert into employees values (355, 'Wendell', 'Whittington', null, '2009-06-23', 'Beauty', 'M', 82130, 6);
insert into employees values (356, 'Kevin', 'Schubart', 'kschubart9v@dailymotion.com', '2011-01-20', 'Camping', 'M', 154856, 7);
insert into employees values (357, 'Petey', 'Edmeads', 'pedmeads9w@example.com', '2011-06-18', 'Movies', 'M', 102539, 1);
insert into employees values (358, 'Georgi', 'Tesh', null, '2015-03-12', 'Movies', 'M', 139587, 7);
insert into employees values (359, 'Francesco', 'Leggin', 'fleggin9y@163.com', '2005-12-11', 'Toys', 'M', 89967, 7);
insert into employees values (360, 'Preston', 'Holligan', 'pholligan9z@shutterfly.com', '2010-06-18', 'Device Repair', 'M', 26582, 7);
insert into employees values (361, 'Salomi', 'Yalden', 'syaldena0@webs.com', '2012-12-08', 'Music', 'F', 38525, 2);
insert into employees values (362, 'Ira', 'Hollier', 'iholliera1@tamu.edu', '2015-03-28', 'Garden', 'F', 68937, 7);
insert into employees values (363, 'Angie', 'Mation', null, '2013-07-10', 'Device Repair', 'F', 150873, 4);
insert into employees values (364, 'Conrad', 'Brognot', 'cbrognota3@latimes.com', '2016-04-21', 'Toys', 'M', 154205, 1);
insert into employees values (365, 'Joshua', 'Gyse', null, '2016-03-28', 'Garden', 'M', 98439, 1);
insert into employees values (366, 'Lorne', 'Hughson', 'lhughsona5@yelp.com', '2010-01-23', 'Tools', 'M', 50223, 5);
insert into employees values (367, 'Lauretta', 'Rounds', 'lroundsa6@wordpress.org', '2007-12-14', 'Automotive', 'F', 75978, 6);
insert into employees values (368, 'Duke', 'Samart', 'dsamarta7@wikipedia.org', '2008-03-11', 'Device Repair', 'M', 40727, 5);
insert into employees values (369, 'Kincaid', 'Beaby', 'kbeabya8@fastcompany.com', '2011-03-04', 'Jewelry', 'M', 92218, 3);
insert into employees values (370, 'Genvieve', 'Aherne', null, '2008-06-20', 'Music', 'F', 118649, 5);
insert into employees values (371, 'Malcolm', 'D''Costa', 'mdcostaaa@wikispaces.com', '2016-11-24', 'Garden', 'M', 138493, 1);
insert into employees values (372, 'Chantalle', 'Campes', 'ccampesab@discuz.net', '2010-03-09', 'Furniture', 'F', 83195, 5);
insert into employees values (373, 'Susan', 'Andreone', 'sandreoneac@latimes.com', '2012-12-06', 'Garden', 'F', 79827, 7);
insert into employees values (374, 'Cherilyn', 'Pheasey', 'cpheaseyad@japanpost.jp', '2003-07-05', 'Grocery', 'F', 67359, 4);
insert into employees values (375, 'Ellene', 'Wallwork', 'ewallworkae@parallels.com', '2015-11-09', 'Garden', 'F', 22326, 1);
insert into employees values (376, 'Euphemia', 'Tytcomb', null, '2007-04-18', 'Decor', 'F', 132618, 1);
insert into employees values (377, 'Benyamin', 'Reddyhoff', 'breddyhoffag@loc.gov', '2016-03-25', 'Clothing', 'M', 35593, 2);
insert into employees values (378, 'Robin', 'Pooly', 'rpoolyah@spiegel.de', '2005-04-07', 'Pharmacy', 'M', 128729, 6);
insert into employees values (379, 'Mandel', 'Beddoes', null, '2013-09-30', 'Furniture', 'M', 84572, 4);
insert into employees values (380, 'Edik', 'Wardhough', 'ewardhoughaj@businesswire.com', '2016-12-11', 'Tools', 'M', 88378, 2);
insert into employees values (381, 'Retha', 'Debney', 'rdebneyak@indiegogo.com', '2004-06-29', 'Computers', 'F', 74771, 5);
insert into employees values (382, 'Allx', 'Paraman', 'aparamanal@irs.gov', '2007-05-19', 'Books', 'F', 156535, 3);
insert into employees values (383, 'Dun', 'Draisey', 'ddraiseyam@printfriendly.com', '2004-12-31', 'Phones & Tablets', 'M', 82064, 2);
insert into employees values (384, 'Marc', 'Costley', 'mcostleyan@photobucket.com', '2013-09-06', 'Cosmetics', 'M', 158810, 4);
insert into employees values (385, 'Doe', 'Larkworthy', 'dlarkworthyao@amazon.de', '2014-10-14', 'Automotive', 'F', 106046, 1);
insert into employees values (386, 'Lacee', 'Haddeston', 'lhaddestonap@soundcloud.com', '2006-11-27', 'Beauty', 'F', 111691, 2);
insert into employees values (387, 'Marijo', 'Hostan', 'mhostanaq@ameblo.jp', '2015-04-01', 'Phones & Tablets', 'F', 71197, 7);
insert into employees values (388, 'Maryrose', 'Carmen', null, '2011-04-28', 'Grocery', 'F', 124581, 4);
insert into employees values (389, 'Ninetta', 'Barwick', 'nbarwickas@github.io', '2008-01-29', 'Music', 'F', 48186, 3);
insert into employees values (390, 'Kent', 'Byford', 'kbyfordat@time.com', '2006-07-18', 'Computers', 'M', 100379, 6);
insert into employees values (391, 'Enrique', 'Rogeon', 'erogeonau@mediafire.com', '2010-01-26', 'Movies', 'M', 108612, 2);
insert into employees values (392, 'Bronny', 'Burnard', 'bburnardav@admin.ch', '2007-01-05', 'First Aid', 'M', 148802, 6);
insert into employees values (393, 'April', 'Whetnell', 'awhetnellaw@drupal.org', '2010-07-21', 'Books', 'F', 56446, 2);
insert into employees values (394, 'Stormy', 'Najafian', null, '2015-07-28', 'Automotive', 'F', 126983, 6);
insert into employees values (395, 'Garold', 'Chasney', 'gchasneyay@house.gov', '2016-02-21', 'Furniture', 'M', 118100, 7);
insert into employees values (396, 'Ferrel', 'Barnett', 'fbarnettaz@photobucket.com', '2015-05-13', 'Phones & Tablets', 'M', 142158, 1);
insert into employees values (397, 'Sheffie', 'Caddies', null, '2014-05-28', 'Jewelry', 'M', 78104, 6);
insert into employees values (398, 'Gustavo', 'Jollands', 'gjollandsb1@constantcontact.com', '2014-03-01', 'Sports', 'M', 77085, 3);
insert into employees values (399, 'Chilton', 'Trewhella', 'ctrewhellab2@biglobe.ne.jp', '2004-04-15', 'Garden', 'M', 38655, 5);
insert into employees values (400, 'Kermy', 'Faulo', 'kfaulob3@oracle.com', '2016-08-13', 'Grocery', 'M', 35931, 7);
insert into employees values (401, 'Willard', 'Parrish', 'wparrishb4@soundcloud.com', '2008-08-04', 'Furniture', 'M', 39178, 6);
insert into employees values (402, 'Filippa', 'Frean', 'ffreanb5@ca.gov', '2004-02-20', 'Clothing', 'F', 44967, 6);
insert into employees values (403, 'Wyndham', 'Bavester', 'wbavesterb6@senate.gov', '2012-02-11', 'Children Clothing', 'M', 113211, 3);
insert into employees values (404, 'Ripley', 'Haldene', 'rhaldeneb7@blogspot.com', '2012-04-23', 'Jewelry', 'M', 65609, 3);
insert into employees values (405, 'Mirelle', 'Glusby', 'mglusbyb8@spotify.com', '2016-08-27', 'Device Repair', 'F', 23051, 6);
insert into employees values (406, 'Ingrim', 'Simonitto', 'isimonittob9@apache.org', '2014-12-20', 'Phones & Tablets', 'M', 158148, 6);
insert into employees values (407, 'Annie', 'Rattry', 'arattryba@typepad.com', '2007-12-10', 'Computers', 'F', 106737, 7);
insert into employees values (408, 'Frederico', 'McCory', 'fmccorybb@ask.com', '2006-01-03', 'Pharmacy', 'M', 23915, 3);
insert into employees values (409, 'Kimberley', 'Devereu', null, '2004-01-08', 'Computers', 'F', 49788, 1);
insert into employees values (410, 'Nadia', 'Jeacocke', 'njeacockebd@miitbeian.gov.cn', '2010-10-24', 'Cosmetics', 'F', 97848, 1);
insert into employees values (411, 'Jodi', 'Barwise', 'jbarwisebe@ehow.com', '2006-03-29', 'Toys', 'F', 127398, 4);
insert into employees values (412, 'Anitra', 'Hanaby', 'ahanabybf@weibo.com', '2007-09-10', 'Phones & Tablets', 'F', 97722, 5);
insert into employees values (413, 'Kerry', 'Nystrom', 'knystrombg@shop-pro.jp', '2007-06-14', 'Plumbing', 'F', 50934, 1);
insert into employees values (414, 'Patricio', 'Lapthorn', null, '2011-02-25', 'Phones & Tablets', 'M', 26453, 5);
insert into employees values (415, 'Borg', 'Plews', 'bplewsbi@wordpress.org', '2006-11-23', 'Jewelry', 'M', 109413, 6);
insert into employees values (416, 'Manolo', 'Garling', 'mgarlingbj@comsenz.com', '2012-06-25', 'Vitamins', 'M', 146293, 5);
insert into employees values (417, 'Gleda', 'Kivelle', 'gkivellebk@issuu.com', '2015-09-30', 'Decor', 'F', 67410, 4);
insert into employees values (418, 'Bryce', 'Lahiff', 'blahiffbl@europa.eu', '2006-04-02', 'Jewelry', 'M', 45077, 6);
insert into employees values (419, 'Glyn', 'Broinlich', 'gbroinlichbm@mtv.com', '2005-02-09', 'Cosmetics', 'M', 101689, 2);
insert into employees values (420, 'Ivett', 'Brierley', null, '2016-03-18', 'Vitamins', 'F', 64753, 6);
insert into employees values (421, 'Nalani', 'Latimer', 'nlatimerbo@sun.com', '2013-11-03', 'Tools', 'F', 59281, 2);
insert into employees values (422, 'Malory', 'Yea', 'myeabp@flavors.me', '2012-07-16', 'Pharmacy', 'F', 107893, 6);
insert into employees values (423, 'Gav', 'Cohn', null, '2008-07-18', 'Sports', 'M', 115978, 3);
insert into employees values (424, 'Yasmin', 'Greystoke', 'ygreystokebr@google.fr', '2005-02-07', 'Books', 'F', 58104, 4);
insert into employees values (425, 'Ki', 'Churly', 'kchurlybs@yandex.ru', '2005-09-09', 'Decor', 'F', 92180, 5);
insert into employees values (426, 'Cal', 'Goacher', 'cgoacherbt@comcast.net', '2008-07-12', 'Cosmetics', 'F', 162454, 7);
insert into employees values (427, 'Robenia', 'Dietmar', 'rdietmarbu@csmonitor.com', '2009-05-13', 'Toys', 'F', 118338, 2);
insert into employees values (428, 'Sidney', 'Buntine', 'sbuntinebv@senate.gov', '2004-03-17', 'Pharmacy', 'M', 29992, 2);
insert into employees values (429, 'Flory', 'Bevens', 'fbevensbw@etsy.com', '2012-05-28', 'Device Repair', 'M', 81690, 4);
insert into employees values (430, 'Anatola', 'Daulton', 'adaultonbx@ftc.gov', '2003-12-14', 'Movies', 'F', 92703, 5);
insert into employees values (431, 'Guntar', 'Finden', 'gfindenby@creativecommons.org', '2006-09-02', 'Movies', 'M', 39568, 7);
insert into employees values (432, 'Alister', 'Worsfold', 'aworsfoldbz@tinypic.com', '2011-05-19', 'Computers', 'M', 90751, 7);
insert into employees values (433, 'Deeyn', 'Halmkin', 'dhalmkinc0@comcast.net', '2007-10-04', 'First Aid', 'F', 37501, 2);
insert into employees values (434, 'Clementina', 'Frankcombe', 'cfrankcombec1@foxnews.com', '2016-09-04', 'Automotive', 'F', 95492, 1);
insert into employees values (435, 'Valenka', 'Morales', 'vmoralesc2@omniture.com', '2016-05-26', 'Beauty', 'F', 115627, 4);
insert into employees values (436, 'Sue', 'Synke', 'ssynkec3@hibu.com', '2004-10-14', 'Grocery', 'F', 148697, 3);
insert into employees values (437, 'Karlee', 'Broughton', 'kbroughtonc4@ibm.com', '2014-06-08', 'Cosmetics', 'F', 152695, 2);
insert into employees values (438, 'Betsey', 'Reedshaw', 'breedshawc5@phoca.cz', '2012-02-10', 'Automotive', 'F', 152141, 2);
insert into employees values (439, 'Yancy', 'Marunchak', 'ymarunchakc6@hubpages.com', '2010-03-24', 'Children Clothing', 'M', 158546, 3);
insert into employees values (440, 'Megan', 'Chilver', null, '2011-04-19', 'Furniture', 'F', 82859, 6);
insert into employees values (441, 'Olenolin', 'Lucy', 'olucyc8@china.com.cn', '2008-01-05', 'Furniture', 'M', 83712, 7);
insert into employees values (442, 'Elvira', 'Rubroe', 'erubroec9@instagram.com', '2005-08-29', 'Clothing', 'F', 50300, 6);
insert into employees values (443, 'Mayer', 'Bownde', 'mbowndeca@woothemes.com', '2010-01-24', 'Garden', 'M', 153513, 3);
insert into employees values (444, 'Roslyn', 'Purse', 'rpursecb@narod.ru', '2011-04-06', 'Children Clothing', 'F', 42605, 2);
insert into employees values (445, 'Nehemiah', 'Offin', 'noffincc@paypal.com', '2012-08-26', 'Beauty', 'M', 48788, 5);
insert into employees values (446, 'Charmion', 'Cambden', 'ccambdencd@abc.net.au', '2011-11-25', 'Toys', 'F', 96393, 4);
insert into employees values (447, 'Marybelle', 'Seden', 'msedence@google.com.hk', '2008-07-17', 'Computers', 'F', 108672, 1);
insert into employees values (448, 'Benni', 'Wenden', 'bwendencf@usatoday.com', '2004-09-24', 'Jewelry', 'F', 101509, 6);
insert into employees values (449, 'Brenn', 'Garley', 'bgarleycg@baidu.com', '2009-04-22', 'Movies', 'F', 91689, 5);
insert into employees values (450, 'Chantal', 'Griffoen', null, '2011-07-20', 'Clothing', 'F', 104667, 5);
insert into employees values (451, 'Henderson', 'Forlonge', 'hforlongeci@ycombinator.com', '2010-09-23', 'Toys', 'M', 108569, 4);
insert into employees values (452, 'Bradley', 'Tolliday', 'btollidaycj@gov.uk', '2007-05-05', 'Vitamins', 'M', 55793, 1);
insert into employees values (453, 'Austina', 'Riggoll', 'ariggollck@hostgator.com', '2011-09-05', 'Children Clothing', 'F', 28507, 6);
insert into employees values (454, 'Mill', 'Roust', 'mroustcl@wufoo.com', '2008-11-12', 'Beauty', 'M', 96023, 2);
insert into employees values (455, 'Keen', 'Kasman', 'kkasmancm@webmd.com', '2014-02-15', 'Children Clothing', 'M', 127363, 1);
insert into employees values (456, 'Jessalyn', 'Horley', 'jhorleycn@bluehost.com', '2004-10-03', 'Automotive', 'F', 86929, 7);
insert into employees values (457, 'Gleda', 'Deboo', null, '2010-06-16', 'Tools', 'F', 87481, 4);
insert into employees values (458, 'Rob', 'Medwell', 'rmedwellcp@dyndns.org', '2014-01-13', 'First Aid', 'M', 164011, 5);
insert into employees values (459, 'Lauree', 'Asken', 'laskencq@icq.com', '2008-12-11', 'Beauty', 'F', 95398, 2);
insert into employees values (460, 'Cherianne', 'Oxnam', null, '2016-12-18', 'Automotive', 'F', 150821, 6);
insert into employees values (461, 'Stefano', 'Greener', 'sgreenercs@bbc.co.uk', '2015-05-16', 'Sports', 'M', 61867, 7);
insert into employees values (462, 'Patsy', 'Drewry', 'pdrewryct@friendfeed.com', '2009-01-27', 'Tools', 'F', 79453, 6);
insert into employees values (463, 'Chastity', 'Hancox', 'chancoxcu@netvibes.com', '2005-09-03', 'Jewelry', 'F', 30260, 4);
insert into employees values (464, 'Caresse', 'Christofor', 'cchristoforcv@slate.com', '2006-02-23', 'Garden', 'F', 73013, 1);
insert into employees values (465, 'Aggie', 'Stebbings', 'astebbingscw@unesco.org', '2013-03-15', 'Toys', 'F', 140189, 4);
insert into employees values (466, 'Sonnnie', 'Arch', 'sarchcx@nydailynews.com', '2009-10-11', 'Toys', 'F', 109849, 3);
insert into employees values (467, 'Eunice', 'Spurling', null, '2010-05-16', 'First Aid', 'F', 33569, 3);
insert into employees values (468, 'Jessee', 'Bruck', 'jbruckcz@jalbum.net', '2012-08-09', 'Furniture', 'M', 101485, 6);
insert into employees values (469, 'Stanwood', 'Govey', 'sgoveyd0@deliciousdays.com', '2015-08-27', 'Cosmetics', 'M', 152382, 5);
insert into employees values (470, 'Hallsy', 'McBrier', null, '2015-12-31', 'Children Clothing', 'M', 98649, 5);
insert into employees values (471, 'Goldarina', 'Sweet', null, '2006-08-09', 'Decor', 'F', 137941, 4);
insert into employees values (472, 'Westbrooke', 'Tilford', 'wtilfordd3@imdb.com', '2014-03-28', 'Camping', 'M', 96080, 2);
insert into employees values (473, 'Peadar', 'Udell', 'pudelld4@dell.com', '2013-01-23', 'Grocery', 'M', 93956, 5);
insert into employees values (474, 'Bryna', 'Rops', 'bropsd5@amazon.com', '2011-04-18', 'Sports', 'F', 30762, 1);
insert into employees values (475, 'Carly', 'Lugton', 'clugtond6@japanpost.jp', '2005-03-26', 'Phones & Tablets', 'M', 123449, 2);
insert into employees values (476, 'Claybourne', 'Jados', 'cjadosd7@usda.gov', '2007-10-13', 'First Aid', 'M', 33693, 1);
insert into employees values (477, 'Fredia', 'Woolis', 'fwoolisd8@illinois.edu', '2016-06-14', 'Camping', 'F', 129658, 3);
insert into employees values (478, 'Levi', 'Rudge', null, '2003-10-21', 'Computers', 'M', 35076, 6);
insert into employees values (479, 'Wesley', 'Gurley', 'wgurleyda@google.co.uk', '2012-08-24', 'Pharmacy', 'M', 107851, 3);
insert into employees values (480, 'Roger', 'Spurdon', 'rspurdondb@alexa.com', '2006-01-01', 'Device Repair', 'M', 20664, 6);
insert into employees values (481, 'Tawnya', 'Fatkin', 'tfatkindc@who.int', '2013-11-02', 'Plumbing', 'F', 126532, 2);
insert into employees values (482, 'Garald', 'Sunman', null, '2008-10-13', 'Beauty', 'M', 145225, 2);
insert into employees values (483, 'Cathrine', 'Barneville', 'cbarnevillede@pagesperso-orange.fr', '2007-05-29', 'Camping', 'F', 154671, 3);
insert into employees values (484, 'Jefferson', 'Priscott', 'jpriscottdf@printfriendly.com', '2014-03-07', 'Toys', 'M', 78047, 4);
insert into employees values (485, 'Kristoffer', 'Benwell', 'kbenwelldg@whitehouse.gov', '2015-05-02', 'Jewelry', 'M', 94938, 2);
insert into employees values (486, 'Bear', 'Sessions', 'bsessionsdh@youtube.com', '2003-03-02', 'Decor', 'M', 143117, 3);
insert into employees values (487, 'Hermione', 'Bellhanger', null, '2010-11-07', 'Music', 'F', 164219, 2);
insert into employees values (488, 'Eugenius', 'Siege', 'esiegedj@gizmodo.com', '2003-01-26', 'Toys', 'M', 152118, 1);
insert into employees values (489, 'Viv', 'Alker', null, '2008-05-02', 'Decor', 'F', 152618, 1);
insert into employees values (490, 'Pascale', 'Heball', 'pheballdl@earthlink.net', '2004-04-15', 'Cosmetics', 'M', 55321, 7);
insert into employees values (491, 'Eloisa', 'Eeles', null, '2016-12-02', 'Clothing', 'F', 39200, 4);
insert into employees values (492, 'Christan', 'Marikhin', 'cmarikhindn@mapy.cz', '2004-01-12', 'Movies', 'F', 25840, 2);
insert into employees values (493, 'Nicolis', 'Vigers', 'nvigersdo@t.co', '2014-04-28', 'Children Clothing', 'M', 137567, 7);
insert into employees values (494, 'Horatius', 'Ferrulli', 'hferrullidp@guardian.co.uk', '2004-06-20', 'Pharmacy', 'M', 33152, 5);
insert into employees values (495, 'Mill', 'Makey', null, '2011-01-08', 'Automotive', 'M', 162522, 7);
insert into employees values (496, 'Jephthah', 'Huffy', 'jhuffydr@freewebs.com', '2012-05-29', 'Tools', 'M', 78984, 6);
insert into employees values (497, 'Marlena', 'Climo', 'mclimods@cargocollective.com', '2008-02-29', 'Movies', 'F', 99807, 6);
insert into employees values (498, 'Krystalle', 'Worcester', null, '2003-05-05', 'Decor', 'F', 135377, 4);
insert into employees values (499, 'Tamar', 'Crosson', 'tcrossondu@spiegel.de', '2005-05-27', 'Books', 'F', 125036, 4);
insert into employees values (500, 'Devondra', 'Bannester', 'dbannesterdv@hibu.com', '2012-03-05', 'First Aid', 'F', 94635, 7);
insert into employees values (501, 'Marlane', 'Sawney', 'msawneydw@mediafire.com', '2011-05-27', 'First Aid', 'F', 50520, 1);
insert into employees values (502, 'Darbie', 'Morando', 'dmorandodx@bizjournals.com', '2015-10-24', 'Sports', 'F', 98668, 4);
insert into employees values (503, 'Dennison', 'Redier', 'dredierdy@last.fm', '2015-11-20', 'Pharmacy', 'M', 83160, 5);
insert into employees values (504, 'Kori', 'Phare', 'kpharedz@va.gov', '2016-04-26', 'Device Repair', 'F', 118995, 3);
insert into employees values (505, 'Corabel', 'Scarse', 'cscarsee0@blog.com', '2004-03-24', 'Security', 'F', 36641, 6);
insert into employees values (506, 'Bartholemy', 'Crudginton', 'bcrudgintone1@dion.ne.jp', '2015-11-08', 'Vitamins', 'M', 25238, 6);
insert into employees values (507, 'Duke', 'Ashford', 'dashforde2@networkadvertising.org', '2005-11-02', 'Children Clothing', 'M', 104397, 4);
insert into employees values (508, 'Asher', 'McCrainor', 'amccrainore3@google.de', '2004-08-25', 'Clothing', 'M', 67857, 6);
insert into employees values (509, 'Brooks', 'Chasemore', 'bchasemoree4@gizmodo.com', '2012-08-12', 'Children Clothing', 'F', 72041, 1);
insert into employees values (510, 'Olenka', 'Burde', null, '2004-01-07', 'Children Clothing', 'F', 114431, 2);
insert into employees values (511, 'Baxter', 'Grahlman', null, '2006-07-18', 'Beauty', 'M', 154018, 3);
insert into employees values (512, 'Rutherford', 'Ennor', null, '2005-12-08', 'Children Clothing', 'M', 74795, 5);
insert into employees values (513, 'Basile', 'Kainz', null, '2003-06-12', 'Jewelry', 'M', 86269, 6);
insert into employees values (514, 'Ashia', 'Breeton', 'abreetone9@upenn.edu', '2004-09-11', 'Decor', 'F', 40464, 4);
insert into employees values (515, 'Cybil', 'Perez', 'cperezea@a8.net', '2004-04-01', 'Automotive', 'F', 123828, 1);
insert into employees values (516, 'Doralin', 'Spada', null, '2010-03-14', 'Device Repair', 'F', 155385, 2);
insert into employees values (517, 'Darell', 'Leyburn', 'dleyburnec@xinhuanet.com', '2004-03-07', 'Movies', 'F', 70928, 3);
insert into employees values (518, 'Alfons', 'Marklin', 'amarklined@cyberchimps.com', '2007-10-29', 'Garden', 'M', 37592, 5);
insert into employees values (519, 'Nev', 'Sebring', 'nsebringee@canalblog.com', '2011-03-06', 'Garden', 'M', 89353, 5);
insert into employees values (520, 'Harold', 'Landa', 'hlandaef@apache.org', '2016-09-22', 'Garden', 'M', 105274, 1);
insert into employees values (521, 'Maggie', 'Gainseford', 'mgainsefordeg@weibo.com', '2003-12-27', 'Device Repair', 'F', 43281, 6);
insert into employees values (522, 'Claribel', 'Kettow', 'ckettoweh@bbc.co.uk', '2011-07-18', 'Beauty', 'F', 22348, 2);
insert into employees values (523, 'Beatrisa', 'Acom', 'bacomei@webmd.com', '2013-07-28', 'Movies', 'F', 84877, 4);
insert into employees values (524, 'Esme', 'Gostick', 'egostickej@hugedomains.com', '2003-08-02', 'Sports', 'M', 51318, 5);
insert into employees values (525, 'Kristin', 'Rymell', 'krymellek@liveinternet.ru', '2005-07-07', 'Clothing', 'F', 51682, 2);
insert into employees values (526, 'Montgomery', 'Lamont', null, '2016-02-06', 'Beauty', 'M', 115964, 7);
insert into employees values (527, 'Bonnee', 'Strethill', 'bstrethillem@a8.net', '2016-04-22', 'Cosmetics', 'F', 147906, 6);
insert into employees values (528, 'Phoebe', 'Reame', 'preameen@noaa.gov', '2003-10-12', 'Books', 'F', 158680, 5);
insert into employees values (529, 'Cornelia', 'Bedingfield', 'cbedingfieldeo@feedburner.com', '2014-08-07', 'Furniture', 'F', 85129, 6);
insert into employees values (530, 'Jeramie', 'Readie', 'jreadieep@google.it', '2009-07-07', 'Phones & Tablets', 'M', 59578, 7);
insert into employees values (531, 'Patty', 'Halfhead', null, '2014-11-30', 'Games', 'M', 152615, 2);
insert into employees values (532, 'Marlie', 'Toler', 'mtolerer@ifeng.com', '2004-10-20', 'Toys', 'F', 156058, 5);
insert into employees values (533, 'Chastity', 'Labat', 'clabates@loc.gov', '2014-07-24', 'Computers', 'F', 103655, 2);
insert into employees values (534, 'Beale', 'Wooton', 'bwootonet@nytimes.com', '2007-04-23', 'Games', 'M', 116031, 6);
insert into employees values (535, 'Peyton', 'Grioli', null, '2012-05-13', 'Games', 'M', 137463, 4);
insert into employees values (536, 'Addia', 'Dannel', null, '2009-11-22', 'Grocery', 'F', 20613, 5);
insert into employees values (537, 'Geneva', 'Borth', 'gborthew@wordpress.com', '2009-07-26', 'Children Clothing', 'F', 44857, 7);
insert into employees values (538, 'Tammie', 'Cratere', 'tcratereex@sourceforge.net', '2014-09-11', 'Games', 'M', 107579, 6);
insert into employees values (539, 'Fulton', 'Penny', null, '2013-12-18', 'Beauty', 'M', 121990, 3);
insert into employees values (540, 'Cody', 'Stodit', 'cstoditez@thetimes.co.uk', '2003-10-05', 'Sports', 'M', 87813, 1);
insert into employees values (541, 'Adrian', 'Vase', 'avasef0@tmall.com', '2009-08-14', 'Music', 'F', 41871, 7);
insert into employees values (542, 'Ricard', 'Lyptrit', null, '2005-10-18', 'Toys', 'M', 93232, 6);
insert into employees values (543, 'Sherwynd', 'Shelliday', 'sshellidayf2@t-online.de', '2010-09-19', 'Sports', 'M', 164470, 3);
insert into employees values (544, 'Kincaid', 'Bader', 'kbaderf3@themeforest.net', '2010-11-10', 'Security', 'M', 162233, 6);
insert into employees values (545, 'Kathi', 'Kirkby', 'kkirkbyf4@psu.edu', '2009-03-06', 'Phones & Tablets', 'F', 78530, 4);
insert into employees values (546, 'Dorree', 'Lackmann', 'dlackmannf5@zdnet.com', '2011-01-22', 'Clothing', 'F', 61632, 2);
insert into employees values (547, 'Em', 'Bassam', 'ebassamf6@walmart.com', '2009-04-30', 'Garden', 'M', 41339, 3);
insert into employees values (548, 'Camey', 'Bonham', 'cbonhamf7@altervista.org', '2016-04-24', 'Clothing', 'M', 88291, 2);
insert into employees values (549, 'Hyman', 'Espasa', 'hespasaf8@who.int', '2004-05-25', 'Jewelry', 'M', 63399, 3);
insert into employees values (550, 'Elvera', 'Tinline', 'etinlinef9@who.int', '2016-07-17', 'Vitamins', 'F', 163933, 2);
insert into employees values (551, 'Ram', 'Blowes', 'rblowesfa@cocolog-nifty.com', '2007-09-14', 'Movies', 'M', 87479, 4);
insert into employees values (552, 'Betsy', 'Densun', 'bdensunfb@hud.gov', '2006-09-03', 'Movies', 'F', 28882, 6);
insert into employees values (553, 'Ewart', 'Carren', 'ecarrenfc@google.ru', '2004-03-19', 'Movies', 'M', 112238, 3);
insert into employees values (554, 'Gran', 'Dummigan', null, '2015-03-12', 'Games', 'M', 30313, 7);
insert into employees values (555, 'Andra', 'Saile', 'asailefe@indiatimes.com', '2003-06-21', 'Sports', 'F', 150195, 6);
insert into employees values (556, 'Mollie', 'Darco', 'mdarcoff@taobao.com', '2005-01-01', 'Music', 'F', 76273, 7);
insert into employees values (557, 'Octavius', 'Chiommienti', 'ochiommientifg@wikispaces.com', '2007-06-17', 'Furniture', 'M', 31653, 6);
insert into employees values (558, 'Teodor', 'Dubery', null, '2012-08-22', 'Furniture', 'M', 139403, 7);
insert into employees values (559, 'Grady', 'Forder', 'gforderfi@psu.edu', '2007-10-27', 'First Aid', 'M', 119123, 3);
insert into employees values (560, 'Otha', 'Blything', null, '2015-11-27', 'First Aid', 'F', 135108, 7);
insert into employees values (561, 'Renado', 'Bulcock', 'rbulcockfk@mtv.com', '2013-06-27', 'Movies', 'M', 124693, 5);
insert into employees values (562, 'Romona', 'Cuncliffe', 'rcuncliffefl@sitemeter.com', '2013-05-15', 'Games', 'F', 37589, 2);
insert into employees values (563, 'Burl', 'de Merida', null, '2010-04-12', 'Camping', 'M', 73523, 3);
insert into employees values (564, 'Vonny', 'Mallender', 'vmallenderfn@unesco.org', '2009-07-16', 'Furniture', 'F', 55248, 5);
insert into employees values (565, 'Hanna', 'Playden', 'hplaydenfo@businessweek.com', '2006-08-07', 'Garden', 'F', 116456, 2);
insert into employees values (566, 'Stormy', 'Alelsandrovich', 'salelsandrovichfp@t-online.de', '2016-04-10', 'Computers', 'F', 28217, 3);
insert into employees values (567, 'Nefen', 'Roberto', 'nrobertofq@blogspot.com', '2009-05-15', 'Decor', 'M', 86014, 2);
insert into employees values (568, 'Del', 'Baldung', 'dbaldungfr@disqus.com', '2007-12-04', 'Books', 'M', 69681, 3);
insert into employees values (569, 'Selle', 'Harhoff', 'sharhofffs@google.nl', '2008-11-20', 'Maintenance', 'F', 40041, 4);
insert into employees values (570, 'Cy', 'Mence', 'cmenceft@icq.com', '2016-01-18', 'Automotive', 'M', 144146, 7);
insert into employees values (571, 'Reinold', 'Isgate', 'risgatefu@oaic.gov.au', '2015-10-09', 'Tools', 'M', 108110, 1);
insert into employees values (572, 'Mandy', 'Miere', 'mmierefv@rediff.com', '2008-12-03', 'Tools', 'F', 142299, 6);
insert into employees values (573, 'Nan', 'Ellerman', 'nellermanfw@odnoklassniki.ru', '2009-08-06', 'Sports', 'F', 28029, 1);
insert into employees values (574, 'Helena', 'Schultheiss', null, '2015-11-29', 'Grocery', 'F', 102563, 6);
insert into employees values (575, 'Lilli', 'Wrack', null, '2012-05-25', 'Cosmetics', 'F', 136056, 5);
insert into employees values (576, 'Zahara', 'Hindenberger', 'zhindenbergerfz@jiathis.com', '2004-03-04', 'Decor', 'F', 88174, 7);
insert into employees values (577, 'Elbertina', 'Kidder', 'ekidderg0@eepurl.com', '2003-07-22', 'Movies', 'F', 111253, 4);
insert into employees values (578, 'Katlin', 'Bemrose', 'kbemroseg1@webs.com', '2011-05-21', 'Automotive', 'F', 60089, 6);
insert into employees values (579, 'Olly', 'Wheelwright', 'owheelwrightg2@msn.com', '2003-06-11', 'Pharmacy', 'F', 161357, 1);
insert into employees values (580, 'Hugh', 'Jopke', 'hjopkeg3@vinaora.com', '2012-08-30', 'Children Clothing', 'M', 61893, 4);
insert into employees values (581, 'Terry', 'Coning', 'tconingg4@wikimedia.org', '2006-05-21', 'Decor', 'M', 39709, 7);
insert into employees values (582, 'Erhard', 'Tabourin', 'etabouring5@yellowbook.com', '2009-05-20', 'Children Clothing', 'M', 109317, 5);
insert into employees values (583, 'Whitby', 'Oates', 'woatesg6@dion.ne.jp', '2012-01-17', 'Movies', 'M', 147446, 1);
insert into employees values (584, 'Arlina', 'Hartness', null, '2014-11-25', 'Vitamins', 'F', 122516, 7);
insert into employees values (585, 'Clarance', 'Yegoshin', 'cyegoshing8@google.de', '2010-03-17', 'Books', 'M', 88536, 3);
insert into employees values (586, 'Sibyl', 'Crackett', 'scrackettg9@slashdot.org', '2009-10-08', 'Pharmacy', 'M', 155151, 6);
insert into employees values (587, 'Petr', 'Littleton', null, '2011-03-05', 'Grocery', 'M', 89574, 3);
insert into employees values (588, 'Kellen', 'Chisnell', 'kchisnellgb@desdev.cn', '2003-06-21', 'Garden', 'F', 24614, 3);
insert into employees values (589, 'Ly', 'Farquarson', 'lfarquarsongc@4shared.com', '2004-01-30', 'Pharmacy', 'M', 52451, 7);
insert into employees values (590, 'Sandro', 'Gonin', 'sgoningd@bbb.org', '2015-03-20', 'Jewelry', 'M', 29170, 7);
insert into employees values (591, 'Wrennie', 'Bealing', 'wbealingge@icq.com', '2004-03-26', 'Furniture', 'F', 160170, 7);
insert into employees values (592, 'Juan', 'Tuley', 'jtuleygf@sohu.com', '2010-01-22', 'Device Repair', 'M', 136597, 6);
insert into employees values (593, 'Jermain', 'Levane', 'jlevanegg@so-net.ne.jp', '2016-02-17', 'Camping', 'M', 71163, 4);
insert into employees values (594, 'Bordie', 'Kulvear', 'bkulveargh@independent.co.uk', '2007-05-01', 'Garden', 'M', 48468, 7);
insert into employees values (595, 'Francoise', 'Chape', 'fchapegi@hc360.com', '2014-09-19', 'Pharmacy', 'F', 128279, 1);
insert into employees values (596, 'Samara', 'Durdle', null, '2014-05-08', 'Pharmacy', 'F', 71269, 4);
insert into employees values (597, 'Blake', 'Keizman', 'bkeizmangk@sogou.com', '2005-05-12', 'Books', 'M', 104884, 2);
insert into employees values (598, 'Darrin', 'Bellino', 'dbellinogl@springer.com', '2004-01-17', 'Sports', 'M', 142943, 6);
insert into employees values (599, 'Bernadene', 'Fissenden', null, '2015-08-24', 'Games', 'F', 22983, 5);
insert into employees values (600, 'Bethena', 'Trownson', 'btrownsongn@com.com', '2013-01-31', 'Books', 'F', 141202, 3);
insert into employees values (601, 'Sammie', 'McClosh', 'smccloshgo@cisco.com', '2014-06-16', 'First Aid', 'M', 29568, 4);
insert into employees values (602, 'Karna', 'Olek', 'kolekgp@miitbeian.gov.cn', '2005-05-12', 'Jewelry', 'F', 41938, 3);
insert into employees values (603, 'Avram', 'Sever', 'asevergq@lulu.com', '2014-10-13', 'Phones & Tablets', 'M', 59209, 3);
insert into employees values (604, 'Sayers', 'Gherardini', 'sgherardinigr@msn.com', '2013-01-31', 'First Aid', 'M', 111532, 1);
insert into employees values (605, 'Rorke', 'Royden', 'rroydengs@nature.com', '2005-01-19', 'Security', 'M', 89252, 7);
insert into employees values (606, 'Mira', 'Unworth', 'munworthgt@thetimes.co.uk', '2005-06-13', 'Jewelry', 'F', 32948, 2);
insert into employees values (607, 'Maryanna', 'Billin', 'mbillingu@woothemes.com', '2006-01-26', 'Clothing', 'F', 132264, 2);
insert into employees values (608, 'Kaye', 'Spivey', 'kspiveygv@tiny.cc', '2010-06-17', 'Garden', 'F', 77836, 6);
insert into employees values (609, 'Adrianna', 'Pickford', 'apickfordgw@google.ca', '2011-09-14', 'First Aid', 'F', 108411, 2);
insert into employees values (610, 'Darrin', 'Shemelt', null, '2016-08-10', 'Furniture', 'M', 86327, 5);
insert into employees values (611, 'Spense', 'Winckle', 'swincklegy@list-manage.com', '2015-11-17', 'Decor', 'M', 79045, 4);
insert into employees values (612, 'Joete', 'Caesar', 'jcaesargz@wsj.com', '2015-08-01', 'Garden', 'F', 50475, 3);
insert into employees values (613, 'Brandise', 'Jans', 'bjansh0@lulu.com', '2008-02-15', 'Computers', 'F', 163512, 4);
insert into employees values (614, 'Rooney', 'Kempstone', 'rkempstoneh1@livejournal.com', '2011-01-23', 'Pharmacy', 'M', 25835, 6);
insert into employees values (615, 'Manolo', 'Kupec', 'mkupech2@aol.com', '2015-12-16', 'Movies', 'M', 83344, 7);
insert into employees values (616, 'Nadia', 'Alonso', 'nalonsoh3@google.fr', '2016-03-25', 'Vitamins', 'F', 136017, 3);
insert into employees values (617, 'Jacob', 'Phythean', 'jphytheanh4@un.org', '2010-06-12', 'Decor', 'M', 126992, 3);
insert into employees values (618, 'Courtney', 'Geertsen', 'cgeertsenh5@g.co', '2007-11-11', 'Books', 'F', 56692, 5);
insert into employees values (619, 'Rosalia', 'Belton', 'rbeltonh6@kickstarter.com', '2006-09-08', 'Plumbing', 'F', 72546, 4);
insert into employees values (620, 'Lionel', 'Uridge', 'luridgeh7@addtoany.com', '2006-11-15', 'Computers', 'M', 140136, 7);
insert into employees values (621, 'Dore', 'Fairhead', null, '2009-07-22', 'First Aid', 'F', 48122, 2);
insert into employees values (622, 'Husain', 'Crookshanks', 'hcrookshanksh9@ebay.com', '2006-12-10', 'Camping', 'M', 41892, 7);
insert into employees values (623, 'Gran', 'Nelthropp', 'gnelthroppha@netvibes.com', '2005-12-01', 'Vitamins', 'M', 43666, 6);
insert into employees values (624, 'Lucius', 'Stilgoe', null, '2004-04-11', 'Grocery', 'M', 21120, 5);
insert into employees values (625, 'Jamie', 'Burne', 'jburnehc@quantcast.com', '2003-03-13', 'Cosmetics', 'M', 99770, 6);
insert into employees values (626, 'Quentin', 'McPhillimey', 'qmcphillimeyhd@baidu.com', '2009-03-16', 'Garden', 'M', 58423, 7);
insert into employees values (627, 'Gorden', 'Epdell', null, '2007-12-20', 'Decor', 'M', 146577, 1);
insert into employees values (628, 'Amalita', 'Gannicott', 'agannicotthf@furl.net', '2014-11-09', 'Cosmetics', 'F', 147379, 3);
insert into employees values (629, 'Bekki', 'Emmanueli', 'bemmanuelihg@surveymonkey.com', '2011-03-18', 'Cosmetics', 'F', 84573, 3);
insert into employees values (630, 'Deina', 'Feldheim', 'dfeldheimhh@gov.uk', '2007-03-24', 'Beauty', 'F', 101678, 2);
insert into employees values (631, 'Stanislaw', 'Biggerstaff', 'sbiggerstaffhi@com.com', '2003-11-24', 'Toys', 'M', 95290, 2);
insert into employees values (632, 'Myra', 'Vasnev', 'mvasnevhj@who.int', '2015-12-11', 'Books', 'F', 87574, 7);
insert into employees values (633, 'Tyson', 'O''Scanlan', 'toscanlanhk@slashdot.org', '2008-07-03', 'Furniture', 'M', 50439, 5);
insert into employees values (634, 'Roobbie', 'Picknett', null, '2016-07-25', 'Grocery', 'F', 146639, 2);
insert into employees values (635, 'Ardyce', 'Saffon', null, '2007-03-31', 'Games', 'F', 135105, 4);
insert into employees values (636, 'Adam', 'Fenwick', 'afenwickhn@whitehouse.gov', '2015-09-15', 'Sports', 'M', 67057, 3);
insert into employees values (637, 'Valentina', 'Ditchburn', 'vditchburnho@tiny.cc', '2014-01-19', 'Movies', 'F', 104213, 2);
insert into employees values (638, 'Kit', 'Angric', 'kangrichp@angelfire.com', '2014-12-30', 'Phones & Tablets', 'F', 46100, 3);
insert into employees values (639, 'Jorry', 'Carrigan', 'jcarriganhq@constantcontact.com', '2015-04-04', 'Beauty', 'F', 56926, 2);
insert into employees values (640, 'Karlik', 'Shemwell', 'kshemwellhr@tumblr.com', '2007-06-13', 'Tools', 'M', 24777, 2);
insert into employees values (641, 'Jakie', 'Satch', 'jsatchhs@kickstarter.com', '2004-09-27', 'Furniture', 'M', 48668, 7);
insert into employees values (642, 'Agnella', 'Fleming', 'afleminght@xinhuanet.com', '2012-03-08', 'Camping', 'F', 78892, 5);
insert into employees values (643, 'Rodolph', 'Epps', null, '2016-08-24', 'Computers', 'M', 45769, 1);
insert into employees values (644, 'Kerstin', 'Shildrick', null, '2005-10-30', 'Grocery', 'F', 162926, 1);
insert into employees values (645, 'Tracey', 'Buncombe', 'tbuncombehw@yahoo.com', '2005-12-03', 'First Aid', 'F', 96845, 4);
insert into employees values (646, 'Ivory', 'Chitson', null, '2005-08-03', 'Phones & Tablets', 'F', 35112, 3);
insert into employees values (647, 'Berri', 'Bisacre', 'bbisacrehy@cmu.edu', '2003-07-03', 'Children Clothing', 'F', 62083, 4);
insert into employees values (648, 'Abbott', 'Mundow', 'amundowhz@prlog.org', '2003-06-05', 'Automotive', 'M', 106517, 7);
insert into employees values (649, 'Jesselyn', 'McClory', 'jmccloryi0@scribd.com', '2016-06-27', 'Cosmetics', 'F', 92991, 4);
insert into employees values (650, 'Roarke', 'Giggs', 'rgiggsi1@independent.co.uk', '2008-12-03', 'Device Repair', 'M', 21023, 5);
insert into employees values (651, 'Lazarus', 'Wyllcocks', 'lwyllcocksi2@acquirethisname.com', '2005-04-16', 'Camping', 'M', 127132, 1);
insert into employees values (652, 'Phaidra', 'Dunrige', 'pdunrigei3@cam.ac.uk', '2005-04-17', 'Decor', 'F', 51899, 6);
insert into employees values (653, 'Rockey', 'Boddis', 'rboddisi4@skyrock.com', '2012-11-13', 'Games', 'M', 66561, 6);
insert into employees values (654, 'Tann', 'Sapshed', 'tsapshedi5@bloomberg.com', '2004-09-18', 'Cosmetics', 'M', 85403, 3);
insert into employees values (655, 'Darin', 'Pooke', null, '2016-11-18', 'Movies', 'M', 142023, 2);
insert into employees values (656, 'Fowler', 'Buesnel', 'fbuesneli7@yellowpages.com', '2008-03-30', 'Camping', 'M', 44078, 3);
insert into employees values (657, 'Adriena', 'Hugonin', 'ahugonini8@java.com', '2005-08-12', 'Games', 'F', 98103, 1);
insert into employees values (658, 'Danice', 'Greson', 'dgresoni9@state.tx.us', '2009-02-10', 'Garden', 'F', 59085, 5);
insert into employees values (659, 'Carce', 'Greenalf', null, '2009-04-29', 'Children Clothing', 'M', 91026, 7);
insert into employees values (660, 'Rochette', 'Dowse', 'rdowseib@dedecms.com', '2007-11-11', 'Clothing', 'F', 126305, 3);
insert into employees values (661, 'Jamison', 'Hrycek', null, '2014-04-07', 'Garden', 'M', 87682, 1);
insert into employees values (662, 'Verina', 'Furzey', 'vfurzeyid@zdnet.com', '2005-06-03', 'First Aid', 'F', 53924, 1);
insert into employees values (663, 'Shelly', 'Khrishtafovich', 'skhrishtafovichie@youtu.be', '2010-12-23', 'Decor', 'F', 76879, 6);
insert into employees values (664, 'Lukas', 'Gumm', 'lgummif@goo.ne.jp', '2004-11-03', 'Beauty', 'M', 63076, 7);
insert into employees values (665, 'Patty', 'MacPaik', 'pmacpaikig@nydailynews.com', '2003-08-17', 'Grocery', 'F', 159307, 5);
insert into employees values (666, 'Dreddy', 'Lettley', 'dlettleyih@smh.com.au', '2015-10-28', 'Sports', 'F', 38793, 4);
insert into employees values (667, 'Willard', 'Bestwerthick', null, '2015-10-27', 'Music', 'M', 103759, 1);
insert into employees values (668, 'Giralda', 'Melding', 'gmeldingij@stanford.edu', '2014-04-17', 'Children Clothing', 'F', 37206, 1);
insert into employees values (669, 'Lorenzo', 'Gaiter', 'lgaiterik@woothemes.com', '2006-01-16', 'Children Clothing', 'M', 110944, 3);
insert into employees values (670, 'Garrard', 'Baudone', 'gbaudoneil@hexun.com', '2012-06-19', 'Vitamins', 'M', 104859, 7);
insert into employees values (671, 'Gianni', 'Goodship', 'ggoodshipim@miibeian.gov.cn', '2008-11-20', 'Security', 'M', 38963, 6);
insert into employees values (672, 'Jeane', 'Partener', null, '2016-10-09', 'Pharmacy', 'F', 136466, 5);
insert into employees values (673, 'Kerry', 'Tollerfield', 'ktollerfieldio@wordpress.org', '2004-02-20', 'Movies', 'M', 156513, 7);
insert into employees values (674, 'Tabitha', 'Sindle', 'tsindleip@epa.gov', '2014-12-28', 'Movies', 'F', 137125, 3);
insert into employees values (675, 'Becka', 'Oggers', null, '2008-04-10', 'Clothing', 'F', 68190, 6);
insert into employees values (676, 'Ashlin', 'Manneville', 'amannevilleir@blogs.com', '2012-03-14', 'Movies', 'M', 59170, 6);
insert into employees values (677, 'Leilah', 'Rigardeau', 'lrigardeauis@mlb.com', '2012-12-02', 'Camping', 'F', 109202, 5);
insert into employees values (678, 'Rudie', 'Gilling', 'rgillingit@dion.ne.jp', '2012-04-04', 'First Aid', 'M', 40765, 1);
insert into employees values (679, 'Leonidas', 'Orrow', 'lorrowiu@1688.com', '2016-03-02', 'Jewelry', 'M', 71801, 1);
insert into employees values (680, 'Byrom', 'Legen', 'blegeniv@ucoz.com', '2009-11-02', 'Jewelry', 'M', 73439, 1);
insert into employees values (681, 'Tessi', 'Morten', 'tmorteniw@1und1.de', '2014-08-09', 'Computers', 'F', 95386, 5);
insert into employees values (682, 'Giorgio', 'Tryme', 'gtrymeix@unesco.org', '2013-03-06', 'Decor', 'M', 109973, 2);
insert into employees values (683, 'Noelyn', 'De Marchi', 'ndemarchiiy@slashdot.org', '2014-05-28', 'Automotive', 'F', 125305, 4);
insert into employees values (684, 'Carmela', 'Harkins', 'charkinsiz@utexas.edu', '2014-05-16', 'Children Clothing', 'F', 92247, 5);
insert into employees values (685, 'Hogan', 'McKendo', 'hmckendoj0@hatena.ne.jp', '2015-06-26', 'Device Repair', 'M', 42484, 2);
insert into employees values (686, 'Ysabel', 'Jenicke', null, '2011-07-07', 'Beauty', 'F', 87090, 2);
insert into employees values (687, 'Mag', 'Eminson', null, '2011-03-14', 'Beauty', 'F', 74700, 4);
insert into employees values (688, 'Silvain', 'Thoresby', null, '2014-01-24', 'Children Clothing', 'M', 68570, 7);
insert into employees values (689, 'Teena', 'Halgarth', 'thalgarthj4@lulu.com', '2006-04-10', 'Camping', 'F', 89718, 4);
insert into employees values (690, 'Romy', 'Vamplus', 'rvamplusj5@dagondesign.com', '2007-07-14', 'Vitamins', 'F', 152916, 1);
insert into employees values (691, 'Alfy', 'O''Keevan', 'aokeevanj6@tumblr.com', '2010-08-15', 'Vitamins', 'F', 64811, 3);
insert into employees values (692, 'De witt', 'Hess', null, '2006-08-30', 'Beauty', 'M', 74511, 6);
insert into employees values (693, 'Akim', 'Catonne', 'acatonnej8@unesco.org', '2005-12-28', 'Books', 'M', 139254, 7);
insert into employees values (694, 'Tonya', 'Billiard', null, '2010-06-18', 'Books', 'F', 81913, 1);
insert into employees values (695, 'Farlie', 'Caudrey', 'fcaudreyja@wunderground.com', '2003-07-21', 'Device Repair', 'M', 89678, 2);
insert into employees values (696, 'Roma', 'Pfeifer', 'rpfeiferjb@japanpost.jp', '2016-10-02', 'Tools', 'M', 120070, 1);
insert into employees values (697, 'Jasper', 'Nestle', 'jnestlejc@netvibes.com', '2006-10-09', 'Pharmacy', 'M', 27017, 6);
insert into employees values (698, 'Horst', 'Rock', 'hrockjd@techcrunch.com', '2013-05-17', 'Music', 'M', 130342, 6);
insert into employees values (699, 'Nelli', 'Cottam', 'ncottamje@jiathis.com', '2015-09-01', 'First Aid', 'F', 66998, 7);
insert into employees values (700, 'Jewelle', 'Hulstrom', 'jhulstromjf@ovh.net', '2005-06-19', 'Children Clothing', 'F', 140092, 6);
insert into employees values (701, 'Lucilia', 'Toffolini', null, '2003-08-05', 'Furniture', 'F', 86610, 7);
insert into employees values (702, 'Lily', 'Bayly', 'lbaylyjh@timesonline.co.uk', '2008-07-06', 'Garden', 'F', 91483, 1);
insert into employees values (703, 'Darnall', 'Riddlesden', null, '2003-05-23', 'Clothing', 'M', 77589, 6);
insert into employees values (704, 'Lotta', 'Stillgoe', 'lstillgoejj@yolasite.com', '2004-08-09', 'Furniture', 'F', 33652, 1);
insert into employees values (705, 'Tallie', 'Greatrakes', 'tgreatrakesjk@discuz.net', '2006-08-07', 'Security', 'F', 146932, 7);
insert into employees values (706, 'Chloris', 'Dealey', null, '2011-10-28', 'Books', 'F', 41549, 3);
insert into employees values (707, 'Yale', 'Deporte', null, '2006-11-02', 'Camping', 'M', 132097, 4);
insert into employees values (708, 'Abbot', 'Attwill', 'aattwilljn@cbsnews.com', '2010-12-08', 'Movies', 'M', 78935, 3);
insert into employees values (709, 'Gracia', 'Rosendall', 'grosendalljo@blogspot.com', '2008-10-14', 'Tools', 'F', 56159, 7);
insert into employees values (710, 'Charis', 'Bradborne', 'cbradbornejp@scribd.com', '2015-08-14', 'Automotive', 'F', 130995, 3);
insert into employees values (711, 'Merrily', 'Lummis', 'mlummisjq@zdnet.com', '2009-11-27', 'Music', 'F', 77382, 5);
insert into employees values (712, 'Ernesto', 'Locarno', 'elocarnojr@kickstarter.com', '2016-09-26', 'Music', 'M', 57633, 2);
insert into employees values (713, 'Marcos', 'Beames', null, '2014-12-26', 'Cosmetics', 'M', 158321, 2);
insert into employees values (714, 'Tamiko', 'Coale', null, '2012-12-01', 'Phones & Tablets', 'F', 61928, 5);
insert into employees values (715, 'Kippy', 'Jurgenson', 'kjurgensonju@soundcloud.com', '2012-01-26', 'Decor', 'M', 124033, 1);
insert into employees values (716, 'Anders', 'Aronovitz', 'aaronovitzjv@furl.net', '2014-03-26', 'Garden', 'M', 152439, 4);
insert into employees values (717, 'Rayna', 'Auty', 'rautyjw@icq.com', '2011-10-04', 'Children Clothing', 'F', 75188, 3);
insert into employees values (718, 'Trescha', 'Perks', 'tperksjx@storify.com', '2013-03-02', 'Vitamins', 'F', 135611, 3);
insert into employees values (719, 'Margret', 'Dacre', 'mdacrejy@dagondesign.com', '2013-08-28', 'Beauty', 'F', 134595, 4);
insert into employees values (720, 'Kenton', 'Drinkall', null, '2013-01-04', 'Music', 'M', 121621, 1);
insert into employees values (721, 'Albert', 'McClements', 'amcclementsk0@imageshack.us', '2010-12-25', 'Jewelry', 'M', 143432, 4);
insert into employees values (722, 'Alejandro', 'Mickleburgh', 'amickleburghk1@feedburner.com', '2014-02-06', 'Grocery', 'M', 100530, 1);
insert into employees values (723, 'Paddy', 'Wood', 'pwoodk2@wsj.com', '2015-09-10', 'Device Repair', 'M', 99370, 4);
insert into employees values (724, 'Kath', 'Antonijevic', 'kantonijevick3@parallels.com', '2011-10-28', 'Decor', 'F', 151894, 2);
insert into employees values (725, 'Mendie', 'Jouandet', null, '2008-05-14', 'Vitamins', 'M', 141707, 4);
insert into employees values (726, 'Kristoffer', 'Newtown', 'knewtownk5@fema.gov', '2012-04-02', 'Computers', 'M', 44334, 1);
insert into employees values (727, 'Glory', 'Padwick', 'gpadwickk6@pinterest.com', '2016-03-18', 'Books', 'F', 53815, 3);
insert into employees values (728, 'Ludwig', 'Toffalo', 'ltoffalok7@tmall.com', '2014-06-11', 'Clothing', 'M', 36023, 2);
insert into employees values (729, 'Paxon', 'Northidge', 'pnorthidgek8@ftc.gov', '2009-05-01', 'Pharmacy', 'M', 162924, 4);
insert into employees values (730, 'Timothy', 'Andreassen', 'tandreassenk9@cloudflare.com', '2016-08-06', 'Security', 'M', 65680, 6);
insert into employees values (731, 'Iosep', 'Warmisham', null, '2007-03-02', 'Clothing', 'M', 75340, 2);
insert into employees values (732, 'Donny', 'Brecher', 'dbrecherkb@blinklist.com', '2005-05-23', 'Phones & Tablets', 'M', 28857, 4);
insert into employees values (733, 'Issi', 'Reedyhough', 'ireedyhoughkc@nba.com', '2005-07-10', 'Decor', 'F', 86630, 4);
insert into employees values (734, 'Zita', 'Lavis', 'zlaviskd@pbs.org', '2003-11-17', 'Vitamins', 'F', 51503, 3);
insert into employees values (735, 'Merola', 'Matteacci', 'mmatteaccike@liveinternet.ru', '2008-07-15', 'First Aid', 'F', 116875, 6);
insert into employees values (736, 'Byrle', 'Giannasi', null, '2005-03-18', 'First Aid', 'M', 70260, 1);
insert into employees values (737, 'Rudolf', 'Tungate', 'rtungatekg@nih.gov', '2016-06-23', 'Books', 'M', 92068, 7);
insert into employees values (738, 'Casandra', 'Kinlock', 'ckinlockkh@boston.com', '2006-11-06', 'Decor', 'F', 51651, 6);
insert into employees values (739, 'Cecilius', 'Cottey', 'ccotteyki@exblog.jp', '2003-01-20', 'Vitamins', 'M', 98882, 6);
insert into employees values (740, 'Job', 'Dewhurst', 'jdewhurstkj@mapy.cz', '2007-10-13', 'Clothing', 'M', 57843, 6);
insert into employees values (741, 'Wilmar', 'Henzley', 'whenzleykk@cyberchimps.com', '2009-04-09', 'Furniture', 'M', 41951, 7);
insert into employees values (742, 'Gerri', 'Branston', 'gbranstonkl@msn.com', '2013-01-29', 'First Aid', 'M', 54843, 7);
insert into employees values (743, 'Shell', 'Tungate', 'stungatekm@constantcontact.com', '2010-03-28', 'Vitamins', 'M', 47649, 2);
insert into employees values (744, 'Chelsey', 'Vedikhov', 'cvedikhovkn@histats.com', '2003-02-24', 'First Aid', 'F', 57309, 2);
insert into employees values (745, 'Olimpia', 'Peplay', 'opeplayko@microsoft.com', '2014-03-22', 'Plumbing', 'F', 82586, 3);
insert into employees values (746, 'Merv', 'Barrett', 'mbarrettkp@intel.com', '2003-08-02', 'Furniture', 'M', 25602, 1);
insert into employees values (747, 'Nadine', 'Parlett', 'nparlettkq@vkontakte.ru', '2013-04-25', 'Toys', 'F', 141032, 5);
insert into employees values (748, 'Rubetta', 'Skinner', 'rskinnerkr@imdb.com', '2003-06-07', 'Children Clothing', 'F', 104955, 3);
insert into employees values (749, 'Berte', 'Westmerland', 'bwestmerlandks@multiply.com', '2014-01-05', 'Computers', 'F', 125125, 6);
insert into employees values (750, 'Murvyn', 'Lefley', 'mlefleykt@rakuten.co.jp', '2015-05-28', 'Decor', 'M', 59784, 7);
insert into employees values (751, 'Sayres', 'Warrilow', 'swarrilowku@tamu.edu', '2011-09-12', 'Toys', 'M', 108295, 7);
insert into employees values (752, 'Melita', 'Higgonet', 'mhiggonetkv@tripadvisor.com', '2006-09-17', 'Sports', 'F', 136922, 4);
insert into employees values (753, 'Adelaide', 'Gubbin', 'agubbinkw@hc360.com', '2016-12-01', 'Toys', 'F', 27578, 7);
insert into employees values (754, 'Ivie', 'Aubrey', 'iaubreykx@google.es', '2010-04-04', 'Automotive', 'F', 111359, 7);
insert into employees values (755, 'Tate', 'Leaburn', 'tleaburnky@nydailynews.com', '2013-02-10', 'Jewelry', 'M', 48460, 5);
insert into employees values (756, 'Del', 'Eglinton', 'deglintonkz@mozilla.org', '2011-12-30', 'Plumbing', 'M', 145652, 5);
insert into employees values (757, 'Fredrika', 'Cudby', null, '2005-09-26', 'Games', 'F', 97607, 5);
insert into employees values (758, 'Weylin', 'De Caville', 'wdecavillel1@theatlantic.com', '2014-01-21', 'Clothing', 'M', 86194, 5);
insert into employees values (759, 'Jefferson', 'Ridett', 'jridettl2@imdb.com', '2007-05-06', 'Children Clothing', 'M', 75030, 2);
insert into employees values (760, 'Nathalia', 'Norcross', 'nnorcrossl3@nba.com', '2013-06-15', 'Furniture', 'F', 27627, 4);
insert into employees values (761, 'Lindsay', 'Tace', 'ltacel4@tuttocitta.it', '2015-07-16', 'Games', 'M', 86426, 7);
insert into employees values (762, 'Orsa', 'Tourne', 'otournel5@webmd.com', '2005-07-19', 'First Aid', 'F', 163239, 4);
insert into employees values (763, 'Alexander', 'Bodker', 'abodkerl6@drupal.org', '2010-08-01', 'Music', 'M', 151422, 4);
insert into employees values (764, 'Urban', 'Conwell', 'uconwelll7@multiply.com', '2015-02-23', 'Beauty', 'M', 162169, 2);
insert into employees values (765, 'Joseito', 'Baumert', 'jbaumertl8@dot.gov', '2004-09-17', 'First Aid', 'M', 104018, 7);
insert into employees values (766, 'Nonnah', 'Dict', 'ndictl9@about.me', '2003-03-08', 'Music', 'F', 145169, 1);
insert into employees values (767, 'Arri', 'Chetter', null, '2010-02-06', 'Computers', 'M', 122059, 3);
insert into employees values (768, 'Erminia', 'O''Carmody', 'eocarmodylb@independent.co.uk', '2007-01-06', 'Computers', 'F', 146467, 7);
insert into employees values (769, 'Bebe', 'Swede', 'bswedelc@paypal.com', '2005-03-20', 'Jewelry', 'F', 104602, 6);
insert into employees values (770, 'Sibilla', 'Guilder', 'sguilderld@over-blog.com', '2014-07-23', 'Computers', 'F', 116241, 5);
insert into employees values (771, 'Berti', 'Randerson', 'brandersonle@opensource.org', '2016-10-06', 'Children Clothing', 'M', 150740, 3);
insert into employees values (772, 'Stefano', 'Dincey', 'sdinceylf@bing.com', '2007-07-09', 'Cosmetics', 'M', 94751, 7);
insert into employees values (773, 'Stephi', 'Dickin', null, '2005-12-17', 'Jewelry', 'F', 52698, 1);
insert into employees values (774, 'Falkner', 'Townsend', 'ftownsendlh@1688.com', '2011-05-10', 'Camping', 'M', 46793, 1);
insert into employees values (775, 'Maisie', 'Terrill', null, '2005-03-28', 'Camping', 'F', 36445, 1);
insert into employees values (776, 'Fields', 'Balls', 'fballslj@reverbnation.com', '2015-09-02', 'Pharmacy', 'M', 52413, 6);
insert into employees values (777, 'Eilis', 'Mart', null, '2008-01-04', 'Toys', 'F', 136130, 4);
insert into employees values (778, 'Devon', 'Pauly', 'dpaulyll@sitemeter.com', '2005-04-29', 'Camping', 'F', 27049, 2);
insert into employees values (779, 'Yuma', 'Whitlow', 'ywhitlowlm@virginia.edu', '2007-12-02', 'Furniture', 'M', 48357, 2);
insert into employees values (780, 'Emlyn', 'Bittlestone', 'ebittlestoneln@cocolog-nifty.com', '2015-08-18', 'Pharmacy', 'F', 146046, 6);
insert into employees values (781, 'Gilemette', 'Binney', 'gbinneylo@wordpress.com', '2007-05-21', 'First Aid', 'F', 48726, 3);
insert into employees values (782, 'Shaina', 'Twigg', 'stwigglp@bing.com', '2015-08-04', 'Books', 'F', 87994, 3);
insert into employees values (783, 'Chrissy', 'Appleton', 'cappletonlq@census.gov', '2014-02-27', 'Automotive', 'F', 146522, 1);
insert into employees values (784, 'Starlin', 'McConachie', 'smcconachielr@so-net.ne.jp', '2004-09-07', 'Sports', 'F', 38120, 1);
insert into employees values (785, 'Keenan', 'Gerran', 'kgerranls@disqus.com', '2006-08-23', 'Maintenance', 'M', 47734, 3);
insert into employees values (786, 'Billie', 'Alderman', 'baldermanlt@usa.gov', '2003-12-31', 'Plumbing', 'M', 64956, 5);
insert into employees values (787, 'Issi', 'Arran', 'iarranlu@dagondesign.com', '2015-10-07', 'First Aid', 'F', 104520, 7);
insert into employees values (788, 'Dianemarie', 'Grundy', 'dgrundylv@aol.com', '2004-03-19', 'Furniture', 'F', 59887, 3);
insert into employees values (789, 'Ellerey', 'Galsworthy', 'egalsworthylw@fotki.com', '2009-06-16', 'Toys', 'M', 85002, 4);
insert into employees values (790, 'Ellery', 'Le Brum', null, '2006-01-27', 'Movies', 'M', 82882, 6);
insert into employees values (791, 'Barby', 'Daniell', 'bdaniellly@cbc.ca', '2016-12-26', 'Clothing', 'F', 164588, 6);
insert into employees values (792, 'Matty', 'Baldcock', null, '2008-06-11', 'Device Repair', 'M', 76953, 4);
insert into employees values (793, 'Faustine', 'Ivanov', 'fivanovm0@netlog.com', '2009-06-05', 'Clothing', 'F', 157392, 1);
insert into employees values (794, 'Juliann', 'Piser', 'jpiserm1@businessinsider.com', '2016-01-26', 'Device Repair', 'F', 37404, 1);
insert into employees values (795, 'Valry', 'Philcott', 'vphilcottm2@webnode.com', '2014-07-22', 'Furniture', 'F', 109203, 1);
insert into employees values (796, 'Lawton', 'O''Leary', 'lolearym3@cisco.com', '2013-04-06', 'Beauty', 'M', 103570, 6);
insert into employees values (797, 'Glyn', 'Seeborne', 'gseebornem4@ca.gov', '2010-11-29', 'Device Repair', 'F', 61377, 7);
insert into employees values (798, 'Milissent', 'Lockart', null, '2013-07-01', 'Cosmetics', 'F', 65910, 1);
insert into employees values (799, 'Way', 'Kochlin', 'wkochlinm6@meetup.com', '2006-07-15', 'Automotive', 'M', 51989, 6);
insert into employees values (800, 'Zeke', 'Keyworth', 'zkeyworthm7@google.nl', '2009-04-26', 'Toys', 'M', 163688, 2);
insert into employees values (801, 'Darnell', 'Moorey', null, '2006-10-06', 'Games', 'M', 97312, 6);
insert into employees values (802, 'Tatiania', 'Fall', 'tfallm9@un.org', '2015-03-11', 'Cosmetics', 'F', 86820, 4);
insert into employees values (803, 'Edvard', 'Scinelli', 'escinellima@columbia.edu', '2008-02-16', 'Books', 'M', 92019, 1);
insert into employees values (804, 'Annie', 'Denge', 'adengemb@jigsy.com', '2015-02-01', 'Toys', 'F', 149161, 3);
insert into employees values (805, 'Arabel', 'Critchley', 'acritchleymc@oaic.gov.au', '2009-03-03', 'Movies', 'F', 87799, 2);
insert into employees values (806, 'Griz', 'Doxsey', 'gdoxseymd@free.fr', '2013-04-15', 'Jewelry', 'M', 105948, 3);
insert into employees values (807, 'Gav', 'Scampion', null, '2016-06-04', 'Pharmacy', 'M', 71505, 1);
insert into employees values (808, 'Manfred', 'Emlen', 'memlenmf@goo.ne.jp', '2008-03-24', 'Clothing', 'M', 160417, 5);
insert into employees values (809, 'Babara', 'Antoniewicz', 'bantoniewiczmg@nhs.uk', '2007-01-15', 'Tools', 'F', 153102, 1);
insert into employees values (810, 'Caryl', 'Hillitt', null, '2014-11-08', 'Clothing', 'F', 50835, 4);
insert into employees values (811, 'Gustave', 'Fayne', 'gfaynemi@so-net.ne.jp', '2010-09-26', 'Device Repair', 'M', 147926, 7);
insert into employees values (812, 'Ileane', 'Santos', null, '2007-04-26', 'Device Repair', 'F', 49071, 3);
insert into employees values (813, 'Lauren', 'Bertenshaw', 'lbertenshawmk@webnode.com', '2006-04-13', 'Pharmacy', 'F', 166016, 7);
insert into employees values (814, 'Dorothea', 'Addicott', 'daddicottml@theguardian.com', '2003-02-27', 'Grocery', 'F', 46062, 7);
insert into employees values (815, 'Celisse', 'Simcoe', 'csimcoemm@eventbrite.com', '2013-03-08', 'Toys', 'F', 71923, 7);
insert into employees values (816, 'Gianina', 'Creus', 'gcreusmn@vkontakte.ru', '2013-01-20', 'Clothing', 'F', 48107, 7);
insert into employees values (817, 'Kinnie', 'Domenc', 'kdomencmo@gmpg.org', '2015-07-08', 'Computers', 'M', 30231, 1);
insert into employees values (818, 'Larry', 'Donn', 'ldonnmp@xing.com', '2013-03-08', 'Children Clothing', 'M', 56245, 5);
insert into employees values (819, 'Elisabetta', 'Sheppard', null, '2008-07-31', 'Computers', 'F', 105522, 4);
insert into employees values (820, 'Courtnay', 'Disbury', 'cdisburymr@bbb.org', '2016-07-25', 'Games', 'F', 115928, 4);
insert into employees values (821, 'Lyndy', 'Satterley', 'lsatterleyms@ucsd.edu', '2005-06-20', 'Vitamins', 'F', 103572, 4);
insert into employees values (822, 'Ashia', 'Stoves', null, '2004-10-27', 'Vitamins', 'F', 22190, 5);
insert into employees values (823, 'Pall', 'Dumingo', 'pdumingomu@desdev.cn', '2014-11-09', 'Grocery', 'M', 65452, 5);
insert into employees values (824, 'Barbee', 'Westraw', 'bwestrawmv@google.co.jp', '2008-07-03', 'First Aid', 'F', 58392, 3);
insert into employees values (825, 'Danice', 'Faulkes', 'dfaulkesmw@netvibes.com', '2012-03-17', 'Camping', 'F', 112997, 6);
insert into employees values (826, 'Akim', 'Dorro', 'adorromx@baidu.com', '2013-12-12', 'First Aid', 'M', 111325, 6);
insert into employees values (827, 'Claudine', 'Dyble', 'cdyblemy@vimeo.com', '2005-05-20', 'Children Clothing', 'F', 134442, 3);
insert into employees values (828, 'Evey', 'Gilloran', 'egilloranmz@time.com', '2010-04-17', 'Beauty', 'F', 71278, 3);
insert into employees values (829, 'Aloysius', 'Izkovici', 'aizkovicin0@pagesperso-orange.fr', '2013-06-28', 'Books', 'M', 120775, 5);
insert into employees values (830, 'Gillie', 'Shenfisch', 'gshenfischn1@vimeo.com', '2009-02-16', 'Device Repair', 'F', 104223, 4);
insert into employees values (831, 'Aguie', 'Epsly', 'aepslyn2@xing.com', '2014-03-08', 'Beauty', 'M', 144955, 3);
insert into employees values (832, 'Monique', 'Ivanovic', 'mivanovicn3@desdev.cn', '2016-06-13', 'Sports', 'F', 150061, 1);
insert into employees values (833, 'Tailor', 'Solesbury', 'tsolesburyn4@bloomberg.com', '2013-09-19', 'Grocery', 'M', 48200, 6);
insert into employees values (834, 'Gerick', 'Paulus', null, '2015-08-08', 'Furniture', 'M', 158121, 5);
insert into employees values (835, 'Ibby', 'McElwee', null, '2013-03-13', 'Games', 'F', 132891, 6);
insert into employees values (836, 'Poppy', 'Lines', 'plinesn7@gmpg.org', '2010-07-27', 'Automotive', 'F', 144511, 2);
insert into employees values (837, 'Ralph', 'Busch', null, '2012-06-10', 'First Aid', 'M', 92954, 2);
insert into employees values (838, 'Dasi', 'Ramey', 'drameyn9@bbc.co.uk', '2015-10-17', 'Furniture', 'F', 51075, 1);
insert into employees values (839, 'Almeria', 'McGrane', 'amcgranena@cargocollective.com', '2008-08-18', 'Pharmacy', 'F', 63772, 3);
insert into employees values (840, 'Archibold', 'Deely', 'adeelynb@fda.gov', '2003-04-26', 'Automotive', 'M', 69379, 2);
insert into employees values (841, 'Cassie', 'Dahle', 'cdahlenc@upenn.edu', '2009-05-10', 'Computers', 'M', 134404, 6);
insert into employees values (842, 'William', 'Bletcher', 'wbletchernd@washington.edu', '2011-03-09', 'Vitamins', 'M', 95453, 3);
insert into employees values (843, 'Berkley', 'Clows', null, '2007-06-11', 'Automotive', 'M', 44641, 5);
insert into employees values (844, 'Laurie', 'Infantino', 'linfantinonf@china.com.cn', '2007-05-31', 'Automotive', 'M', 29752, 4);
insert into employees values (845, 'Caty', 'Toy', 'ctoyng@kickstarter.com', '2012-07-24', 'Movies', 'F', 78267, 4);
insert into employees values (846, 'Stanley', 'Brecknell', null, '2009-11-17', 'Sports', 'M', 151814, 4);
insert into employees values (847, 'Gweneth', 'MacCrann', null, '2014-09-12', 'Sports', 'F', 29047, 7);
insert into employees values (848, 'Emmalynn', 'Wilkin', null, '2008-11-21', 'Computers', 'F', 43190, 4);
insert into employees values (849, 'Cobbie', 'Leiden', 'cleidennk@archive.org', '2005-09-04', 'Movies', 'M', 155158, 1);
insert into employees values (850, 'Mychal', 'Mucklow', 'mmucklownl@oakley.com', '2006-07-13', 'Device Repair', 'M', 45608, 7);
insert into employees values (851, 'Bartel', 'Phythien', 'bphythiennm@a8.net', '2015-05-25', 'Computers', 'M', 154818, 2);
insert into employees values (852, 'Fina', 'Fox', 'ffoxnn@phoca.cz', '2009-07-18', 'Clothing', 'F', 116966, 5);
insert into employees values (853, 'Dicky', 'Coalbran', 'dcoalbranno@statcounter.com', '2012-12-07', 'Games', 'M', 91814, 6);
insert into employees values (854, 'Rudolph', 'Mellanby', null, '2011-07-16', 'Jewelry', 'M', 48783, 4);
insert into employees values (855, 'Suzie', 'Meadowcraft', 'smeadowcraftnq@pcworld.com', '2004-08-29', 'Vitamins', 'F', 36127, 4);
insert into employees values (856, 'Stefa', 'Gorger', null, '2008-08-26', 'Games', 'F', 104211, 5);
insert into employees values (857, 'Laryssa', 'Mum', 'lmumns@shinystat.com', '2006-12-02', 'Computers', 'F', 152831, 2);
insert into employees values (858, 'Hali', 'Sloey', null, '2013-06-11', 'Children Clothing', 'F', 47551, 2);
insert into employees values (859, 'Caralie', 'Mulderrig', null, '2010-03-19', 'Furniture', 'F', 155980, 7);
insert into employees values (860, 'Horatia', 'Andover', 'handovernv@ifeng.com', '2007-04-03', 'First Aid', 'F', 30924, 2);
insert into employees values (861, 'Earle', 'Caveney', 'ecaveneynw@ucoz.com', '2014-12-04', 'Vitamins', 'M', 53808, 3);
insert into employees values (862, 'Jada', 'O'' Sullivan', 'josullivannx@admin.ch', '2007-02-24', 'Cosmetics', 'F', 121165, 5);
insert into employees values (863, 'Jonathan', 'Hegden', 'jhegdenny@theguardian.com', '2015-06-25', 'Furniture', 'M', 121524, 1);
insert into employees values (864, 'Xever', 'Bagott', 'xbagottnz@soundcloud.com', '2012-11-21', 'Vitamins', 'M', 145879, 4);
insert into employees values (865, 'My', 'Pedlingham', null, '2015-10-22', 'Tools', 'M', 87955, 7);
insert into employees values (866, 'Kyrstin', 'Kloser', null, '2010-01-05', 'Tools', 'F', 126942, 2);
insert into employees values (867, 'Cristen', 'Laying', 'clayingo2@scribd.com', '2005-02-28', 'Garden', 'F', 158227, 1);
insert into employees values (868, 'Trevar', 'Hagley', null, '2014-01-09', 'Children Clothing', 'M', 48116, 4);
insert into employees values (869, 'Shawna', 'Huyghe', 'shuygheo4@mit.edu', '2005-11-29', 'Music', 'F', 66651, 3);
insert into employees values (870, 'Dorene', 'Dudman', 'ddudmano5@comsenz.com', '2003-04-23', 'Decor', 'F', 97700, 4);
insert into employees values (871, 'Brier', 'Frill', 'bfrillo6@twitpic.com', '2004-07-03', 'Movies', 'F', 48719, 5);
insert into employees values (872, 'Laverne', 'Seson', 'lsesono7@pinterest.com', '2014-05-23', 'Device Repair', 'F', 63744, 3);
insert into employees values (873, 'Gilda', 'Cromarty', 'gcromartyo8@cbsnews.com', '2004-11-16', 'Vitamins', 'F', 133010, 6);
insert into employees values (874, 'Byron', 'Rummins', null, '2003-06-02', 'Books', 'M', 54434, 1);
insert into employees values (875, 'Eldredge', 'Trickey', 'etrickeyoa@tumblr.com', '2006-04-30', 'Beauty', 'M', 60077, 1);
insert into employees values (876, 'Marlowe', 'Crock', null, '2016-12-01', 'Jewelry', 'M', 66384, 1);
insert into employees values (877, 'Claudell', 'Bagnold', 'cbagnoldoc@harvard.edu', '2007-08-03', 'Movies', 'M', 28141, 6);
insert into employees values (878, 'Shelton', 'Jaye', 'sjayeod@cafepress.com', '2016-08-22', 'Decor', 'M', 139827, 7);
insert into employees values (879, 'Reg', 'Newland', 'rnewlandoe@163.com', '2016-10-28', 'Beauty', 'M', 36053, 3);
insert into employees values (880, 'Lion', 'Hindenberger', null, '2013-08-15', 'Vitamins', 'M', 104269, 3);
insert into employees values (881, 'Stefania', 'Baltrushaitis', null, '2007-06-08', 'Movies', 'F', 143381, 6);
insert into employees values (882, 'Evin', 'Patton', null, '2010-09-23', 'Vitamins', 'M', 59706, 6);
insert into employees values (883, 'Valentine', 'Gawthorp', null, '2012-10-22', 'Phones & Tablets', 'M', 128131, 5);
insert into employees values (884, 'Gordan', 'Skones', 'gskonesoj@mac.com', '2009-04-29', 'Games', 'M', 40268, 3);
insert into employees values (885, 'Corabella', 'Howels', 'chowelsok@xrea.com', '2012-08-25', 'Furniture', 'F', 114708, 1);
insert into employees values (886, 'Mortimer', 'Feldstein', null, '2016-07-19', 'Clothing', 'M', 88534, 5);
insert into employees values (887, 'Philippine', 'Greenig', 'pgreenigom@nbcnews.com', '2011-04-16', 'Books', 'F', 99888, 6);
insert into employees values (888, 'Rouvin', 'Baudet', null, '2010-05-17', 'Tools', 'M', 97934, 1);
insert into employees values (889, 'Blake', 'Paal', 'bpaaloo@japanpost.jp', '2004-05-11', 'Furniture', 'M', 88002, 3);
insert into employees values (890, 'Ursuline', 'Crowhurst', 'ucrowhurstop@rambler.ru', '2009-09-26', 'First Aid', 'F', 33488, 4);
insert into employees values (891, 'Aylmar', 'Leipelt', 'aleipeltoq@people.com.cn', '2005-07-25', 'Garden', 'M', 157833, 7);
insert into employees values (892, 'Estevan', 'Harpham', 'eharphamor@cbslocal.com', '2016-07-08', 'First Aid', 'M', 59475, 7);
insert into employees values (893, 'Teodora', 'Ryall', 'tryallos@nymag.com', '2008-11-05', 'Computers', 'F', 86453, 2);
insert into employees values (894, 'Lebbie', 'Slaymaker', null, '2016-10-07', 'Grocery', 'F', 57389, 4);
insert into employees values (895, 'Celinka', 'Jenkerson', 'cjenkersonou@zdnet.com', '2009-10-23', 'Furniture', 'F', 156205, 2);
insert into employees values (896, 'Billie', 'Hould', 'bhouldov@mtv.com', '2008-08-09', 'Cosmetics', 'M', 48551, 4);
insert into employees values (897, 'Christophorus', 'Goodbarne', 'cgoodbarneow@ed.gov', '2009-09-30', 'Device Repair', 'M', 115407, 2);
insert into employees values (898, 'Yanaton', 'Lilliman', null, '2007-04-09', 'Phones & Tablets', 'M', 153406, 2);
insert into employees values (899, 'Alverta', 'Youtead', 'ayouteadoy@oaic.gov.au', '2012-07-01', 'Toys', 'F', 127015, 7);
insert into employees values (900, 'Bianca', 'Blitzer', 'bblitzeroz@noaa.gov', '2014-05-29', 'Cosmetics', 'F', 115026, 2);
insert into employees values (901, 'Nolan', 'Tatum', null, '2006-12-24', 'First Aid', 'M', 129501, 3);
insert into employees values (902, 'Sheila-kathryn', 'Fevers', 'sfeversp1@theguardian.com', '2007-01-25', 'Computers', 'F', 75794, 7);
insert into employees values (903, 'Kelby', 'Nudde', null, '2013-02-17', 'Tools', 'M', 156672, 2);
insert into employees values (904, 'Lindsey', 'Cawte', 'lcawtep3@ed.gov', '2015-11-29', 'Grocery', 'F', 52721, 6);
insert into employees values (905, 'Lissy', 'Bodicam', 'lbodicamp4@skyrock.com', '2004-01-15', 'Camping', 'F', 56205, 6);
insert into employees values (906, 'Lydon', 'Dorant', 'ldorantp5@eepurl.com', '2013-06-13', 'Tools', 'M', 66261, 1);
insert into employees values (907, 'Benji', 'Matuszinski', 'bmatuszinskip6@acquirethisname.com', '2016-07-19', 'First Aid', 'M', 93822, 4);
insert into employees values (908, 'Georgeanne', 'Chazotte', 'gchazottep7@linkedin.com', '2004-08-11', 'Cosmetics', 'F', 132783, 6);
insert into employees values (909, 'Leonore', 'Bowness', 'lbownessp8@techcrunch.com', '2010-12-29', 'First Aid', 'F', 43161, 1);
insert into employees values (910, 'Bathsheba', 'Kermode', 'bkermodep9@goo.ne.jp', '2011-07-11', 'Camping', 'F', 157390, 4);
insert into employees values (911, 'Terry', 'Cosans', null, '2012-04-20', 'Beauty', 'M', 119848, 2);
insert into employees values (912, 'Ardelia', 'Dunkley', 'adunkleypb@toplist.cz', '2015-10-18', 'Toys', 'F', 99819, 7);
insert into employees values (913, 'Estrella', 'Anselmi', null, '2014-10-14', 'Books', 'F', 83064, 7);
insert into employees values (914, 'Iver', 'Davidowich', null, '2004-12-30', 'Computers', 'M', 21626, 3);
insert into employees values (915, 'Krystalle', 'Govern', 'kgovernpe@typepad.com', '2007-04-10', 'Decor', 'F', 32768, 3);
insert into employees values (916, 'Odessa', 'Simester', 'osimesterpf@nationalgeographic.com', '2009-08-06', 'Vitamins', 'F', 123268, 7);
insert into employees values (917, 'Darius', 'Viel', 'dvielpg@intel.com', '2003-06-19', 'Camping', 'M', 155579, 6);
insert into employees values (918, 'Lanie', 'Zamora', 'lzamoraph@unicef.org', '2012-12-23', 'First Aid', 'M', 151539, 4);
insert into employees values (919, 'Carissa', 'Gabbitus', 'cgabbituspi@ezinearticles.com', '2016-09-25', 'Music', 'F', 166765, 2);
insert into employees values (920, 'Donni', 'Cuchey', 'dcucheypj@netvibes.com', '2009-10-14', 'First Aid', 'F', 160416, 2);
insert into employees values (921, 'Rancell', 'Cockitt', null, '2013-07-07', 'Movies', 'M', 30411, 6);
insert into employees values (922, 'Carr', 'Cosgry', 'ccosgrypl@behance.net', '2016-04-30', 'Garden', 'M', 68410, 3);
insert into employees values (923, 'Berkley', 'Greenslade', 'bgreensladepm@linkedin.com', '2004-07-27', 'Toys', 'M', 91990, 4);
insert into employees values (924, 'Lynn', 'Housen', 'lhousenpn@dot.gov', '2015-09-03', 'Sports', 'F', 46529, 5);
insert into employees values (925, 'Alvin', 'McMullen', 'amcmullenpo@icio.us', '2016-11-01', 'Beauty', 'M', 69999, 3);
insert into employees values (926, 'Orbadiah', 'Krochmann', 'okrochmannpp@e-recht24.de', '2008-12-03', 'Tools', 'M', 90020, 1);
insert into employees values (927, 'Maryellen', 'Westnedge', 'mwestnedgepq@guardian.co.uk', '2003-04-19', 'Automotive', 'F', 115973, 5);
insert into employees values (928, 'Kaleb', 'Arnefield', 'karnefieldpr@cisco.com', '2004-07-04', 'Maintenance', 'M', 149076, 3);
insert into employees values (929, 'Pennie', 'Prevett', 'pprevettps@ocn.ne.jp', '2009-10-03', 'Computers', 'M', 153445, 1);
insert into employees values (930, 'Tab', 'Tatterton', 'ttattertonpt@scribd.com', '2014-07-16', 'Vitamins', 'M', 141816, 5);
insert into employees values (931, 'Tanner', 'Welbeck', null, '2006-03-02', 'Toys', 'M', 38903, 6);
insert into employees values (932, 'Gabriella', 'Hadkins', null, '2004-10-01', 'Toys', 'F', 65050, 7);
insert into employees values (933, 'Sylvester', 'Janecki', 'sjaneckipw@prweb.com', '2006-05-12', 'Tools', 'M', 98315, 3);
insert into employees values (934, 'Lenka', 'Larose', 'llarosepx@sfgate.com', '2013-02-07', 'Decor', 'F', 21024, 1);
insert into employees values (935, 'Lyman', 'Sackler', 'lsacklerpy@tamu.edu', '2016-08-10', 'Pharmacy', 'M', 160215, 6);
insert into employees values (936, 'Leland', 'Reichartz', 'lreichartzpz@webeden.co.uk', '2005-06-04', 'First Aid', 'F', 131935, 2);
insert into employees values (937, 'Charlie', 'Yakubovics', 'cyakubovicsq0@51.la', '2007-07-23', 'Toys', 'M', 60560, 4);
insert into employees values (938, 'Benjamen', 'Discombe', 'bdiscombeq1@youtube.com', '2015-01-17', 'Pharmacy', 'M', 159011, 3);
insert into employees values (939, 'Dexter', 'McDermid', 'dmcdermidq2@addthis.com', '2006-02-24', 'Jewelry', 'M', 80657, 4);
insert into employees values (940, 'Linus', 'Lowrance', 'llowranceq3@booking.com', '2005-03-04', 'Maintenance', 'M', 46216, 2);
insert into employees values (941, 'Lynn', 'Scriviner', 'lscrivinerq4@ifeng.com', '2003-06-23', 'Toys', 'M', 139330, 1);
insert into employees values (942, 'Alis', 'Senecaux', 'asenecauxq5@unicef.org', '2003-04-09', 'Books', 'F', 148531, 6);
insert into employees values (943, 'Maurise', 'Dally', 'mdallyq6@1und1.de', '2005-03-28', 'Phones & Tablets', 'F', 75393, 1);
insert into employees values (944, 'Fee', 'Shama', 'fshamaq7@si.edu', '2005-06-05', 'Vitamins', 'M', 80502, 2);
insert into employees values (945, 'Kayle', 'Nucciotti', 'knucciottiq8@t-online.de', '2010-08-04', 'Movies', 'F', 33881, 1);
insert into employees values (946, 'Georgianne', 'Chill', null, '2003-12-25', 'Grocery', 'F', 153826, 5);
insert into employees values (947, 'Jabez', 'Ghidini', null, '2004-03-14', 'Decor', 'M', 153849, 3);
insert into employees values (948, 'Cary', 'Lark', 'clarkqb@blogs.com', '2012-03-01', 'First Aid', 'M', 134559, 1);
insert into employees values (949, 'Gabriello', 'Inde', 'gindeqc@zdnet.com', '2012-12-26', 'Garden', 'M', 44474, 3);
insert into employees values (950, 'Cory', 'Rapelli', 'crapelliqd@umich.edu', '2015-11-19', 'Garden', 'M', 77595, 7);
insert into employees values (951, 'Merlina', 'McCullagh', null, '2009-02-16', 'Automotive', 'F', 137094, 1);
insert into employees values (952, 'Bartlett', 'Brunner', null, '2010-03-03', 'Children Clothing', 'M', 130748, 7);
insert into employees values (953, 'Edgard', 'Pead', 'epeadqg@huffingtonpost.com', '2007-07-22', 'Jewelry', 'M', 62116, 6);
insert into employees values (954, 'Jonas', 'Winslett', 'jwinslettqh@newyorker.com', '2014-05-07', 'Device Repair', 'M', 62382, 7);
insert into employees values (955, 'Rodrique', 'Fowlston', 'rfowlstonqi@diigo.com', '2016-01-04', 'Children Clothing', 'M', 95051, 7);
insert into employees values (956, 'Afton', 'Fairweather', 'afairweatherqj@china.com.cn', '2005-06-24', 'Books', 'F', 68716, 1);
insert into employees values (957, 'Sephira', 'Jarville', 'sjarvilleqk@51.la', '2003-09-20', 'Books', 'F', 159561, 6);
insert into employees values (958, 'Eudora', 'Hanalan', 'ehanalanql@illinois.edu', '2016-08-18', 'Clothing', 'F', 31792, 1);
insert into employees values (959, 'Yancy', 'Rickson', null, '2016-05-16', 'Camping', 'M', 60348, 3);
insert into employees values (960, 'Carlyle', 'Josipovitz', 'cjosipovitzqn@npr.org', '2010-06-29', 'Beauty', 'M', 141315, 2);
insert into employees values (961, 'Jobi', 'Helsdon', 'jhelsdonqo@oaic.gov.au', '2006-05-03', 'Maintenance', 'F', 80331, 7);
insert into employees values (962, 'Wash', 'Huntingford', 'whuntingfordqp@purevolume.com', '2004-10-17', 'Pharmacy', 'M', 158546, 5);
insert into employees values (963, 'Erich', 'Gilford', null, '2012-12-29', 'Books', 'M', 106021, 3);
insert into employees values (964, 'Sofia', 'Clements', 'sclementsqr@webnode.com', '2008-05-20', 'Maintenance', 'F', 154140, 2);
insert into employees values (965, 'Berthe', 'Buller', 'bbullerqs@a8.net', '2008-09-27', 'Furniture', 'F', 156041, 6);
insert into employees values (966, 'Candra', 'Vannet', null, '2008-01-01', 'Computers', 'F', 97259, 2);
insert into employees values (967, 'Fiona', 'Dellatorre', 'fdellatorrequ@soundcloud.com', '2007-02-06', 'Phones & Tablets', 'F', 149004, 1);
insert into employees values (968, 'Juliane', 'Shotbolt', 'jshotboltqv@telegraph.co.uk', '2013-01-25', 'Decor', 'F', 34277, 6);
insert into employees values (969, 'Flss', 'Husbands', null, '2005-09-04', 'Device Repair', 'F', 97891, 3);
insert into employees values (970, 'Barrett', 'Barling', 'bbarlingqx@jugem.jp', '2005-10-26', 'Grocery', 'M', 128512, 4);
insert into employees values (971, 'Noellyn', 'Enterlein', null, '2006-12-23', 'Camping', 'F', 86895, 5);
insert into employees values (972, 'Cirstoforo', 'Mulloch', 'cmullochqz@flickr.com', '2011-05-09', 'Clothing', 'M', 141256, 7);
insert into employees values (973, 'Dona', 'Murley', null, '2016-11-09', 'Decor', 'F', 98159, 1);
insert into employees values (974, 'Thorpe', 'Bick', 'tbickr1@businessinsider.com', '2008-01-19', 'Garden', 'M', 121211, 1);
insert into employees values (975, 'Isis', 'McKinn', 'imckinnr2@tinyurl.com', '2010-06-18', 'Movies', 'F', 124444, 4);
insert into employees values (976, 'Lydon', 'Passo', 'lpassor3@disqus.com', '2003-10-17', 'Books', 'M', 48145, 3);
insert into employees values (977, 'Vickie', 'Pryn', null, '2012-02-24', 'Movies', 'F', 33269, 4);
insert into employees values (978, 'Shem', 'Jewes', 'sjewesr5@sciencedaily.com', '2008-10-22', 'Tools', 'M', 121211, 5);
insert into employees values (979, 'Delila', 'Ambrogi', 'dambrogir6@diigo.com', '2007-06-30', 'Sports', 'F', 27064, 6);
insert into employees values (980, 'Lyndy', 'Tooker', 'ltookerr7@topsy.com', '2007-01-26', 'Computers', 'F', 112796, 4);
insert into employees values (981, 'Thorvald', 'Boncoeur', 'tboncoeurr8@ucla.edu', '2005-12-17', 'Music', 'M', 34565, 6);
insert into employees values (982, 'Enid', 'Wooff', 'ewooffr9@wikipedia.org', '2014-05-17', 'Maintenance', 'F', 54434, 5);
insert into employees values (983, 'Henrik', 'Clayborn', 'hclaybornra@hexun.com', '2014-08-04', 'Device Repair', 'M', 117791, 5);
insert into employees values (984, 'Krista', 'Barnewell', 'kbarnewellrb@guardian.co.uk', '2016-02-29', 'Music', 'F', 85666, 5);
insert into employees values (985, 'Nelli', 'Glading', 'ngladingrc@lycos.com', '2010-07-11', 'Grocery', 'F', 52846, 5);
insert into employees values (986, 'Sheila', 'Matthiae', 'smatthiaerd@fotki.com', '2010-03-26', 'Computers', 'F', 23878, 1);
insert into employees values (987, 'Granny', 'Barhem', null, '2003-05-13', 'Movies', 'M', 125798, 1);
insert into employees values (988, 'Tabb', 'Huddleston', 'thuddlestonrf@yahoo.co.jp', '2003-05-02', 'Automotive', 'M', 47591, 6);
insert into employees values (989, 'Ari', 'Queripel', 'aqueripelrg@npr.org', '2013-08-30', 'Phones & Tablets', 'M', 80695, 1);
insert into employees values (990, 'Cristiano', 'Haney`', 'chaneyrh@berkeley.edu', '2014-07-18', 'First Aid', 'M', 105648, 2);
insert into employees values (991, 'Marquita', 'Seawell', 'mseawellri@technorati.com', '2014-09-07', 'Sports', 'F', 38909, 4);
insert into employees values (992, 'Katharine', 'Brussels', 'kbrusselsrj@cnet.com', '2003-10-02', 'Phones & Tablets', 'F', 29806, 5);
insert into employees values (993, 'Frank', 'Garnson', 'fgarnsonrk@bloglovin.com', '2013-12-26', 'Children Clothing', 'M', 95828, 7);
insert into employees values (994, 'Aurlie', 'Kindleysides', null, '2004-05-20', 'Device Repair', 'F', 104822, 3);
insert into employees values (995, 'Reese', 'Watkin', 'rwatkinrm@typepad.com', '2014-10-21', 'Toys', 'M', 102169, 3);
insert into employees values (996, 'Gardiner', 'Aron', 'garonrn@java.com', '2015-11-29', 'Garden', 'M', 111859, 1);
insert into employees values (997, 'Rhianna', 'Trynor', 'rtrynorro@uiuc.edu', '2005-04-07', 'Beauty', 'F', 120753, 7);
insert into employees values (998, 'Brandice', 'Gillicuddy', 'bgillicuddyrp@adobe.com', '2014-11-30', 'Phones & Tablets', 'F', 134058, 2);
insert into employees values (999, 'Kingston', 'Piwall', 'kpiwallrq@nyu.edu', '2012-07-07', 'Music', 'M', 45679, 7);
insert into employees values (1000, 'Jacquelin', 'Cassam', 'jcassamrr@cam.ac.uk', '2010-01-27', 'Music', 'F', 28726, 2);
```
### SQL Managing Tables Using SQL Queries ✨.
- Data Exploration
- Data Cleaning
- SQL Functions
- VIEWS, Joins, Unions

```sql
------Show only Those Department employees count is more than 38------

SELECT department, COUNT(*) FROM employees AS e1
WHERE 38 < (SELECT COUNT(*) FROM employees AS e2 WHERE e1.department = e2.department)
GROUP BY department
------Below query show Same result as above query------

SELECT department, (SELECT COUNT(*) FROM employees AS e2 WHERE e1.department = e2.department)
FROM employees AS e1
GROUP BY department
HAVING COUNT(*) > 38;

---------------Max paid Employees of each Department------------------

SELECT department, (SELECT MAX(salary) FROM employees AS e2 WHERE department = d.department) AS max_paid_employee
FROM departments AS d
WHERE 38 < (SELECT COUNT(*) FROM employees AS e2 WHERE d.department = e2.department)

------Show highest and lowest paid employee first_name, salary, department, custom column show text High salary and Low salary------

SELECT department, first_name, salary,
CASE WHEN salary = max_sal THEN 'HIGHEST SALARY'
WHEN salary = min_sal THEN  'LOWEST SALARY'	END AS salary_in_department
FROM( SELECT department, first_name, salary,
(SELECT MAX(salary) FROM employees e2 WHERE e1.department=e2.department) AS max_sal,
(SELECT MIN(salary) FROM employees e2 WHERE e1.department=e2.department) AS min_sal
FROM employees e1 ) AS subq
WHERE salary = max_sal OR salary = min_sal
ORDER BY department;

------------------Show Department and there employees COUNT------------------

SELECT department, COUNT(*) FROM employees
GROUP BY department
UNION ALL
SELECT 'TOTAL', COUNT(*)  FROM employees;

-----------------------------------------
------------------VIEWS------------------
-----------------------------------------

CREATE VIEW v_employees_information AS
SELECT first_name, email, e.department, salary, division, region, country
FROM employees e, departments d, regions r
WHERE e.department = d.department AND e.region_id = r.region_id;
------------To look for VIEW table use.------------
SELECT * FROM v_employees_information;

-----------------------------------------
------------------JOINS------------------
-----------------------------------------
SELECT first_name, country FROM employees, regions WHERE employees.region_id = regions.region_id;
INNER JOIN  Syntax.		
SELECT first_name, country FROM employees INNER JOIN regions
ON employees.region_id = regions.region_id;
-----------------------------------------
SELECT first_name, email, e.department, division, country FROM employees e, departments d, regions r
WHERE e.department = d.department AND e.region_id = r.region_id AND email IS NOT NULL;
INNER JOIN syntax.
SELECT first_name, email, employees.department, division, country FROM employees INNER JOIN regions
ON employees.region_id = regions.region_id
INNER JOIN departments ON employees.department = departments.department
WHERE email IS NOT NULL;
-----------------------------------------
SELECT country, COUNT(*) FROM regions r, employees e WHERE r.region_id = e.region_id
GROUP BY country
INNER JOIN syntax.
SELECT country, COUNT(employee_id)
FROM employees e INNER JOIN regions r ON e.region_id = r.region_id
GROUP BY country;

-----------------Show Only those department in table 1 that is not exist in table 2------------------------
SELECT distinct e.department FROM employees e LEFT JOIN departments d 
ON e.department = d.department WHERE d.department IS NULL;

------------------Show the First and the Last person Hire_date-----------------------
(SELECT first_name, department, hire_date, country
FROM employees e INNER JOIN regions r ON e.region_id = r.region_id
WHERE hire_date = (SELECT MIN(hire_date) FROM employees)
LIMIT 1)
UNION
SELECT first_name, department, hire_date, country
FROM employees e INNER JOIN regions r ON e.region_id = r.region_id
WHERE hire_date = (SELECT MAX(hire_date) FROM employees)
ORDER BY hire_date;

-------------------Show Company Spending Pattern----------------------
SELECT hire_date, salary,
( SELECT SUM(salary) FROM employees e2 
WHERE e2.hire_date BETWEEN e.hire_date - 90 AND e.hire_date) AS spending_pattern
FROM employees e
ORDER BY hire_date;

-----------------------------------------
--------------WINDOW FUNCTION------------
-----------------------------------------
SELECT first_name, department,
COUNT(*) OVER(PARTITION BY department) dept_count,
COUNT(*) OVER(PARTITION BY region_id) region_count
FROM employees;

-----------------Running Total of SALARY------------------------
SELECT first_name, hire_date, salary,
SUM(salary) OVER(ORDER BY hire_date RANGE BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW) AS running_total_salary
FROM employees;

--------------------Same As above but Total Reset when department Change---------------------
SELECT first_name, hire_date, department, salary,
SUM(salary) OVER(PARTITION BY department ORDER BY hire_date) AS running_total_salary
FROM employees

-----------------------------------------
SELECT first_name, hire_date, department, salary,
SUM(salary) OVER(ORDER BY hire_date ROWS BETWEEN 3 PRECEDING AND CURRENT ROW ) AS running_total_3
FROM employees;

------------------RANK------------------
SELECT first_name, email, department, salary,
RANK() OVER(PARTITION BY department ORDER BY salary DESC)
FROM employees;

------------------NTILE------------------
SELECT first_name, email, department, salary,
NTILE(8) OVER(PARTITION BY department ORDER BY salary DESC) salary_bucket
FROM employees;

------------------FIRST_VALUE or nTH_VALUE------------------
SELECT first_name, email, department, salary,
FIRST_VALUE(salary) OVER(PARTITION BY department ORDER BY salary DESC) AS first_values
FROM employees;

------------------LEAD() & LAG------------------
SELECT department, last_name, salary,
LAG(salary) OVER(PARTITION BY department ORDER BY salary DESC) AS closest_higher_salary
FROM employees; 
------------------------------------------------
SELECT department, last_name, salary,
LEAD(salary) OVER(PARTITION BY department ORDER BY salary DESC) closest_lower_salary
FROM employees;

------------------ROLLUP & CUBES------------------
SELECT continent, country, city, SUM(units_sold) FROM sales
GROUP BY GROUPING SETS(continent,country,city);
--------------------------------------------------
SELECT continent, country, city, SUM(units_sold) FROM sales
GROUP BY ROLLUP(continent,country,city);
--------------------------------------------------
SELECT continent, country, city, SUM(units_sold) FROM sales
GROUP BY CUBE(continent,country,city);
```

To View the live site click [here &rarr;](https://portfolio-template.surge.sh)

![Portfolio Gif](/images/portfolio.gif)

## Power BI Reports

![Power BI Report](/videos/powerbi2.mp4)
![Power BI Report](/videos/powerbi1.mp4)

## MS Excel Reports

![MS Excel Report](/videos/excel1.mp4)
![MS Excel Report](/videos/excel2.mp4)

### Contributions are warmly welcomed ❤️.