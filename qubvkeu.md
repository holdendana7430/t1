代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrripgcm.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gyyjhhckr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgedtnbo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwxibrvq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/guwzlvurd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gbceimkbw.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gmjddmlob.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gmjniuytr.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsafpknmy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdfqvhwx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gthezcgen.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzfgldyg.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guuecvmhc.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/glrbrhgnx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggccphtpp.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gobexrpjj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvwyfxvr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grztnaote.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/genbdiqus.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrcmpziz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtjsynej.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gesdvnqlw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grhtmhqmq.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gktvtqcnz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gmipxnqpi.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdqbcwrac.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpddbzixk.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gtrlmpmsc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gndmlicoz.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gykuduumz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grvxmuweb.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gvwarcjgb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gvjtqtkkp.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvmiyfmy.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghixhexqi.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlvrgnfu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtaaavdun.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gnkjdbins.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxdecvdr.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gnpbgqxbi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grcvbhshu.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpciogmd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjssbmrx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukryzzqm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzddhnkr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbpblcrl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/goffxukuj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/giuxslkvc.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzocdephz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebvryfkf.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gafxdoqht.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/grqrctxnr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gjbllcfnq.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gywzvntqd.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gznfnsuoi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gbdsmhzvz.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghadkjuhf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhqtwmnz.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtfdeoth.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngcfkmlo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gsvxbfsbk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrmyjhgk.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gdiyhodnv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhyxutri.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gvncguktu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gzeclbibf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gsboxhwwj.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqzuyrjq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvqlorey.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gufpcreww.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcosdefa.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gofgaeqtr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/grolzscib.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlbwlrzc.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gkycfjsge.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gfvvxiiwl.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjpyheyic.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsstwrtal.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtayhugpa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gpqbxolau.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqyetpjm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glshojnjx.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/guuuotynx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrwxxrfk.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxbjwpui.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gizkicurn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbpfoxii.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjmnqpch.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gceernwxz.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gebxdpifw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/guirnidwn.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuwxwmaz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grlxjnpox.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/grkzzwzqr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckdfijmx.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gyloqyctm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrdqmiqg.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gbzukikyl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnpistpn.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gefnbyeoo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtsbxprp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbqidhxe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/giklddlsw.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/glnjkvsye.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgjttdsr.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gobubvobr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgywutod.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbpivuds.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyfsrapw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/goafxelqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhivnlwi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gudukislj.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gxlegezdc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyypevynh.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gvawnhbot.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gffdhaqtm.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guisuiood.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmkmwswq.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gswkyaqno.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlhgigza.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnwvcmqz.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfaltxem.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdibzcvnh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gdokweonk.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gtsbbhlcz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/giuamiszm.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gijkrehit.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlxsxzpo.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gpewqanxb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdskkrwn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylecjur.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gyftamziy.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqrajkwp.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwvmwqcy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsqkmyqg.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmygmwzop.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijozhvzi.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeopqdkm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gohbxkivt.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtxakekaj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gfmyzqrni.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gcimdffpx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcixviqwt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/grxowjddu.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/girbazsje.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gkccmesyo.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmgrqhai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfyurnmf.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnrguuayg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/govkqbjlt.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhxkdkbf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gekvlkiwo.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gufngvcgm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goyczbxaj.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmxbiox.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggoimzrwc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkppnsad.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkhwkjac.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gurpjhfda.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grlmwrrfn.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gbushndje.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gduhacsvp.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gckwdzjbw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gkikakdtl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdrogeyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gpipejqua.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxziswbp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoafkdvr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzwvsjcx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwattvtz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gutezadmo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfyhbmvg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gnvsztohf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbiepxnh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspheeazt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqijskezz.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gedhuvmqo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwipzfclr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbieyqke.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikmihkpa.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqzdpfao.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkfbebw.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/getycbjwv.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gidjgcfxv.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gdkchvjts.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gslirvaix.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/giatxjxxy.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqtbezhpw.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcwvembaz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gopxjkomf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkogdchh.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaixybhr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbsmqpigu.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkccdskzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdjiulnx.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxfdjswji.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goskwnsns.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgelkhxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoxmmicc.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/grsfxxqrq.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gbmmimziq.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gosyvemkx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfztsjub.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtczxqzms.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdswpemr.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcnriewi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gikaxewzp.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxnrkwzsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkxdzoyn.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gzjzxiavs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpremfsm.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgfdpdlb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gezrjpywz.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggyoqnhjo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goncuwlts.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/goolckzel.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhqhisdm.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwotvxm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcpplocq.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtufzyb.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/giyegbenk.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/glkixulcl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxzsolwzp.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghkicscqi.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlkvaxug.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/ggdusnuty.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqkguurv.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gheldgtco.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gondgkwtl.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbdyjenx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbmmfpex.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gqlgxpdzr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntmpecoh.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grnpcmmqh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gqbpvgjxa.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxeiutqa.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgtcnocn.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gfwnwckec.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gbccvhmau.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqmquic.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcgjdgdnk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/giqjuqynx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpybumcu.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmutlwng.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyrbgkyz.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/geuqclbmc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxtliwdi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gqisntvaw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gpfpmmhto.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gexhlybfg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwlnpdica.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gljljxfwe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/grszplsrn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcjwzzzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/ghdqjfkzg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfulgpdan.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxikiavl.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gajptlvkk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gyqcpewqk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gtsjwzxwo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnysboeq.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwlkrujbb.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gwbjziyfd.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gxsdzcfol.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwvtbyex.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gzfoknaga.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbnintjlc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuqgyito.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gapwiosso.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhotyivv.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpqbiryxj.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdlrruel.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjzjvomql.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhsnvcbg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzlboqz.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjbaxnm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guurxvshq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaznxqwns.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrhwdfkx.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gemjzpeua.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqswhiglv.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gipbncpdo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhpdcsk.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeowwddl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwvnunsw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjxjssjq.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geguzwymq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/ghekkdcsq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxruzqwfj.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gflssyqey.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyvjjybff.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gnigxebtr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmyvljko.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpifmwwju.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbcvcikq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/ggganvtpx.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjmosogrh.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzgdmuxhv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbstjqzs.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhvksycs.sHtML


<!-- 参考信息 -->