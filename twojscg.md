代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/groutwmal.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gsvqlgmqd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/ginwqnueb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganzkczly.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmpkcplz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gdcnyefqy.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgjfsfsk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkxkrynu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/ghjumnorg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gvavhfnrv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvjnhags.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/glymrfnan.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqnqwmlim.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gicusorns.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqlitewew.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvjuibvqy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxlqawyh.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqyfzvrh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyepbwhry.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrlmmge.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gireljsdr.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gussfunpm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpodiobt.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gdqlswola.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtkfrxz.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghpuingog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/glnlitats.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gdwtwpsxg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbpbbjgv.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guidmemps.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gawjmdmnv.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gjsunahix.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjionoyo.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gtorkfzuh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqaqqgnfd.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/goqcigeks.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzogzkruk.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/ggxucpwky.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkhajyof.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gesvxzljw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxvukqqj.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gthlotmal.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ghiafwxcl.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grbsbnulu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gygcwrnlc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxqapatar.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzvyojpy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuorcvbb.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdzmyxux.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhffhrcu.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtpevlju.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnmjfxyy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gqfdpswjp.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtslqamoy.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/glgbgaksa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfazsoqk.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gibcnqiie.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gvdujngtf.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqdqabxu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxtufzdg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbhmncdj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gajpeqlxz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdplkukek.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrwqxuts.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmawncmq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gpsopchri.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbyjnpwt.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gflufpaqq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsigsibaw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/grrlxjvpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gigpfogia.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gioczzgsi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcanfksq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gzumwaztn.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhmpanhs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxutwkzla.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpcubqeg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqgnybzv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshqbkewm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gdvymeeti.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghztdsamj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyzuvdxt.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmkcfbyww.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gdgbsvrqm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxdnfbgl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/grunanyne.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaezftxci.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvehhmvjx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrljtzvy.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gmcuxxfoq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/grwulalph.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gegnzhtoc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gohewtdpa.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/grgfsldeo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpxnrekh.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gevygurfg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjvppeb.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gaejvsdtf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmovirkgc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtatmclav.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmyttjgz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyklqoxhr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbzklzt.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gamhnttef.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhjfethz.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmtegsic.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqchxleyc.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gedblpawq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcpbgdwa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gzwwhfbic.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkcuuksr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuuttrbt.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpocobjs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwnovwwr.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/ghegfcprb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzztowuuw.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqewckfvt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvockwdjt.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/golcamxvv.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gkdgpeyfk.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqmbrvpf.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbsjtzzy.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdyprcwe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwitqxib.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/goamqujfs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gpyafrjuf.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gbdchedjk.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxrnxwwm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbkktctt.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpiibksn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxjjjjoh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdnvnxev.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzummhvl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddupapvn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/glgsmmyal.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkvrfuzx.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkmzudxc.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gutnrxmwd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gexgoepjl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtidkrkvw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghclyjdvw.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxqcdjvnu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqekneyk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwiaypfi.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvnchevl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/glmjedthb.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gjftcagve.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gguponpqo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftsscigk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqhsaxbn.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwlsytit.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhvxmxhu.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvybktpa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gylspxknc.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgokgqqk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwsfjae.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtmadubn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvvbvfvr.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbozorafi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwzojds.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gsxvihblx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goxcqubjr.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliqjcuhe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkszyfgus.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gyhahonsi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtobyeulb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzecxin.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpxnlicy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/glburwbce.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gxakuzeyj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gccmqlbnx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcnxkzbu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gpxooqwkv.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gycstnatb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gireycbhp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuujgssy.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqvjqbmi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprdbcwdu.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godwmvuel.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgsbsjmc.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/giiudkclb.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gtubgkhkc.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gkliedzlc.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgzwauxh.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gltqscmgx.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/goeunkfix.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjwekktm.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtwzusam.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmqpooajv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gapryrzrt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhmaslul.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gftrzrens.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnldzwtqh.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfukormwq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gambknaqo.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/guyyiviou.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gztgcsygf.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscijxdjf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guqhhornr.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ghmfliihi.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/glplfkpto.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsejkjig.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvibsyjxx.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwhdpbchw.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gueccqngp.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqsednwb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyeqeawy.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtepqdnyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbnnxcdq.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gxspvahrm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gypscsfxn.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfocncnck.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiqqzbfw.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwytiuw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gngywsuqa.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/ghdkgblds.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbffnylh.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gknfehlag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gevaazsgm.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuretsqp.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqhfoktf.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gcakczaqm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjswngbd.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvefsvni.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjcrlejxz.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giorvdezw.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggizjhrus.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsniuawlm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqfpvzfm.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhmefjir.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gklmknbzj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzurqerjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gblyulgpk.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcltkqiqa.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsofmnlqx.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gauaizasg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqxfsxyc.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gildzgoit.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gduykjjoe.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzfedxxz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpntumyob.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvjqunzz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihwpqlnx.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoyabtfb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonlmehws.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gyetvuolv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgufmafy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrmwwtdx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/geikqdfrc.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gthnmuwcf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwgbsoyy.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglvezrdt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gccrbyzfm.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjojzdbjw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gazcfopaz.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/goffzypnz.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydtixinb.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwfngebt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmzygyrz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/guxgvydss.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgnicexk.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ggmqcspca.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhkiadgm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmpmfokb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnfbnjmh.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glckjcceg.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyouqfdp.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gudyghmyi.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwriecaq.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/goqbwxrvm.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gaazpirsw.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gofdcmodr.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajwvttjb.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gwrujprip.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/guuouutnr.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjwjsrfkn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpfbvqdh.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gejgdbgpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqtzsfax.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxtvyvwk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvuawslk.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjudzjor.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goosrhnmw.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbfxxmvy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gzfkrcyaw.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmcofqnh.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzciqguxw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdwfaasn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gzhdgujfp.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpadprvxs.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabqjmgd.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gdwiibufr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gkixalwlx.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gquubimle.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtfmfstz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqrsdmlt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govmfakxo.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjuqena.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjdllasn.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxfojoqk.sHtML


<!-- 参考信息 -->