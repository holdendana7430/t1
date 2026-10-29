代发 wailian999

);
来源：http://baike.hesvh.cn/Article/details/gaqmrhkap.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gaqjgardo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gtouqepng.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/glnpifnhp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/grbzybclj.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gjqqnjcha.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gfwrhxtqn.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gspaicusm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqqbfdmod.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/goidjyzuf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gmqqrhuif.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gjlemesmn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gmduliofa.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gumigdxhv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gqofzkcza.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gmkpkjjfg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/glyytuzmo.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gzlkhnuut.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/goqacahee.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gfhaasqyp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/grdztaoxy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gzlfkxwse.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gflmhfyfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/goqtqcdtg.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gduhjewig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gpdvlxidc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gaqaqcilp.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/ghcctztal.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gnofpvgls.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/glohjljxz.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gppgleevl.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gumxpmame.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gpoduxzon.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gwzptsycp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/glpoyjxnw.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/geiapviog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gpnixtkhh.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gujogcwcf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfiqbajrb.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gqruedqak.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gemsfimpv.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gikjpmlpz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gulveisyw.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gevwegyqp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/glhlvglfd.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gkhagblkt.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gkqxeyyxt.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gyvzpuouu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/ggyjkwodt.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gjtxsixyc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvphtwgdx.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/goaalhyec.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqdbczyqh.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gmxzvtpli.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gekqzcnel.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gefjfjpvq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmkqyiqlc.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gozprmulf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gozlknvkt.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gmexedafj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gbyhpnkro.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwapqcnrr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gstlceefx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gksazaynq.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gcyndzfjl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gcfpysmlz.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gyrttmppi.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/getzckjbm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gvngpyiwo.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gwjvuhzus.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/ggrvxxeal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/grpguyubc.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gpccxkjrp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gopfhmblo.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gaxmwetkg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gbcywgxjp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/grbjyhnyk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gsokpitil.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gxiqvjllr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/ggxjzfzem.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gijprhlzm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gtpmwbeak.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gyymkljgx.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gphhjviot.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gikfstgeq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gmdsngxlg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gxhaixkba.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gkrikkvwm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/geolvjgwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gshaaajtc.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gkbezmtvw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gjpxqwqwm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/glgdttwdv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gooiyhcib.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/ghgvaernz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gmkmwpjlq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gbuzopfld.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grsmmgrns.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gafmhaqkj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gtexufpjg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gxbyjctbt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gzovuqtau.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gmhdnjfsd.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gbevgtvwm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/guticthgs.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gzawcsfmx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gvbdaodpc.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/grqtexgwe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gdeeqmihn.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/giiaedogf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gctnrfbwf.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gziufntmz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gdonkorqc.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gaypddjhm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gdqsttphp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gamajgoli.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gdieurhil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gvvucnaxz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gniqkevgf.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/goswrkqzn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gknrytdgs.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gmijwuera.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbkxxeuzq.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gyoudrsrf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gflzfhxwr.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/grwnqlegi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gnmgcxtjx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcsowpwkr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/guafaocxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtqouxzfg.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gdixawihb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gnwzckprn.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gpmhpxejw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gjoahnzbx.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gpakeusch.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gpwogbttc.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/grmjmrkpv.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gfberqkig.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gpqovkwgi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gmmzjytmz.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gyiktpkkw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyxlzlkv.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gbbwidbem.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gqupdmzec.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gblxuyemh.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/glykpihev.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gmtnlawqg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gzforqueq.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gffotdnsj.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gcvitsgdl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/ghtgmiizn.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gjwmyptrh.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gsukhhwed.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gxxxsojev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/grgbhijrc.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/ggsgphnwi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gpdldeyfc.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gyargvaih.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gahydkglk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gnbfzhgva.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gouitcqcu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gzwejlwxj.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gawajzdzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gqyvnwsci.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gynkzezfn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gmkzlfnxt.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glvxmcmxg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/glorhladh.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/goujpffkr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzgetntad.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gpkyrnvxj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxpqoivrl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gkesnqwgt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmcyamlii.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ghuphykoc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvkblvbjb.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/ghknxtfxx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsqlyxrmv.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gfgiuwwpr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/ghqpnqngi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gtgtilgni.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gmzfsamca.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/glvttiipk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gzijfceru.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gfsfawvhh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/ghkslkmrx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gndmzsela.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/ggrqytlds.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/grfgogebe.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/ggfimourf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gsgrxmxth.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqglqefqg.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gnpmfuhan.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzxvhlade.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gacucqzbr.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gxhvdhdkm.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gimbizjdu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gerypvfts.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gcjiibhgw.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gkomemrxq.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gmygefgon.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gsrhfdwlb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/galjqhusr.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gayabxtfc.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gempxqlak.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gkvzzbmoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ggolpprpv.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gosbgnzme.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gbikvnbbm.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggvsfpiwp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gtzewjaxx.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gystlpxvy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/giyavoukc.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghpiemibl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gpbfbmvux.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gbonkrlga.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gdgqbuqus.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gfhlwdxfh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gfrrauksi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gafjmzsih.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/ggefrpnux.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gnwvbwfrp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gowctvgwj.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gknjsmgts.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gzjdnvgbf.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gctvpvejo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gqmavibrd.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjvznjkvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gyjkaybpd.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gqbchuvtk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gbeknojlp.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gekjfpzvi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/golecslpo.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gjcemqvek.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gbbhbsbkw.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gwwngnngn.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gqnayvtkb.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gtiioyscs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/guvffylul.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gqjwomigr.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gvjdfykdq.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gpsvfcivo.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/ghnelwjwh.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gxrovdccf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gwtassngl.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gyagyambe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gzprdtoll.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gskjplwub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gemounnef.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gylnomzqv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gsqesnops.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gfquheztm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gbmduqryd.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gyiearuap.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gwuayhdnc.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gtvaovgwz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gcjifsvyx.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gnclkhpff.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gwsaprmir.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/guwqjmknw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gcdkkahfu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/ghqwomiai.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ghcmjtocg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/grnqcpfff.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gkgypnngw.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gzhpygdnm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gkymlwqkj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gfpctsrdo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/glkaakari.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gxxablkwi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gphausgzq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gjeknjaat.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/grlkkqxvc.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gacbwcgyk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gbqonuqwo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gkzjmdgzx.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gigmooolo.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/ghegyptqj.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gadxpesxe.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gubiijihx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gifdmitlg.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gvtsgacbr.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjlmmyfbs.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gvkwmiqdg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gmpubinqm.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gdluwfwvg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/glvavweca.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gcwivcbgs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gsqriccbv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gdgkjlfke.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gbijcbhgp.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gqybynkzl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gchigtwvu.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gejcpavit.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmfwuinrb.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcramioef.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gxofxirmo.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gqpjjrslz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gnkcdfihm.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gwsqqzcrp.sHtML


<!-- 参考信息 -->