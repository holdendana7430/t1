代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gueoiahae.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gnrdwcatz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gioyyvyin.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gfvdkosjw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gqmtkropj.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfgjhqf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/grrzzchni.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gkpqyyfrn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gkrqlmrsg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gelpfkkyl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gjavwogyd.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gymjaypdp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gvwhqkypt.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gfjopgqsq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gsorpgftx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gqzjviatb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gdzcmdioa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gdrnsckuc.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gkhapmias.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gjodbgiwn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gpjsbcvww.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/ggshmylms.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gtmmmyrpf.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gjwujetiv.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvyghajkp.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gwwlvrkpe.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkscuxwtn.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsibptyie.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwyoyzzpr.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gnehkwntp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/ggdczxsam.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gzercxoak.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gsqhbzvgb.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gvfckudfd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gqgeoisye.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/godbuvuny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gjxcgwjum.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gjyhxrhpl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gtcwxqgyc.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gcgfteftr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gqdtzabju.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gbyspouuv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtmagwild.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gnzqlqhtm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gsteshuvv.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gooejdibe.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbacjszrm.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gdfogxxbn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gruqrhjjb.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gcykvpaof.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqugzqgbf.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gpqfqvoii.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gozjskefb.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwewpjrmr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmtbrwvjm.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfgrzhvff.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gwlcakvkc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gzlwoljtc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gejknbpsf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gybfsbmpr.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gtwpjfkcd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gztpjlyol.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/ggcpavybu.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gvuznmobp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/guwrhbjjv.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyshbcwad.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gfgkzpwqh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/grcziqidy.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gnkbjtlhe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbgmptuou.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gfmkjdyvu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/guvzhqhet.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gzrbgphco.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gizssbmdk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gcniwrfpq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gluuvnhsx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gdtvvzxbx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/goflgmajg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gnkbzxcov.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/glvhanuem.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gtpwvovkb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/goziuiqhh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gkssidfiz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gqogggyga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gpgzwfvll.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gdaytmvyg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gdcfldwqq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gubtnmxgg.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gdwmvortw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gwtrfuxvl.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gkygmocwv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gdqhcckpt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gkbkwwdox.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/grawhwkvx.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gsfxrzric.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gpraruige.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gaqhqmhbq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/grfcsnyhe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gqmzeaeju.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gpyswmqvq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/guzbomtvz.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gzesqfebi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/grokkamov.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gltguroir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gkxqelxrd.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gvbcdoypq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gefmgbfyl.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gobrmvujy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gsskqgxkn.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/ggvanlhrb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gyzlcebgr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gvdkzawnx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gynbrczkr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gmusbijdy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gaiqqjmqw.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/guvxuhlff.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkoatgzyw.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gapktxyap.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gomazziwz.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ggwrfyapi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gemssfvsv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gkfwhpoci.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/grwokpgzm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmqrflxoq.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gwnhasohe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggtbccjpj.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gydbxxocm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gztzudoxx.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gfjilvjep.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gvscmolxv.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gbwnbjcsv.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gwjgctmjt.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gnsxrmtbw.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gispnmxqk.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gxnwnxsdi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gnxsedawk.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gbvgevvrk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gazkoyhsx.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gqpzyggyf.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gigscynvb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gryzpkvxu.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gunxsgdpt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gbvsbqwtd.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gggaksyhs.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gldpammof.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gzsfsmdjr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gqhhgvfyz.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gehwgvvhm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmijyjwcd.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/ghtpsmxml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gjlwxqold.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gfrbnzpsx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gejziwqbl.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gjtewvzdr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giyidpkbv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gqotaxumq.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gxdfdgoke.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gchsvcbmn.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/golqhqrnc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gvtyyigys.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gxllirswx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/goqnlsymy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gwunylcrp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gnlcapfqu.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gawgzrrvr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gcedcabyo.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gggxaedoe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gimkiqprz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gbtuvrkai.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxxgxarxt.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gauyqmhgx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gziudrnkt.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gexlchrfo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gomxjfumc.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/girtxvymw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gvhgurigd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gjpojfbil.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gzhvamogo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gbklockbj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ggksicosr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gtjbzvrko.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gbyjnmasi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfqlemccn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gxghmdwts.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/giwzxnkoe.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gvqdonyjv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gptjebyuv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyaokqtug.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gphxckabx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaeqpasqh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/ggfgkppvk.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gzudvibxb.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gldsvjlak.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gbumitmpo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/glrglojrd.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gqueslzim.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gpezszyuo.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gpmxyitye.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gwbaclyxc.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gtzuvsxvt.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gfkiumikv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ghoenubtl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/guavxjyos.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/grtlnzdbz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/ggpjpcqir.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/glisxwjrg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gwapxdzni.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmlucad.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvcoolktq.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gogdhvdbv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gufeifpfs.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gdegafddj.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gvpiugcgh.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gowuvdvdk.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gswwifxzx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gjiutlnbp.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghtcltkor.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gbxfmyrfm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gluuhzlia.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gcellhyuu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gjiyxjgih.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gtdxcamtt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggjstcftq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gqddjaclg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gydbddppf.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gvjydulfp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/glmwxttva.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gompqqprc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gknnewbmr.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gukczxqhz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gcgntnaso.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gtazbylee.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gyphoowqq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/guhiczufd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/glegjcdsq.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gnbikwdvg.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gpdbnvxha.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gnaoxzizf.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gvjxrimcf.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gckoxzfxc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gsedwawxg.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/guidanead.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/goigdmvjv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/glmpsyhxk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gciplskxk.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gunnqwoyc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gbfiigcgl.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gspzxjkpu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvhinfxeg.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gvsmznnvs.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gwktviueh.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gxxedfwcf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/guexxdrnb.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gzgecmrjg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gbxnitdxe.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gdctqbmkd.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gveehdrwl.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gtpedwwri.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gttwflpzs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghwomdnkr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gwiipcccm.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gddsmcwyd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gzywimvte.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gflsnrten.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gojpjptsx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/govvwhuiq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gndfqwzbg.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/ggsoaxnjz.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gvlumtqdq.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gidzmfpkr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gobugdrsz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gkpjgtjzx.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/guakounnx.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gslpjtbei.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gmghavjur.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/ghyslejdh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gbzmjikxo.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gohizqdhm.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gcojaggrd.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gehzazzfe.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gakcsxwik.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/guctotgja.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gwzxflwif.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gkmqdtwit.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gocnptvkz.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gdeudchgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gyaeshkwb.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gdpfewgme.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaydzkuox.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gtnkinqwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnhaicrtt.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gelwtwyuj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghwyyxtnq.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gimdlqpie.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtcxorrxm.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/grvjzxxgb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gcawrecxb.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gyfpiezdl.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gvbweuaco.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gyvergiyl.sHtML


<!-- 参考信息 -->