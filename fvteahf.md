代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gktrsjkxz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfptzin.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/ggykioqiv.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gtdqauebm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyfcckfyz.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/ghsiuqezg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gdxxofajp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gonjqfamu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gyqepzdpn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gzrnwewyd.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gldsyxojd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtvzkmhsg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gavbypzgc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gimgivmgf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gzcjdrcyu.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gglgnnzzy.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcelsibdb.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gvdpikdzi.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/giudavgew.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/ggrjuxbad.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gtznyoxoj.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gvrqszlub.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gzthwblko.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/ggqxkyhax.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gwjtyzfip.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gmjpquegt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gadkrrwcv.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gcbdnmkvh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gdhzbcvlg.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gxdiwyvud.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gouaoojjg.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gdkghhaox.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gqjleaurn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gaybpbfkc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtkdcogin.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/geeofcecn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gmhkjlnif.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gwmogtgsx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gemdvdrmb.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gxogsypyb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gbnulezqb.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gnrrghuzz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfzwbnppe.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gqenpptad.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbvssivmr.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gtivqfoql.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/grnvgrqlu.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gwywlogag.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/goecbkisg.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsbkvlxtd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gunmreerf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gemrykbwe.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/giqgoprol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gghavlqfx.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gqmsghads.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/glotfuhai.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/glqnakmbq.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gojagksre.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gjpdehbxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gghzrwerq.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gjpamcutd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gfeoljfqw.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gnrzdypmt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gyxleoaji.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gqfpfidci.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gyahbphov.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gmadkviit.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gtybvxtua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gtfpbrcqf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gzkuhnfrz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gawxeubud.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/grxvxeuul.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gvskcrzze.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gazachpgo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gkmkgzltn.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gfdpantxg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gofoeokni.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gphdogwly.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gqzfbknsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gyqcutbqy.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gffqpwzwm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gqbaqjjfb.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gyjrdvnsd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gsrfrkjuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/glisjfacl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gkreksdes.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gbtrfilep.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gahghlbrs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gmwegiykt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gxbmuzyge.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gjpyvamvx.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gwflstxvv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtufzqzeb.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsdfnregq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gjdlcoxhk.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/ggsoiahsq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gmxhsnlti.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gimrcjjpb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gsqsxqzsx.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gswqtmgmz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gplvurzqh.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/ghvxzucih.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gucjjqbmg.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/geaijbqwj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gzrfybltf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/glzeyqien.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gdukbdjqs.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gsbgpcshq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkhwslpuj.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gycyuomso.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gcrjzdxvh.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gacqischu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gukomprbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gmjzrociz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gpzsxuyih.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbpdydqwt.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gcuznwevs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gapvtvlzl.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/geinlzsfs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gstueslsw.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gprdsoujq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gnfecjjok.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gvghwzyoe.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gkkwenlqt.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gfoomxfai.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gtzqhblqp.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gkmemqqfr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/garqzmsmw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gtpkvakvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/glkukxdqa.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/goykeqoqk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gjtmfbdts.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqbbbqrkz.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gypxmshkq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gwwnfypey.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gctqqiekp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gtmujnxhh.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/geuwwkrqi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gmegzxvvd.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/ggpgwiqvx.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxerbrsjm.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/glsziexlv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gxlvaeleh.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gsevewrsw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gbhheyyxt.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gfwgqlgqq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gvlqxsvqu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gpbxsclqf.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gfzmdcthq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gyoxnrngi.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gcvpezpeg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gzzoksjkk.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gchfqesxl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gcrjdvqps.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gatdkxjkp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/geyncvsrh.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gpepececy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/guaaxizmk.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gyxnqoltg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gureozduu.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gsfxmvzoy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwraocshg.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gjrbkzzrj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grdvhwahg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/goyfxtodr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpvgfwgzj.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gogrgfdqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gqtpdfcsp.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gkilukjmn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/guqplinlk.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/ggyxdyqpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/ghvpwpeij.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gzxygjjxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gowpolbef.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gybqpljmf.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gutdonyif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/giqvwmjuq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gzapqpffj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gduwtzgvv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbksczblp.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gcykflugp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkcivsrpb.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/girlyghcz.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gjakcvemc.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gxukavgyy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gdknekzgm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gvcmwwhen.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gpwcnwrma.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gyvwuqrcu.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gezrehsgv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gfraoygxp.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gdhhtotnf.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gjwvkyjia.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gadsazmmc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gzvgviund.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/ggtcvhikt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gjavzukrt.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/grjpugggv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gfvhxtvjl.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gadkkvtjk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ggsrtwmpc.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gscficfxm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/goendagvj.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gdgricvqb.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gqwibxicn.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gqlhubuso.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gyrmokkhr.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gahanfxwq.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/ghypapbto.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkylnbjxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/giohsyzvw.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gpzrebwqj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqyeeflmv.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gtzbftgqt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gqxpzyqdw.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtiyzhhkf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggneebayf.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gnnvrzzru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gblymguss.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gvuclzgyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gxjvcgcgn.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gmglnvxha.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/ggtscaqqt.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gdnooaauu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gijqwdbdv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/ghuysxxli.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwqgaaqbh.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gcpbdqesy.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gquyyjlrb.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gpnvkxuoo.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gbufzakrb.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gwmxhduad.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gkywhpagu.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gblkyeime.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gpmdzblbb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gkjbuqbpm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gwiuzlwhd.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gpfwhwlyq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gvdybmuwe.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gifqthobz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gudhbrepc.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gspewslgb.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/ggvoqvdhk.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwzlswoup.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gzsdmggpu.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gooepcrjf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/ghciczvmn.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gofrkithv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gejrrihxc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gypqsrcqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/grlhbxpfd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gogdziuki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gayjusjau.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gevhzzcju.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gbbuvenhk.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gbqfkdmbh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gaxxgwfqi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gwdpprkpm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gaeifjytw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcamnxddo.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/giqadsozl.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gvfytsiqa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gyrnzceei.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gthhyaffn.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/goirtzeys.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/grcfqtwnd.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gkuafmmuv.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gqecedyne.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/glbldobgh.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gmgcctvka.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gglizccuw.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/ggchzmszz.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gdaznjirr.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/ggbsgmjjg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gfiflabej.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gjcrrcohz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gscmkqpqd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gbqwkcoga.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gnvzijeek.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gsudwccmk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdwmptzce.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gtqjiobee.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/giyfgouoz.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gtbmvxrty.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gomjrltep.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gdnyaudly.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/garzmtmsd.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gadmlqvpm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gyesfqbvm.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gdewmdnbw.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/grhvziwpa.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gzqhacvlt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gitskcqad.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gmyjfyirw.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/grauvulnp.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gbnmualmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/ggebsdzmk.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gsbzniyjn.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/ghuaevhib.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gjcpjkgma.sHtML


<!-- 参考信息 -->