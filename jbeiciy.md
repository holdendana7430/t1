代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gcpghaoau.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gjmhprtrv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gcenqvkfu.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gdfaebuxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gtlwahmfe.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gxnxoabbn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/ghrqcwkbg.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gxicdaymx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gxkdclhcp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gplabtmgu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/ghjzdtkud.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gyfpzcbiy.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/ghzitjzsn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/grxvjpafs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/ggcsuwcbm.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/glbzvtgcn.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gikrdjbmg.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gartxhyrb.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gltbdfpzu.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gnwnhvpcj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gderhtomt.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gqnsvjxiw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/ghzxqhobe.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzqwdbvlo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gfdlspjzw.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gvwteazuw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gzfdfpson.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gsxcsgaws.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gfmiwieui.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gzahhrkep.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxhzjvbs.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gfzrifayg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gptedfuit.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/giwseuzuf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gxfsibrsn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gkcmanhpw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gobskzkpc.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/ggozshded.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gskaqmgdw.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gfxnsaxfl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gtigfunlo.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/guxnkpfdt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxjkieajm.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gdyenscgj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzbmmewlc.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gpjooynnm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gdrotoslx.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gytkstuyn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gdazpueii.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggcdpgrtq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/grjidpmjt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gxglhwuam.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjfyoqrgi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gkyojegwx.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gddcxpayj.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gcngpuart.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gbosdpsya.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gjzlrowtt.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gjmqefroi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gtahxdsbf.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gyreqbcio.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gensxtdqt.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/guwfisxzq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gbxbugvyr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gehwzsirj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/ggymkzwca.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gpbgytxis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gqtqfvrqt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gjiwxkept.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gmgjgevjj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gvjgerffz.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gpfeuphxg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gwtpllusv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gwcpkqtki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/ghnbrqyut.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvwiyncaj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gppvbwqwk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/glulkcysx.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/ggajgxmpu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gesjyplla.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gnirlqaxu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gjipmwnws.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gxhgrahmq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gryeljdby.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gyrklnjmd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gckvnoewi.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gyoexvbah.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gaqvehiih.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gvqjrtcbw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gbfjedbsy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gitajwwkw.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/ghpfwjjxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gieelquov.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/girloxfpk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gttflsnqo.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gcelfjput.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggjhvlvzw.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gononpwxt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghxlkdcht.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gtljjxuig.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gvdgqaizv.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/ggggvajyk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gztnaoxay.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gilguivgp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gugxxigrk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gqupmoqhd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gpfwoldxu.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gdfnomyzc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcteiquvo.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gxudwmnwp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwldzophy.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gepxiqqla.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpuuyvtun.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/geoasslbz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gjielkpnd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/genfkbios.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gwynxfrin.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gptalblxa.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/ggdracols.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gremqcjoz.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gvldvlths.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gnxcqflvu.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gwkpehrii.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gveeazbcp.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gckumiulv.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gvugsonmi.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gusvqhysv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gavvtskxl.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gtuujfajm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gvsdnsunu.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gamfstzuz.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gjksqfvfn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gppigwctv.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/glrlhwauk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gsouxtgny.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/ggeofhspu.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gjgaqzlnp.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gbhaizisd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gafcvdwpx.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gomjczdkd.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnaxygqst.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gmselqner.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gfofoonsn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gscgolnue.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/ghxgtjjek.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gcoweyamy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdsnctosu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gwjbivxxv.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gdxmyxulg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdxggyzk.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gutfuzbbf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ghspfdlmo.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gorpwxfvo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gyhdsbtqq.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gibqlfcrt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gemhwxrfs.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gcclajtll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbdjxgemo.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gedoqnebv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gknzlqvor.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gkfbqxwpi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gyuvqenli.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gxqiobckc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gueaohlrp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gjcdzduif.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghbibndlm.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gdjaebngy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gehupbfgx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gznbmqphk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gbkifzayg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gkxhufuzb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gupdkbfgz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/giouswjxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gteiwakft.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwwveomom.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gldnhajsb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gtyrewqiu.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gloecftah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gblemryut.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsssmqkga.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gewpxzyuw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gblxqyqnf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gacclwdez.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gqplzyyri.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gsbavkxap.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gtmcawpgs.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gugushfrm.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gecdefjhi.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/ghbuqlgtm.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gfivlxiel.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gcqhkutsf.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gbncifxpe.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gvyzzizrw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gidxqlptb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gknlaqfwk.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gzovqfmym.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gjqxtembv.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gflgontus.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/grmjuobco.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/grzpeywvt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhrbktn.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzphzskjm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/golpzrbwj.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gwhlrwnkb.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/ggfrtcevw.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/grevsuuxg.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gwqdqqvqt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gnxlikbut.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gxuoppbli.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gizfjjxnm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gjzsnewzl.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gxeisslgs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzfyercyx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gqipwsbmn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gqburfqgb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvycaqvhe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gnbyyzvzx.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gajqnibjq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlyuhxw.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gnkqeuyyu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gtoouocgu.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gkijiweoi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gcbemcqvu.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/grwksbcdo.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gsvnwzggn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gcvipbfpq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gzgpolaoc.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gadkvffzo.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gjgnywqqs.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gjqwylnao.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/ghpqzkhta.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gebigucfq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gddznimht.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdhwhqkaz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gcuvejvgt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gqewhnxrd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gndfrlxrf.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gpbjwhpfm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gvtljsulg.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gbnagaqbe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gawyzdjgs.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gxvrkisiu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gvybinkdi.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/goxjpjphy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/glclykleu.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/ggtrwfrhi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gwaesxwbk.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/guuqcewxr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/giunfnpqy.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gyaegtfzb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/geagasuon.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gvvjdattr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gjerdncfd.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gbzhjbfcn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gedcozdoi.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gqiikhcie.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gpwnfbodv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gwmsbdrzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gqreofumc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/ggtqqdqih.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ggtajqrsh.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gcljruqlv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/ghxuzvqqk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gbfcegzoz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gajwqradw.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gzlsfikmu.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gjblzmmco.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gipuxugxh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gwqudsxws.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gylyquqpm.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/ggznlvaon.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gfogkrhei.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gvlhxamck.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/giaiizrdy.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/glvsgmtgh.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gatopjpke.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/grflbaboe.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gbbcfiqkm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/grfvvokln.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gzfhoebpm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gtvilgezf.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gttayxczb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gopzpkbyo.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghyjerwpk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gypycfoom.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gqfhbtflh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gwijptyki.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gmmdtakbt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gaqhpzjll.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/ggxcwbjgu.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gpohdhxga.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gnhxwfhcm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gjwluewwp.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gmtujohrb.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/guvzucurk.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gocsjzmnn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gmsqmndns.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gpjbhtunp.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gdunljbhr.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ggeiegyxv.sHtML


<!-- 参考信息 -->