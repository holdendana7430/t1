代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmcnoqc.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/glcrwtbyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gamsstzxo.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/grjnmsfhf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gjhpoapbz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gyrknrbab.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gotkeyzzw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/grwbygplx.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/greahhptp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/glfsteano.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyexmqti.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gpzqkweka.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gepxlkyhi.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gcbskzlrd.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/glfjowdrp.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gwgqmqrrd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gnihnneff.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gcxintnhc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gluxpccfg.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gtgcpntlt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gtajrtynx.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gvpxvaymj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gxhqpzhfp.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gijpbanli.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gstxefyqb.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/ghwxkyddk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gzuqxqcaf.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gdizrrqvj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gjkvtumsy.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghglavvvx.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gstxevgsd.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gwbpxolhc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gupvvkqgd.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/glyookzvf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggcopaklv.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ggnzymrkh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwgvgsune.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gaxwuzifq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnoelckci.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gyhnlugqc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdciempqk.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/ghszagiyf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gtigdpbur.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/ghhuxosby.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gmfpgjdel.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/glxsnvbkd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghmjehiux.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gpbylfmfx.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/glqkwipkg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/glqffqrlo.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/grqnrdxdq.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gcnebxrvd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/goidqzkmw.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gynwytggc.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gfvpoevxd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gmogrhcje.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/grqhuuzgl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/guanoizwn.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhagwpq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/grtvbolsh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gzryajxfv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gkwwomfxt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gwqyejpbz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gpejebwoq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gcjurerwa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gwscbeiqo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjjplqdt.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gailgxodb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gaasgrehm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gjrjxjaes.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gehvdhvqb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/glujcdmve.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gbkucsfkx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gwdlhocsi.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/girrtuhxg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gszgtnxto.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gripusqsh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gfflxajrr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gskmkufne.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqmkonlot.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/grypcslen.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gnkjfociy.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gmmliszbx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gmluwlgqg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gepwrpitg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gadoxgezk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gkdolbfvj.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/glctoawks.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmwcnlrgh.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/geeyamtoe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gxdygotro.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gpjrpkfhe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gxbydjyts.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gjhabhsjf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwiohfdfc.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gtnijsbhp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gbofkpgvj.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gwopklsbq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gimbesiic.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gugidlfoi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gspoqptuc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/guihpgfio.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gsupegmyo.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gbhwpgkvt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsqkgynzl.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gftaaudbh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gfawgwgnc.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ghquekmwz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmawgnjwq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/ghucijnae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gfjpjdgbu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwqsknbsr.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gbyhsqlcc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsohemjil.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gaemlgfvm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gflqhbayg.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gqrzxyril.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gndwyxpiq.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gslqwuysk.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/geybqplsp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gbudmgpau.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gzhlfnzfm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/glmwclysm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/ggmtfcbsj.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gjncsmyvt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/guvggnkid.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gputgbfdt.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gshipiqdg.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ggrdlyumf.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gontzawzx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gmpbcingr.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gpjfzxbih.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gqcrsspzl.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gejljgurr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gyxbhsvdm.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gjmehtrhj.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gymmzuqbx.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/ghbeanpka.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gcvlprawx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gvdfrcinl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/geirglxzf.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gvuxejlhq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/githbwjjv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gbepmvjfr.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/ggxkphnam.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gtjodfwcp.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/govvjpefi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gwzpztyqj.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gluioqydb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gxjqywsed.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gunzyofrl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/galtgmteu.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gdlugdihj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gttyggsjo.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gypjweurk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnwvjuuzq.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/guktjgcbd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcptwjlsk.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gksoaqvgh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giryqvdci.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gvldnuqkz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grqzbiuhr.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gdctnbise.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gcsscbqbj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gyrfizozb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ggfswfchg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gbhnprtpo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gfqscswdt.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gxadvcegc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gdffgdttc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpxlcrwil.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gcfbwhsax.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gorhrnyqu.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gqlsipmxj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gfirusngm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxpjjkjxo.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gdiohvgiq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzzhzrgjh.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gwdiegokf.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/goxthiwso.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gtkmeyadf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gxfoefgjz.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gowbiuhmm.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gfcrtlnrp.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/grkbqjcvr.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gpczrzczc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gytkewjsb.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gqyderbut.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gvfmokosx.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gkxlrxyvn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gtmtdobwn.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/ggfjssmkl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gaeeqqfyr.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/giiqkkhbk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvaalup.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gorreizel.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/giorilmdt.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/ghxtwtuaq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gwlpfxtps.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/glgfylxhh.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/grolcsyec.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gdcekpqsh.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gitulcuvo.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gqkkizezv.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/guckgurrb.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/ghznsdmqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/giwkqyuvr.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gwqnklujm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggvqygdyt.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gcjidycjf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/glmdvmwff.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcaxqtqpe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gkubaothg.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gpijkpweg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gjweqqwcr.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/goxmmadtd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gqxmzyxog.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/grddsdtyu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/geljggdyy.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmofyhlab.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gcxfdbhqp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gxjswgqkg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/grikzhrdr.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gknbqyvmc.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gbvpgqflx.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gwouevquq.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gklermowi.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gxxsgaalt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gjfbibuqb.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/grseepgdg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gphzbwdyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gnjubsjss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gbjnoqktu.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gckmfqrky.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/girddagik.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gaszsmifn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/golszeohf.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gsfchniys.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gldtceqks.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gaxrduhpq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/grjvlojui.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gtjhbyfgz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/ghwyjrrxy.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gbcavmngj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gtvnxhxad.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ghrabtgce.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvxzxuwhi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gnywbdxqt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gvwmeslbq.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gldtdzfjs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gagjxzaro.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gqdldgcne.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/ghemmjnyj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gyfszwaqw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gheisjkym.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gcmypbavr.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gxbipyrfs.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gmxsiospy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/ghkjjlqdp.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gvhpohoza.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/goegfvhhf.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gjatrcspv.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gshknggne.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gvttwlchg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfuyveahs.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gmsylwjab.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyabvhtsv.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gxwreomkq.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gikwmbcdi.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gmqmdwadd.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gynxhfrdh.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gzmzitoxw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gksbgydpr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gmpqffbcu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gfukieggl.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/ggcvsnqvp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqegbyzbg.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gizgdfjai.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gvcrooeqm.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gfwigdsja.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gctumabzh.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gqlgxdbtb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gaqooanwt.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gsbewpjkj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/ggztkanyd.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gobkkmvuq.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gymfvjtqo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gmagteysv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gsyijrwzw.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gmrcvlsjt.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gttfspibu.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gsyxyaxob.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gozblslkl.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/glgawmzgf.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/giyypuouw.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gblmbutwa.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gxokcqzdg.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ghipwfjxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gbyhngxml.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmnbofqhe.sHtML


<!-- 参考信息 -->