代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmvmbshw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gzovkyzzf.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gboxouncf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gftcmquef.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/glonrndsk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqymkym.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/grnoeivrg.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgsmzvd.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gepegkbct.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxteecbub.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmyfpjcd.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynhgqtrm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gntinolpl.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gihxaxtyu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgnzzpz.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgnqjubm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwsadlop.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpyzdpyl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchskwbrq.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahzmpskz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gioulzlmd.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/guenjsarq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gysxcshmx.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghotnrqup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzrhfeve.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gdloewqaa.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gymvtvkbr.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gutjjvkyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gkftmqkyq.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gybjfkncz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gregdhklr.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/godnrfdjf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgfziybq.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gnawxxpez.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjdfmlxc.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/grzbrneyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grsxafyon.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gztejnbbi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gmmuxteqv.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjahdejaj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gaitvvrqg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsdiylpy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gsfqvcezt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyygeciv.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfcqsur.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gpxtsdnno.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gunkqrymm.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gikqsztdg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gnoxrjytj.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gczicwtjl.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/goxixzqmj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsekutnq.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcryfkcou.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqqeydau.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqfqsecju.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzfaozgdy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcintmcn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkituyicy.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghetksgws.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gjzzqwzak.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnmhwhow.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsbabepn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxvmkmno.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/giurlvjtc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmsrbmgr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/glvahsaot.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/geduxpniq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfxrhause.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxmprmfz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyedbrmz.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubzbftqg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtbcsxoj.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/goqqaihqv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrcazrdt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gtqeoycce.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ggfqluqfv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdqdbcgh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbhibsyi.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyffdici.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdgnfstw.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/grczxrdoz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkuamehd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlpbajhd.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxtiuey.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gthalkckv.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsrthxum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjkjxfih.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gedigsmrj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcupptcid.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gjprowsxb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvnbvop.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqhgnfo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gocfoakav.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpsldweq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpefyhefa.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gumlubdpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcelzdpmd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gkkwkmuul.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrlmqpcf.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gtydurxzj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbstfgpnx.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnzomvscj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhpherop.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gfzbmixuu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/geihrikls.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gttliaezt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyqaxfbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfscrun.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/geshoproj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgqghjrs.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxybxexi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsviatzjt.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcscgkdvo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwupdhla.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqsuwrnr.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghybpsrws.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsadevz.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcvozvhn.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gzkhtwjvy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghavleqjm.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gkpnnhiiy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/geussyunf.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/galbkjtrg.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gujkkrlbx.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvfqbqhq.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ghlnpdrko.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmroztet.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gtedbyhgd.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkusoshkn.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gltehqmio.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/grvhldfri.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzgslccm.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grkkgxyun.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/guxplaeug.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbuowzit.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaqscxtc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhyfykdo.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbwcsrvb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyunocxd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gjxgndrxn.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzvjfxrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gvsyebvug.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gzehtckyz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getklgmhh.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/grljzxjlg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gzahuszcs.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/glbvljueo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxvttsgt.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gqbqwlatb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtpzmijlc.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvssndndr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmqqoyaz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkascexg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gspqwgrvt.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvlguphgl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubcvpsaf.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/guvqywxpa.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpbpodolc.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gicmjkbpw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ggftokopz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqipowds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfteaww.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gkzhfigsp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmgsonfs.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/geaevuueh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggryktsiy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtestvtmk.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmugqjchi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guedlhfbo.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbdruitm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdffimjsb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glexjvbpb.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gasvmdcpt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grqifplcm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgwtwebu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvvqggyn.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjkdkusi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgboifua.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gvvgtlghn.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyyhytyjj.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gryqsfrvm.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwnyqpiq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcuskasu.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gesfoaaju.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibhheexw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvqspch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdkshjti.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbggkeew.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxounzwdi.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcifvyns.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gvmocnaov.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvumtmjg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gybbjwmrb.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxmwdvnlw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gluamqntz.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/geywsyero.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gdzaqfubu.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgnmnqip.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gmrrpkogu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsidznqdo.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggelawvkb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcdqdahf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvnizoji.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwipfrxkx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtcrmyfyb.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gflnujirg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glwrednsh.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glmumupqe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfwbhpds.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gaulnamje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goxnrrzoo.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gxmmxcugn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gswgdjcdw.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcygwasf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsebpdyd.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcntvleuj.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gevxnpzah.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvogborkc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggfvhyaek.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gxixmgzcr.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkjnbvrk.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdyovyru.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmhfibezo.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkvvppgfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gstlgrkgp.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/goittdxnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/grrxvecfs.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/glkqqxjzy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqeluwme.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdntqikek.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gihqcniap.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxlhyyua.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/geytmacyg.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshjzeonu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gpnkdaxnd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgzgpyhr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gemnujsqh.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpadcqxgn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gqaibuggn.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwfnouar.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghatlxitg.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgghtyfh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/guuhqzexa.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxkngaod.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsutfldx.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzsjupt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gbidxrqma.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvrcphyt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gygggldnp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncfpoybx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gflinnldz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/giwqdboyh.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gimjyjtlg.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgttkzka.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gabfdmeud.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqugnruy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guddfhhbm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggltgheom.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpghelkkm.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwayulh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gysauszgv.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurftgqmh.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gexuobirl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdcpigvm.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmobeqcu.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbatzxax.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/goicdgtws.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gpafdouwf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gdbartotp.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/geppdeleu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxqogtp.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwmvatoz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrrbevwd.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjljxfyq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtihbgfbr.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gteivrjbl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gxlgxwbph.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtplstmmw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvnvdzdvr.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gimjtffun.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfysvvyzr.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gzexeteux.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjpeyhiqn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmtkcrg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvinclii.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjapsgsy.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhivbvnp.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvziomgs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gfiqzbjrz.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/guktybqgj.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/glpsmbdll.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsodlwso.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/grdgjmosi.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtomrrwyc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjieyena.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgpplkw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gwnywiogs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/geznfuosw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/glieuuwmp.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/griknmaqr.sHtML


<!-- 参考信息 -->