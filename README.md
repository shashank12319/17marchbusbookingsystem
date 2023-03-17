# 17marchbusbookingsystem


SELECT schedule.* 
FROM travelschedule AS schedule 
LEFT JOIN stations AS source ON schedule.source_id = source.id
LEFT JOIN stations AS  destination ON schedule.destination_id = destination.id
WHERE source.id = 1 OR destination.id = 1;

SELECT * from travelschedule;

SELECT schedule.* 
FROM travelschedule AS schedule 
WHERE schedule.source_id = 1 OR schedule.destination_id = 1;

SELECT * FROM travelschedule 
WHERE source_id = 1
AND destination_id = 3
AND estimated_arrival_time > now();

SELECT * FROM travelschedule 
WHERE source_id = 1;

SELECT * FROM user WHERE username = "shree";

SELECT * FROM stations;

SELECT * FROM stations WHERE station_code = "AMR";

SELECT * from travelschedule;

Select ts.* from travelschedule ts WHERE source_id = 1 AND destination_id = 3 AND estimated_arrival_time > now();

select station0_.id as id1_5_, station0_.name as name2_5_, station0_.station_code as station_3_5_ from stations station0_ where station0_.station_code ='RNTB';

select user0_.user_id as user_id1_7_, user0_.email as email2_7_, user0_.password as password3_7_, user0_.role as role4_7_, user0_.username as username5_7_ from user user0_ where user0_.username='shree';
