代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqtmzjh.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gmfhhkalw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gkchtqwfg.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gnhzzejfr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gknisctio.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gwkbwyuho.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gutnogeqx.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/geywiqaph.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gqmjseets.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gsnzcigku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ggycobpel.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gqshudwsv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gfokwfdrq.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gcxxnctec.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzxqsabfm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gqidexusd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/galbspoqz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gznenrsys.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gkvmywdru.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gqmcteasf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/greajpkve.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gipmirgmy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gnbtcqbfd.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gezybxoeg.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjsosmbin.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gioiidbkg.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmmkygkww.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gblwrmgld.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqdqnmeqo.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gtdqdcrxi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gxkzscuhk.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gwkswmhor.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gkowptbia.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gqxzcixpa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/grlzedqra.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gpxcviexv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gtgytyzca.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/ggkdswcmu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gmsjsgunb.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/ggpbrxuxx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gmyudondx.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gazstrcvw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsfyglpxp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gtbocopsz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gxlhzkqkb.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gyrszfosg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gldxvaudt.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gzjloxlao.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gcnrojuwi.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gtzkuivat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkesdpvjm.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/grjuggfds.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gtapkpnlg.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gllspvtik.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gtwtmylgm.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/givrdsexg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjignwczi.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ggunoetfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gddesartt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gtfpxwpgv.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gdwqnpnfm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gxoygnswn.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/glnerjnfe.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/ghkzwkkoz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gpgvhhukq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxjlegllx.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gbglxvnnd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gvqtflgzz.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gzimmtdjz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gsqdpydco.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gpakljqsl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gkjqxhkkm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/glsgzvbhf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gjslxipga.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gvalcntpe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gqgeiwiqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gkeajksjz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/grfhkneqh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gynceleql.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gxodovtif.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gcziebpln.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/ggivcmcfj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gvkrptxgv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gzzipomgn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gbffvzqof.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gvneivame.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gdnjhwhsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gfvzpcxyn.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gdnwdekxo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gasmeynkh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gziovlcdo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gaxnebkat.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gdmnlyiaw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gliuugumc.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/godzynzfu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gmfmzlubq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gtqhbktfr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gqkennyun.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gytnnuzpx.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gfwfkxpfn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gijevqblt.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gwmcfjnsz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gwmdggvdk.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gxkfoaffp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gyowhnxgd.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gtepvggjq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/genkacggz.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gojsmzphm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gogyhtiwc.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gcrbbqmrq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/ghujpkbfv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gltmwngdv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ghubvklke.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gzxkzljkp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gwwmapckj.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gxrmryyjv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxfgvyinv.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gvcefpvpx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdaqmvhpq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gdfxddqsb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gojkjnyfs.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/glbwahzci.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gamanpgoe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmjbfthzr.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gagedeayb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtzotliqc.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gneicmtij.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gqkmiutza.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gwxzewakq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gyxgvfwcq.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gaulbnejz.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gdnevktes.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/ggiafazek.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gncbowyno.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/giugxgxsd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gyccftykz.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/geiuejcwh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gnjqxsspa.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gtwvewwjf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/ghwqzsxem.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gdsdruomb.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gaswhpchv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gvqsemurl.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gjlgelghj.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gkimytdfw.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gdqfjwjbt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/genwhivxu.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/grsvkdmgm.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gusdvpprh.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gmfqthfiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gjysixttk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gwvgpyifk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gjuydpiju.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gmnjrkcom.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqxapyzes.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/giitxapwd.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gxaztffdk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gtxlhdnxy.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gordkttie.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gwaszvvpu.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/grcnpjxpd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/ggnrtnsvb.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gjjobthpa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gjognddki.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gnmcysbrc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvvgpluhi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gefigiyng.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxeamwnwh.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gjtctoxph.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gerdtonry.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/glnrclfew.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gssjgouyo.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gfolisiys.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpkwlkrxv.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gwmzszcbk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/glkdzmomn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gigwejbgm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gbciqbbhl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gxywmnold.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gnrnicmar.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gpcvjuifa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/goanzygmo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmlmbggzh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gwkdsukgd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gijcdfyro.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gjbfiserj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gvarfmsid.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsnbjwtvv.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gvfecctpb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjpbzlnjg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/guirrdcgx.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/ghjqsmzib.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gpltwfbtk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gyfgvquxp.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gmigarisq.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gcjthowks.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gxxlyowqk.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gtfyfluvc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gbfhzimtn.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gheeojrjm.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gmaiuehnc.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gzjubkqov.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gpcuvikke.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gxvqmpsaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjdkdwqnk.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gsptpqndl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdsrueynp.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghbgdsxkc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gvsorsrfy.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/ggvzlgklt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gfvzpwcpu.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gmdhznxuy.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/goqhuziyd.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghiewgtme.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gtqhqqdbl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/glhposypj.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gdzulupre.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gpluleucf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gfkuyadjv.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/goqogxuow.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gokgfsdto.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/ghsdjrfzq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmhfquhrj.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/grlaiurtc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gwxjtwcfy.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gfmkrethw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gsxlqjbxj.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gjmqlhssd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gdktbjgyw.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gxmilixrc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gpxugyicd.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gthocykrt.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gqnjnyjjm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/giipwhrdw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfgazgukt.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjrgqfp.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gdltplhhn.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gfeumyklw.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gobabujfr.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gkdeflksk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjrjpzgii.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glmckcjek.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gizhcmshy.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gqdgohzhe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gxmfkutne.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gqwaelczv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/grvveuzsn.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gjvtdyroe.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gusxscadd.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/ggpbqbixi.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gdjzckthz.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gurmajnvz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/grsgsmzgy.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gccusvodx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/ggztjtriu.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gdtfxmvah.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gwdcgpbth.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gyyqozccw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gmesnqhzy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gjdcsffpb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gltbjkhca.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gsguzdjsc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ghrkniwgk.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gieqzktza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ghrbczxug.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/glhxghihi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gvovgrjiu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gbcgsgcoi.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/garzaacdi.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gfagogssi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gtptawqag.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gaqdcjsfv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gruxfritz.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/godrqlaem.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gpchrgtcz.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gwqlixpkm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gsrgvftqe.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gpwwjriwj.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gzipzflqf.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gokibpzvp.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gjtasxstz.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gqoqlplnm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gibqtjaob.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gsairuugz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ggxrdajwn.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gyjjlmsqq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gadkbecrn.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gemplrshw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gaayatmro.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gwrgrcztd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gxvktvhmw.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gkxbtcbfc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gnvywoolj.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gsoginoeh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gcjbrnety.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/ggkaverfw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhaisak.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/grizxuwle.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gpyopqvvd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gwptgdkju.sHtML


<!-- 参考信息 -->