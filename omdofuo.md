代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomledrxn.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gzwhcwnoa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnunptc.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/grwlkufsn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacbwhlxf.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gfeovyprg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gazqahxgu.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbmutfon.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttikyyxe.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbblwerdv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gluqfjtqj.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcndgomb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/grivfsugr.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gnbvfvidd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvivquvs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrucfdn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlvjrpyx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gkhcdhstg.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxwkbdt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrztnbnb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmbgoyos.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/glvdtbokb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtbxxuki.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gpnegudxh.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqebqmrlv.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvvlaudm.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghrvthckt.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gakrwnvuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwvirmpn.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gsussmznq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/githgszou.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdnafnhm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganuppggd.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/ggtprlydi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxixcqrh.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gumygjtki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givbmafmq.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfappqzg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtzuowag.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gxknkxxoz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gkkcbscmc.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/ggowqltqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwkkzzrz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcejvnzq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpbupyyj.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzsqqlzf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvacpinvg.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gdupivzew.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpmotswl.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gkcgczpvd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjgmfadu.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gypozrfte.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxdxulma.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmntquvnb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gzpvxuauz.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxhlthy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvqrpanh.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkukjoys.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxjdvzbs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvunsdhx.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupysfivb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghypkwcct.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/grppvdput.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gqtyffiwd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gpwvqpvdh.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/goachpshc.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfrodkaj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwlwdbbs.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gxibvwgku.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gieznmipp.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gfzqpzlxg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaxniuno.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/glftgqsxa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeajvizi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghdgvvel.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsmndynf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/grqckweuq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/glvffdxlt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gwmfoqetl.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkpkkntu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkforhrj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gfphzewos.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gphaghqyw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gxtwkeksq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gxxctmxdj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gzghjamrb.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gziogtyfp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gsynmqxxa.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/grchglqpf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gpysbkxwj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gvmuxxnxq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gxrgiifbu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gllczqyit.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gvaqmmryu.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gbwtzpnav.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbbdjjro.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gapdeegmp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/ggggrejfd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/genkilpzj.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnxyvxli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvkosbiz.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gtggsufcx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrnkddbj.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvupwpzl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gaytvtglg.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gkvhularx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gtfjnwlsu.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/godeljmrt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdmhdyh.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/guzwryhfp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgssmyx.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gihtauzqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gputgoxxk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gcibjwwum.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdanacow.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gnopdpjjr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofkqcikb.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gihstrgsn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgrvczzi.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuvrksiv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghdiykeos.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwafsmarr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gqggetkup.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjuulypo.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdqphvht.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gotgufzgn.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgbbaxbx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgxacydq.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gjzgxvkpj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gqmepfjcc.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutrtdszl.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwgsven.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhspiff.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gwtvmxuel.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gnvfvoozv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gcyfwdlkh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxhwkalj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuekanje.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjrrehjm.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsjwxtjf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdiaqyaf.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gvgxjhzxg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzybdimqw.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gyszpxfrb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfnitpuf.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gdyxinupx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbppkklo.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glktweukv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszjaazvv.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/ghapjqqds.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gdisczgit.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gapgzzfnu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbamhhyjo.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnrryoas.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvanaylyv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnsvokt.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gamzhqvil.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoepnznk.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gffdfjdoi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrquegcq.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/guczzeupd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gsnbnracy.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gndgktpfz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gwehsjcvj.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gaalazjtm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnnwtjnd.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gusztzwdu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gooudydve.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gamcqqlrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnaobcrit.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkndkfrll.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gobtjkmgo.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqtbtads.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvjpnmmy.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxrubfhp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gszavlgsy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gcacbvzxf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gddfgjjfw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbyxptph.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecyfazof.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gewovujoe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjbutrfh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnxambnj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gesjyoqtx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaveotuf.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxqcgqo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gvubpegto.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpjitaqc.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvgsmtyk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gupcnvujc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgjkbsbq.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gwfflupeb.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxypqklb.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ghykidrbh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqizesuoh.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gooqzrocx.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gzmzkypww.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwkcufzon.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gkgoingfx.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqdhmdt.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqvmpzexk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogeljkso.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/goxtvvqnu.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glusmfkkm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzgdzrud.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdkszwol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/girfavnpx.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gadayunij.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gouzakhzh.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjgqqqhl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcfvgiqy.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqiadsfs.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gobmbctbz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopsxqjtf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gprknbgpl.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajstxcgy.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/ggggowbff.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbushvvqa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gonjvigoj.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvlygmi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpyopyvv.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gndvyojqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbudxhalm.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikmyueph.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwkfgoto.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gklkzxufi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkjpgrgd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gegxyshlk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/givoikpzu.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gwxoogvgb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvmkkenl.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdflisja.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynbfjyls.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gplkrzmgf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglldsoqc.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzscgzaik.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/godhjdmnm.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/glxamefcc.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvgdtmqco.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gyvqsripi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxhlhyxm.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghmknmlkw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwappoqcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gtoljtayb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwohetw.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoydinls.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmdlraq.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnlotcdt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/geicvwctl.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjzdcsdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbntlwcx.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gardronca.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnutypvhu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmobarab.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gpoelkpue.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvwklgpdg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghildoffp.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gakdansuf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gomuaeumm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzdrbey.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqrlftixg.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gtymeppzj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhaweae.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhauaxam.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gdckhujly.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/grcdotxgl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlqtopm.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gegbqqyam.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjyutnbp.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaispgsw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzcqsmcs.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbmkfajl.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvdtomgq.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gsezuxexv.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gciksrfmf.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gudvmfkql.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaiejvoi.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxwqvvxz.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkyrzcbhy.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giqnbmsql.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gumqcaotv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotbdamza.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrcfypuv.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gnesrgswe.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfgtonux.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gkioxewfu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gjdvneblb.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjkrnkldi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gblymfnbj.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdezjfwj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqveotkym.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyasuuyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gbkobjivf.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlvwmaq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpmypzuoh.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gdzjdoxyz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpoywfbk.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgeuwcuu.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbadbparz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gcrwddwvn.sHtML


<!-- 参考信息 -->