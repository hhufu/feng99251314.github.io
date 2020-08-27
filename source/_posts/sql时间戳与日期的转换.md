---

title: sql时间戳与日期相互转换

date:

tags: Mysql

---

NOW()：当前日期时间
SELECT UNIX_TIMESTAMP(NOW());
将日期格式转成时间戳 1493016522 SELECT UNIX_TIMESTAMP(create_time);

SELECT FROM_UNIXTIME(1493016148);
将时间戳转成日期格式 2017-04-24 14:42:28