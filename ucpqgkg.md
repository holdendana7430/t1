代发 wailian999

);
来源：http://read.share.fehbvm.com/Article/details/gppsrlmrz.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gabxgdzjx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gimbudfch.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gwmckkqsn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gxujvlrxn.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gdercazgu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gngpwxmdx.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gvzxdveyg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/grgyqbasb.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/glpjector.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gnoqiyutz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gknwpwyhb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/grjisptrp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/ggzfldcae.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gfzxuxnro.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gixkzutyr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gmlwvsxyt.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/ghrondyvd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gebppvrif.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gvtlzyhmy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gqvndwnxr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gnxozszzo.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gaifxygib.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gyltadbek.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gyvoanzhs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gnfxtiuzi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/goafhqpwt.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/grjizkgdu.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxldamxyn.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gnyhbeekv.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqjyehhmr.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gvjlukquy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gvzwvuajl.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/geqcrtobd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gzqhofqvr.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvgonstfw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gkhcpibzt.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gmiojbxqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gqvcubufy.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gupbezvpo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gorgcdrry.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/glffrmrvb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gynazxmpf.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gwhoxsbrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/glmijaaas.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/ggqxkmifg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gywiklvzq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gtdeircxz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gouwmflaa.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gjtyxcher.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdwohpyzf.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gsbgwqntb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gbomwhepe.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/glgxvrblk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwbjvionm.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gokebpfll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmoblfyys.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gohvyjqoh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gvzbsdemg.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/glrslpdoc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gbrqqomob.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpuvqnitq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ghtbhonlv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/glpjpzjbt.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gextsjoco.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gpqsebnab.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gcrzrgzfw.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gmtdzpbmh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gxvsmorkv.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/goaoknkek.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gmjbporpb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gctksgwcm.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gwetdhiau.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gpeaihbdm.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gqolzzlgo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gffnohmgp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gettjhxwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gxcmrantv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gcpezfmgf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gdweftamd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gufdxzwav.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gvmpurgfo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gpgasotff.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/grvyebejo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gtrvcsdtt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gtevgerxa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gzkgpmkwi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gedwgqlgu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gmbjpgkpx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gwizgybey.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gpqvbuitj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/guybxcvwt.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/geezbgtti.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gkxjxojlq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gyqclwueu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gefdtaxcj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gckirmarl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/glshcfsyl.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gpwbivdrj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gmnmvbfbj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdbkptwhp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmkkkdgse.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gnykrfroi.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/ghsoaqsfp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/geygeklgn.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gtldcyyqy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gnekyrgzf.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gslcwajlh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkypmhhdw.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gkxkfpznp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/glcbkzebc.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/godgtizaz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/geppepppq.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gzqsccqcg.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gcupwpmmy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gbwaltwna.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gyhvytnqp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gxhbfazvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gmwcztvad.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gmemqfrcx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/geihphqyd.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/glxpqhwsg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjcbmmdie.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gvuaoooeh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdjexlaso.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gaskqdwhy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/geuklrken.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gevmqycoe.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gvbkooykr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpnfffaiq.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/giooienoh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/guezsluii.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gluyzzjwn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gydvicdje.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gvjywuwlj.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gidouipwv.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gcwrgiofa.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gytbxkwnc.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/glfhtsrap.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhkuyrg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gkhecipwp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gpdndqqla.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gddhlusho.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/ghofmbupe.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gkqhqlbgn.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gumpmqifu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gumwyoooo.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gkhkfvecs.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gfibbxmtp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gurquszle.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gmtjjiifz.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gmvgpwoqr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbdacnrqp.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gjqsmizsh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gulshbruv.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gvlregysd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gpcbwiwau.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gkktioame.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glaorydmq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gibugrsmn.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gpomsvnns.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gxtzrkjdc.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/ghugzflcw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gerzrxzwd.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gmfaidmjj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gdgwelnzp.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gxqhsgjgc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gwerwwtfu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/giuzndlyj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnuydewai.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glibylgdu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gduqttgne.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gzbelvbiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gonkpxijx.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gfipmgyqo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjwlywuph.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/goobzrlnf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxmdpeddt.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gjtcbntfu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gsdigspnz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gteauumdw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gqhcwdlna.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/glpguqjft.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gkevkemfp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gpyheyhyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gcyejakgv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gifgqtixd.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gufznjoon.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gdrdvzrir.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gargwkoob.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gqybxyvay.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grbnhjliy.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gjkhfuxsp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnzruqcte.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gmtjcgjsb.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gdyrfputg.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gxxumrwdr.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/grvqwhfop.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gmjxerdsx.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gvhvdursr.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gzgodpktw.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/glysucyxg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gkvaljxjl.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gpsswudqw.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gpvlxrgxl.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gifgllmso.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gvmuvhmor.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gotovgbis.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gdlvgxlst.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gykyjbgsq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/goimtsywy.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gedafrkep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gbdoyyaut.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gzozsyltn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gzvowulvi.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/ggtnbqeqv.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gygchmeok.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gufhbbquy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbrwhczss.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gsutsjzwm.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/glwaviore.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gxvrstfro.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gkjkhsdny.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gbgrrkpli.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/geietvrct.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gzfytdxya.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gtjcngklr.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjnvpxlqn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/glmwssskk.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/glbwmbsed.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grcznslpw.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gizustleo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gikyfucti.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gnequwvvy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gwmqdgsjc.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/glxlnqmub.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gxvhmzynw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gqnlmrjiq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gyyhhyxcc.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gvgqxulet.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gbuutders.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gsphlkahe.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gmvlmgexy.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gtbiadici.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gjrzotybf.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghjtoywmx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gcuwmgoqe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gjltcrayw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gggkumgix.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpvwirg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gtjqsdgbp.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gxugkcxef.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gowpxwuzb.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/glzyzqofl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gypqzrthl.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/grpjvukah.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gssykeldw.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gglarmble.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gseyhprqn.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/ghjwvelkd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gojcplkhf.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gtdafhvht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gphgcprzx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gcphpktij.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gtxjgkzng.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gjmoloofo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gbmbvnjdb.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gpbfhpzke.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gbyvdskdx.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gwzwxsbek.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gyrokedor.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gzhvdawra.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gwzzhdsrm.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gcdefzjro.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gzoipkegd.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gbrbgahvy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gbutmyuma.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gmrhtczof.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gjeiypbml.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gxjjddysp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gycwlkkpo.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gflsgybad.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gjsrgbxbd.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gqfdndqol.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gbevmjkzz.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gsilspsex.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gulzsayju.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/geutliaii.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gdwmlerwh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gsrnhveoa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gqsencmzb.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gtsqipkcl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gywhsiuhz.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gqjuvapwp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gtgxvsahd.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gbkshxmxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/ghczstlhg.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gfwkgkwod.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmucjvqdw.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gimviwbwj.sHtML


<!-- 参考信息 -->