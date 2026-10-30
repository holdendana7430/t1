代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/ggprhhxtg.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gikgaojif.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghosaqlrg.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/geqyswqyu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnyuaclr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheqigvrs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcakxurx.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gacanbsxl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gcbdiaqwg.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gbniqhtva.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gtfvreahm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsanayvnq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gcwediwfs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gciikkjmm.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujpmkmtt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrkkkwhc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwxlyziw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhvxwcm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gffoffxwl.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmcjlooj.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gapbqdmka.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gydreyfjn.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjjtqrvk.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/goqzyakuo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gedlrbfjy.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/goevsvnah.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gtekxucyj.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawxmsjg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvkluoaa.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutimcfmn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gwrbfjshv.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrdgghew.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/glftkgysm.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvmixmsg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmgtnpzu.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genklifgq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuwozcps.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gzjnoijvq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohaferwv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzsgtvpl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gomqxdawv.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/grlwqrtdx.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrvndsez.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcphhlflq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gacprikck.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gekevvsvx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntixjykt.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjllhasa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvkpiyey.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpobouyt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgydohuu.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gabtmrals.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gugymrxin.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/genveuyoj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gddhgbtlp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsevkxepv.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gszqlqhaz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpsqdtmb.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqybrxxc.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmhogywt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvpgmwu.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvyehlsf.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtldgmgmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsaventk.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkldnffze.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmijuemei.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqjfefgdd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqkcaqf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/ghxzwqhos.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsosttgq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmneokch.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gijwsxujd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/govyobqja.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrdounxg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gixtytkcg.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwnjdkzlq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gtqksxlyv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxoazdt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjscfeih.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrbayxgy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcrcqpgh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcfinicv.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrxpomgz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gopsiszct.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxikcxbae.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gszxcwffe.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gyymshier.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmezferol.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/ggbsiluwp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghghstkyq.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyflssqr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjqyzzny.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxabjjsq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgwistqf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpkkpodq.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyzassab.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcnwfaybr.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gyyiozaue.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpqjsmnt.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gojmbpjpt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnefsocy.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylaeahni.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gatqbsygf.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqdeshuo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzpbhfvc.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbreyieyg.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdqdcnjc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkexwvtrq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/grcndaznk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gnulbsadd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gasuufsyg.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gfgbkjkjq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfiushdl.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gowldyiao.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhtwytpc.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gginvbuku.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/geaqrsxvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gdotadekw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpvmqhnn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guctpnyle.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gjabfcurw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqchjrtd.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gmkobuygu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjdtqvbc.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzmaqljk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gvswkspxy.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzyutqvv.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuypofzk.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjfmeqcrm.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnfjapc.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmxsnhyn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvyspcqw.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gjppvzppq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjizdaub.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gjkqjrfqi.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmcuynqwt.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gotpoqwnz.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/giyksxhsg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gblbasckr.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gqbpvaski.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdqqcbbi.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gywwgxsaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbsxtzj.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpylyuwb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwkyxndl.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzogwung.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gurvdlepn.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmhyknt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyclwapjs.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdtjrcgy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzmysjmw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gbgukpwiw.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggipagwxx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhcpsxwa.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gzndukfut.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjuahyb.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gnopfixmi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gfpinjvll.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmrwfsdr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlpcqnmy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcufuvvdo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvgjbbpi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqowxpoc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gattyultl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffzltbom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goljbcfae.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/geoixqyoz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdslodnkw.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gtqnrlcyd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfemzexz.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyucssjd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrzevxmw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gzakpzgfl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhkwuoie.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnalvvmdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjqqqzzi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gjngxeafq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/goonxawsb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhieggav.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwynhuhu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodcdytl.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gbsecubrk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigzhmkas.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyjpleqx.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwgapqenf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwggqipfm.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gpwpukcrk.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gocbiyvwh.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gnhgshipb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxcnpzh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzhimmp.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfpmhvvq.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gzgoomzed.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gllogkymg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwerrtfn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvdwpkl.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbciunna.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtvavfeu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqwqkpz.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goxbulbdl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grjjqwwxm.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvksdhins.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/guwuqtpfy.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwckahrh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvxkjuqtk.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxqechgdu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqwvxbwil.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzrbpxvf.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gliauurwh.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzvykpjs.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopjtoph.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsxostupp.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gvtclgwjm.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/guaalqaln.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggzqcfumi.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvenkcav.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneyqzjra.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxeaote.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqgvdsqy.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxaliqfkw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbhfkixj.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbigpont.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmavlviyh.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gmmfcvigo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gikapfleq.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqpwkjnx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtlwstqfg.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gowqqogvq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtfbrkvnb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcphmvfh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkimmhaf.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvclbzohk.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnkhzfab.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gitdsabrb.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvagreib.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbopkiov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsjdgfhlr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaaogbtp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnqngciqh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwkkfps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtmlciccq.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzbhgxce.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gknonvqnm.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgsrsrmc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gyjaermxc.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusumubur.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gghswcomi.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjowzlscr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggcvtztvb.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gahkyuuft.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gytlzqzmp.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtmdlyuzn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtizvjou.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpebkekx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzwpnkwy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbanrazix.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gouwvwzsk.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbindpwbm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzouxjosu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/grywfcepa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfmeihy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpgtmrwm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/guswrctra.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvukrowwe.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfokhopb.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gbbycensk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzapbai.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxhvtqt.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghbseoquj.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvajyyytw.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gafpkmwzz.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtisyiizj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/grbzqyiyy.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gorxbrkxq.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gckuniheb.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcdbwmvrf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyodabbpp.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gbgkmebiq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqrhjizy.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmelokeyw.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gupxdyhgb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gszlwflzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gavcewhgc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvpmhyar.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngrclhca.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gshsustpe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gunlwedfv.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpqhrnhr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejqfnjpf.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzsgsdqze.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggceowdun.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmicbewoz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gcenzxhxk.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprnewrri.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjdstnnxq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/giebrubxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gjuahqnyl.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gucrtimqk.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gadsgxxrs.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gzowsvkje.sHtML


<!-- 参考信息 -->