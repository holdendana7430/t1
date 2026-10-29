代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/grflqkiue.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gymxtaagp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gbcbvwlno.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gfsymciml.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/geqcfbbof.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gduicdcgv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gzexrkaqv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwvfpmwxb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gaierdryi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gerfdzjcs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gihmczygv.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gruadxspb.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/glolbyilh.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/giqexdiuj.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gpaueruwq.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gxxbhvwpe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gplmqskjt.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gtjtxjumt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gqrigqdlo.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/grjwdpuri.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gkyhktasq.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gfptlivan.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gzpohrsag.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/glhkrkkwm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gdpgnsurg.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gowtasxsx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gguomtlas.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gakdfktel.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gdwnknajx.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/ggsofkplc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjrfehcfc.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gkmtturhl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gkruiqvxo.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gbqpwunej.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvcvkzybm.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gljemvrwy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gswcieimz.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gnrqztrxp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsaewhoxt.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gisdtgjcw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gneqbqsjr.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gwviknnfo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gycvyfxdz.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gncjnmghh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gvcpmhczj.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ggqbdzkgw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkkuamaty.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gzvneyqkv.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gbihykifc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gydtoaxoe.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gofwbsyav.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/ghecejbhx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gtywheyoc.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gtmiambhz.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gyuiadpak.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ghvwbzvfg.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gqyqzbbct.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/guwvfpikd.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gasmdfkuj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gwijfcjcf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/ghrrkhiex.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gqeasrxjd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/grmnotmeb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gmhcwexjj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/griswzpmd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gxqczclpl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/giifmysbc.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gaxvkqacm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/graoaggqw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gxenfmrdy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gcpurqqna.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/ggvdegncc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gddjlnxjm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gjcybffws.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gbpeblyfu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gjxpwnjpm.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gfcvsornd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gbrzpqltu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/glvbscrdy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gsnbihqfl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gvrfgseba.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/goynjrlfk.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gczbakoyx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gxwfxwmon.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gpuukfpke.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gplptubiu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gfzjcalrd.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/glgullfve.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/ggryjrlzr.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gyinprafj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gdrlfdtvs.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gvrruhuvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gxbzgtytn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/ghjvrzuty.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmyswgsvp.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/goizsfudp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gpgoioblm.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gohnrfyht.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gxlnhsbcs.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gvrnfjgbt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gcovlfgol.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gvmhgczew.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gclsxuwzv.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/ghpbsqfla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpvnfxebk.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gbaemaipd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ganjeyqzu.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gqgztoadl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnnhqwsyx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gpvjxuzlz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gjafemhfm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gppxxhqde.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gccjyqbgs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gedtpzoeg.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/guolxzmun.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gblcdkweg.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gkffyxyui.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/ghgmfjyky.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gpyvvpmqo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/ghgccqvuf.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gsmbiaggq.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gcfsovujk.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gxlftuvws.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gqyjyarcc.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gbhphfqib.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gblvdzpnx.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/grayvlpnq.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gtwhbnjgx.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ghugcqesv.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gmzxdtycj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/grqwecutn.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/ghdukkikv.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gyaifvfok.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gmbqhfojj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/goiqngeds.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gliwzczyo.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gahxitcpl.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gfjhycdfm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/giywkfemz.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gdgwilacg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gpibmgzef.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gndfsvwtr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmdcjlicg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gvcnzgsor.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gidnpkbrb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gzmtoqgpw.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gdphvpoqk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gwuoalhmk.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gnbxnzeez.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/grqcorfql.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gnooelmzc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gpanmqczs.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/ggcjxqzoh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gihwnfxnj.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gisxlevnn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghmmbcirq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gavjyssua.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gikktfvbm.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gvkohxmab.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmqkylfcy.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gsbnpjuwz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjdfqqfoi.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gnusqadas.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gkexrqfwm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/ghzapadch.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gbzjrifud.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ggozqcxvk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gbdzsaqbs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gsuduchxg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/ggogfduaa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdpfllxtk.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gjpvxbmrb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ggdkoixvl.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gckwwtwif.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gnftiiyrk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxctwbdil.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gunntshqn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtxjobwrm.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/grfxoxdum.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gebiehzgf.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/grbjmwveu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gzwogkpkg.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gddtkmczj.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gjvsoozty.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gohdrwned.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gklzwsewl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/geiinjvjp.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkdfwxcyw.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/guadazjkw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzljdxozn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gthaxnkvl.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gdxnjxdba.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gumlormzc.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gsbdoiona.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gswwdufxz.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjftubpgi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/geersdmhm.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gutxaprhv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ghossjyhk.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/guomhdzph.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gmorfrqee.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/geofuvxyy.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gojlspamw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gmwtbeuey.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gmarjpgjm.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/grhykkiax.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gaplanfcj.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/grphkmlcu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gorlxrluu.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gyijmccdf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gcxdsqwlq.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/grghauwxt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/giebcjmtm.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/ghmounjvn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gtudzoxud.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/geskmzlxc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gqcnhkbyc.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/ggquxakgy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gwvmbonjn.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjehmgtff.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/ghmkiutkk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gtwvvyhxl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/grdthqqsl.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gzolniovf.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gpqyezemn.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/ghslzskpe.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gexzkxjro.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gigzuynmq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gvibpmlwf.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gtuzletrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gwaztdovm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gzegyavcg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/grteywnhg.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnevsbwel.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/grmvwnsxy.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/glciyboof.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gssomthzu.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gncgmfhgb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gtplsjwba.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gtgglsqhx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/glkqparbl.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gbkmxdhaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/glnsxwknr.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gdveucxqt.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gpfabrwdx.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gkjpnpzcb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghhhhpehr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gpoxetbcu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gfybnovyv.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gvbdgtbji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnmrnvcuy.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gfncnkflu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/ghguncsry.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gdqdlwerq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gkpgkuaqz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gnwxkyfok.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gyfttqtmn.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/grhzyhaac.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/ghsnhmwcg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gozknksfy.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gmnpghidp.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/groivhgkc.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gibrsztol.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/guomqhtkp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gpxwrjziv.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gislfcslh.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gvbhfzbox.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gownnorcs.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gxxmvkgmh.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gebihmcrk.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/giptseehh.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gojinlvsi.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/ghfjlgwuh.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/guxazdpfq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gthcgdymg.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gkpxeachb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbrdatmme.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/giqtxfkrq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyyequhzq.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpydlhbfv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gchwpevxb.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gkbbiaxus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/grmncxkoj.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gbgodmhlf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gnfftrhle.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gkprrpyvp.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gzilnxnjn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gibapoojd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gdkyjwplb.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gwdxqigul.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gbtyppngx.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gyhuhdnbx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gjzmeihgj.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gccwrviho.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gycgurrgu.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gvrfaiono.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gnwkzpneo.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gsqlelhdm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gkjhlxmql.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gnseoxwxr.sHtML


<!-- 参考信息 -->