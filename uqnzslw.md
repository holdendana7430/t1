代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxpvdrpt.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwibmybdv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grvjovfuz.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gswxzmeub.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjtmrpc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqoegpkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydddhqxp.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gbcnvjrnt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gupptwpbe.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gecbnzkrl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gdbvvlxpt.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gpdgenaeo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghywpiszz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsbswcob.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gjbzronww.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejcmdqd.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqzuiheq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gtndkcvga.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/ggkhlntcq.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gcfumwdpv.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkqmnrcv.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamrwptks.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjpeljjee.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfemlsjq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmdwsqnt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmusguwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuvnxbzl.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtodftow.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/geycwgssv.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gchmhyxlb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glwcwnsfv.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevkulflv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/ghblksgha.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpstadoog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gpivzucux.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzzyxdro.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsgfrywl.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnsggavv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbefdgxjd.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwhgjcq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gdytfiadt.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaunyezq.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmwhxntvc.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gafsohqas.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmtkzfgi.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gamwunxzp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcrywhsx.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/girdezjao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkvpciiu.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guecenzpu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnphohis.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gibasbekt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ginavpvau.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gutfoxdtr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfnhnkbo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gnvdxmqsg.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/glnhevumz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiedrvjd.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gujbbtvel.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gffcvimcx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaseforx.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gssorxuos.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gurwqzgnw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibepjubt.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwcobdt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtridlbnc.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwzpnevfs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gmlotwntx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gmgfgxnvi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxnfosay.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/ghnmgpwob.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaolggvj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlfdgihu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/guhfxpsaf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gsyumxesh.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjoshfpn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gcppwelqj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtqysxqs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goglucbye.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ghwiiagtn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gffzjvosk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwggwajcr.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsplxuxt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcelkhcwk.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/golnkxcre.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybubwvy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiwkfphe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbrqhxph.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmplufgr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/glgougehz.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gabnezshu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gfnchvrtm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghzyyxrkh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gduenjzoe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiysbqvk.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbymhyzwq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzaakrvk.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gtulrewrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gemvaauvn.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gajchcuqn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpkbdlbp.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gpxxdnuzq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gpokkxqrr.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gvetwmmaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/grkuxdyba.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjchcaaqs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhnrhqos.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoouahwp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gubvmcaoi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfrzvmg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxgxloev.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybrmrtfi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glcnalepr.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/guvstzzir.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytadjcfm.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmofstjwf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghswbjkor.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnnooewt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqntksmuo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxocuqbv.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxomvinz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgvfsebd.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdevbtywz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtwmbnd.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpguizfa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gtrtshwrk.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungrttvn.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqbbqtr.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfxcjcos.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgbcnzfg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftyloirf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/grnuknqsu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtgktkta.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsgqmrxi.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gczmurmoi.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grghfghyq.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/grzzkfcxk.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvczwwlx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gzgjiitmd.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/geujuybnb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqizusfo.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjhihfsm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnqknpql.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gqaobruxi.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejqprtwa.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkuujowo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gowdwtzrf.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgshgrxj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsdstpao.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ghguqfapw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnngvruii.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/ghditgrdu.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/guwuzlebz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvenexze.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gxsxjjufh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gpuktcheo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvphxrdk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gzklfbndx.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gffkknlfi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwzzxhkb.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gekiglkki.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnmuempj.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtchvkyz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdyoorhwf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/goufdcdxv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpiinvaag.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geruqjmoq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdctlop.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcywqwvww.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmavzozpa.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gsszdnzch.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqcxshdw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwpzewfj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghikcozgc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzgccdgd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/grkvkfuxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gvhtlnqad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/grtyrmpxw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwzgpend.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsygticih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzvhdeom.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gvtqptxhr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gltsdkgdx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gragibhev.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ganjeglpp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwpkkfim.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/guphnmhah.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gzdragmwt.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbehpbwsj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvghhaxgc.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gyovbnkdv.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmngbcqor.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/geyuxnkqf.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/genrripjx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/ggwshcgfk.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtxuxowa.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbtcxiqf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjyecdyy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpjtmloq.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxifdlnve.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjdepmk.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gflunzdic.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtczvppad.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gawjrimnh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grzyohmms.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghaygevwc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/giidaxcat.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gebaooera.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirtryck.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoaflrzp.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gmlrpkrtl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyotvyrn.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/grmivhafy.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqehmejov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsedammh.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggvfzoqqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsfejrax.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gcvcbplza.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyyvozepr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecxxlyzn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwmujalp.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvedrygyn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrkcvztl.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjjnavtm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gspdovixz.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gvgvalujf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbecjtlmk.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiopsvqp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyajteij.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gspdbcipk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpppklmva.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glowuczcj.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggqfgyyda.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gelrrbyvc.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghyhfiiym.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfddnwkyp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhyvhfjx.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyujvapll.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqersuapp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gxyzayihn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqetbsbcm.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gebubspfy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/glqzpewfy.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gxurjkdih.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/ggqcougjt.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gznjduomy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gxsrqncbq.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdzychvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnvrxtgkp.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtkpklvi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gjsshbcua.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwignfbkf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohtqcldr.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gyoojydur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtnigsfo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gaddxrgxz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gucycoyss.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdlkzxj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfjmuysxq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/glnbdagmm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvkjkzln.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnledpeeh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjowusu.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzfvouzld.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnozyouzt.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gadrqqeix.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklputoec.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqijyzs.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcademion.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggudhliiu.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbugublg.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwgngcuti.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsdtknpgn.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gthepdyat.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goewhqaxt.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbmvzxay.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgmtjdvt.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gswcalegd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gkxipvrfz.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gkxkjnkkq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggovdmynt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/grsimdakf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gnqgtveno.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfwupqbew.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/genfvbrjg.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwfygbnf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnenuedso.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/getafjdor.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gghhgbynz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrcnmzrg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidkoifzp.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ggqaiiqft.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/galsfssub.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjddnrvcr.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqtyqokve.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/geoentrpp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdedhoaqt.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpspscrw.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/griqousno.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfmkgovu.sHtML


<!-- 参考信息 -->