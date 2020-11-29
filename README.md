# M3Bi


Spring Boot Embeded Server Used 


In Data base access url: http://localhost:9090/h2-console JDBC URL: jdbc:h2:mem:testdb

insert into user values(1, 101, 'User1');
insert into user values(2, 102, 'User2');
insert into user values(3, 103, 'User3');
insert into user values(4, 104, 'User4');

insert into hotel(id, status, price) values(10, 'AVAILABLE', 1000);
insert into hotel(id, status, price) values(11, 'AVAILABLE', 1005);
insert into hotel(id, status, price) values(12, 'AVAILABLE', 1006);

insert into bonus values(101, 1000);
insert into bonus values(102, 1002);
insert into bonus values(103, 1003);
insert into bonus values(104, 1006);


Funtionality 
1)Book hotel
POST /bookings/user/{userid}/hotel/{hotelid} Get Booking Status
E.g. POST http://localhost:9090/bookings/user/1/hotel/10

2) GET /bookings/status/user/{userid}
E.g http://localhost:9090/bookings/status/user/2

3) Update Bonus
PUT /bonuses/user/{userid}
E.g http://localhost:9090/bonuses/user/2

{
"id": 102,
"points": 1100 }
