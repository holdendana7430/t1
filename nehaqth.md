代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkuuwbjk.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/guoshesbv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/glfagebgv.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gncuolnaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gbkzqzngl.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gteorpytk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gclqiicii.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/giehmdmhz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gltlmiblo.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gdonviooa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/giwkbenrd.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gsdxcvnjf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gkjnffywr.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gjpdrsxru.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ggucgnaxk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gdoskryxq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gmdqdqelw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gweglmbfl.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gjswcxhiz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/geuyfojti.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gjlkeiuus.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gptwdtxzk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gdwphntbq.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gqywuwoxa.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggokatfhj.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gkuaxhwnr.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gommlcava.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxkalmnwo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrvgcfno.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gngamlbvl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gvgzvcuvb.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gfvpkmswx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gsvekofnd.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gakickzjv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gbuugkqpy.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gzlqcewju.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gowadjdbb.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gdlanbgcy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gnclzbzik.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gvhzqpbhw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gzgabhqjc.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/glsyyryav.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/goixktavy.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gzejmmvad.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gnqajrngo.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/grdbemkyb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmkobtixl.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/ghvttfqpo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghpjiyuxm.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gnxgxfnec.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gecbjliom.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gpikhbpnm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqjwjtwoy.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gjaqozdyi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxyybbeyg.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gemvkkaup.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gbblkmhen.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gkjrzquoq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gozxpqrub.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gzsjabwoh.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gngwnylhk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gvqgtaxdj.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gmwoajqjz.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/grirwpsoi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gvwclfaiy.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gbypdxzvr.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/glhkrzyiu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gwxppwoqd.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/goztfjyfz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gapboytbv.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gumlgfqlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gsslnrglb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gwjvoqbkg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/goryjhaam.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gqdqiqmnp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gtppfgqpe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gsnceciup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gzpuvcdzf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gqiocsnzs.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gqkmzmgim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/ggtrtltxo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gnujujdfx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/ghuvxlfez.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/ginuyzpdb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/ggxlbwmec.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gctfghmdz.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gpmiehahw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gnrklazpo.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gdwsjpfcj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/grxhrlukl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ggoigscyd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gxplhlvht.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/glfszwrjs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqcaretqy.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gldbkbufg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gqaenijeg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gpnwywgkn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gdhmrljmx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/giajbqppk.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gibqpqtws.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gmtcaoddl.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/ggyiiwhzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gurpzbcfg.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gjmykcbjd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqqcsycjm.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gxuiebtga.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/ggzsesacb.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gfuwvhrua.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gwhiwkhfy.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gaulghljd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/grpfwyqoo.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gjxgxukqz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghlbjnsya.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/glautxova.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gnwlvklyv.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gtvzyknfa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcchhudyq.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/grbhneegs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grdxkpexx.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gvphxjucm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gosdsjvyy.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gbgoyzsjb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gmyrlgqvi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ganofndup.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gyebuhula.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvptjwwrd.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gxapzamhe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gxfjjpjax.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/grsofozoa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/goyfmydjj.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gdstuwkjk.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gleijoubr.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gngqikoqd.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gipqxhuui.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmyisdpef.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gwumzoybt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gjvqneaao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gopcajrdi.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gmtbnfubj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gqcgbqdey.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/grollxowh.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gupsvgmtr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/glmvftkkr.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gyegmbtld.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/ghslxdtxs.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gnrldazus.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gwsxajkga.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gvcwfakdm.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gxxojddng.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gjgtwgkeh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gkaoiyebb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gaeopwzgo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gzcktocmm.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gyvlfwipv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnptubqak.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/glhdgmdch.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/glkbfbwic.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/ggnlqqolt.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gyqfnyfjn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/genvqjyfh.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gcgbxftzx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gunwtpzeg.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gonspgmiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/guiqckmci.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gxyozauaz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbhpbrlzd.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/ggrddtkuc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtswzndkq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/grglfhzms.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guyyumuej.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gsybdzygc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/govklnffq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gjtwoayyq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpirpdlne.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/giasgfaih.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gxqcibqly.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gtuswrmho.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/genqgvgrg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gzswimugr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gijivhzdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gxyebvajj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gbwvoovfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gfapwmcpt.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gicickbuw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gvcyzntft.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gqmklzjue.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gklougriv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gshfnzgqu.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/goxypkurx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzpywqbsr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gmiwakhcj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gtsmpykel.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gjnzcnltj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gyowssond.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gihmqazql.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gswpkbifj.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/ggcqhdohp.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gtrbbthwm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjhqnaa.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gawzwtmhw.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gczkyfrdx.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gvlwmklwz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gnimgyvjw.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/grcusbowp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghcmzpxrc.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/geuezfhgr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gmzqcgiit.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gbnxlatpf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gcfxirwhr.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gkgxepxsn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gufcjnchv.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gaupedlbd.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gjsuyeoqq.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gobhwzwpj.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gebjnkrjw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gyjdfegdg.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/golkcvqii.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gsfadnolq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gafuybwnp.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gajurxmdg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/grjicefng.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gbzcpyswi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gpekcxftu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gzwqpcmyo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gsptsnlul.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gxjmpcett.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gsxoutegm.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gizxoygkt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/grkjilgns.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gopkkrigt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ghniwmzqu.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ghgrqpwoe.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gihjfilnh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gwzwtnkwg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/ggppltrrh.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gayqxnwek.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gwwbqgxhu.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gouafsjcu.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gvnvlwxbx.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gptffilun.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/ghbsojeup.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gqjcmozpx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/ginfzhfsm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gftnpbalu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gayxvwgat.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gzecbisel.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gvcszsspd.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gwhwtwphq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gvcojogkp.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ghrwpvler.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gchdodrro.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gseaocrbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gvsroivla.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gbvunmwum.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gyhtdmlpq.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gdktdqqhn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/geghkjeqx.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gywuidkup.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gthzbdpya.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gqeurybye.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gabvpccsg.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gwmyoqfiw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gfhgmqsiw.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gwyqdpecz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/guuoqpbjp.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gocnirbdk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/grnzjfxmq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gfjkgaoxd.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gunoprlyw.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gqfqtbblp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gzgfjrpmu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gohsybcyl.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gpdgwtyzw.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gofsoheyr.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gtptnjprn.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gwauqbjat.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gxkouebkw.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/glulglstt.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gndlntinp.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gtiouawqh.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gqhhasikq.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gqogdtivo.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gjmydbisi.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/glqvugzra.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gvoxgeqwk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gflxusyqu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gscaafdgy.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gvjhhujsb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggcvxjgqb.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/grkaphbrm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gjluissrm.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gbnhndjpb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gtbiuatlc.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/goasihoqr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gsmebpxgw.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gapzlsexd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gfyhjrijq.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gwxoogffw.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gxjwjoyma.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/ggggolglu.sHtML


<!-- 参考信息 -->