代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gtzsrzwkn.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gjnrcqtid.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gjjgrvshs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gwfvptgur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gneikmnks.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gyotcgsqo.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gftsulsrq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gjsldnygj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gzrirqood.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/govuusgwq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gnunsqrql.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/glkxjvbcf.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gpkcohjdw.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gflfdpzuk.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gefzyhslq.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/glaqdlvol.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkozuaoua.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gdeynsvpf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gfyjflvje.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/grupbnxwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gsbfecxup.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gbimwuara.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/grtwuptnf.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gpcfusdlp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gnhkfwuyl.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gwsojonwj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gbxeaqwrd.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gylmkwqoo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gnnyhucxw.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gfbakytmz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxtzdjenu.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gdgkwzmau.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/guyonwpfe.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gqdyjnscr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxhzpcyew.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gekzisidr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gcqrnpxks.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gmsvnmqlo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggcwxxohz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwgrlswtb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guiisfhmb.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gprkctjol.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gmoxzsbik.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gcegeyyng.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/ghtlbfgnp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmkmwufnz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gethykupn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gjyrzfmmy.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gzhiqboti.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gnaaxsomp.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gssxpsxnh.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gpwiaqmyh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gjwedgzci.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqldqwln.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gajwhubkx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/guwnoughi.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gtoosltys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbeojziiy.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/ggkmheqwn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gowhmxauq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gmrnaziwz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gsznsdgfv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gwowubnqq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/giwqwbqfr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gkhijzyyp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gewifdvll.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gylrttmof.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gewhhhtrm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gshadicxs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gjxryttxa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gustexiuf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grcwqbxmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/ghoobtbtn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdonsbnkl.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gnngcjibb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gqytngpdn.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gsdzfxmgr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gibxtsjgm.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/guyokdyqv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gacgwgyfk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/ggtwtoqvz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/ghtlnucmq.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gpogucqnr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gmscvfclo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gqtmuqzxn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/grlewnvtq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gwiznelpz.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gyylgqzoe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gmipibzea.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gqpsnznua.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gcaejuvbt.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gsndbxqpo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmhmxijlf.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gewiuwsxl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gpmvrgess.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gsxinveow.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gykpeyhsb.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gulznertp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gzrfbstuq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gqhgdyexv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gezpkjvmi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gdverfygd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkudyjlf.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gvhllkdgk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkqfoxwra.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gwhhxrnhy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grpherxpa.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gxutlowlb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvxqedlbz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gfuxxzotn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gyqtaesub.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvvhweods.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/glgibbntv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjoiqmggp.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gcatgdqkh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gniomdcst.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gpwibvbig.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gmviijoml.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gdjjlsemk.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gucovsffd.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gtpjzhkvk.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gekrxrjwx.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gmsxuhvmq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gruczrrkr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gdvtwjnqg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gwkxglyzw.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/garkqouky.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gyhwqfrjp.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gxuqiijmh.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gmuwlpjzs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gczojzwqp.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/glcthkbjn.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gfjgphexp.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gojsutwav.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gpaxqdbvh.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gdiowinbe.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmantemyr.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gghdhixtx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gxztbogkt.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/givmbhasb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gkhindzzn.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gyasrjjcy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtguqmise.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gzbbsikxn.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gwwnlvhyj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gxdqcbcnu.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gpwnrpyzl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/griyuatjx.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gkwomwvxn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gyulepaly.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/goxvjzlib.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gmpigxrwz.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gniwumdvq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqjbhyrmd.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/glvvtrlgm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfkpivocc.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gckcdmtpl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtcktszme.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gfswtqmdf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/grfqjdhcw.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gwyygxsif.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsuxbykfg.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gierrsbct.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/guiygmwxh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gqqjfkuql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gexdgttgx.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/geugjnoqi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/ghtjlyzfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gxvwykpdu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/grqpgxplb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmaluwecf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gmjltgeul.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gtqdcslrk.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gjtdkphmk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gzyidegbc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcadkoihl.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gfrtyrjel.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvgisqiqe.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gvmjopdek.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gldpfbaqk.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gjflwwqxz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gnhztlyou.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gkwinsyzv.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/ggvryhqnk.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gfqtbfgtu.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gxmmpnorq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/giaeiaxyi.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/giztcfkyq.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gplxdfazh.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/grzarntsr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghfplpcdj.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gaggkaict.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gxswcsnrz.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gshqnzxnb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/guawavshd.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gmkmvpota.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/ggmvdfyud.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gaeoldvwr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gruqattju.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gkgutaiud.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gldlccypp.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/galvgjcxr.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gdmgklowf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/grkapjuxb.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gqtotcrgp.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gimyjjlvo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gvzfegzay.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/goeggbvek.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gqojbofws.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gpeelncqv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gplthwsky.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwggkuhmj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gzbaittgi.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gopfsrbrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gjybpmevz.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gzfqachui.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gpdtwpqie.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxgwlgtgp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glbfhifpd.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gvwycbvqo.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gvrcllqzy.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gouhrrzdc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gsvdrtynz.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/govpokbvb.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gqlkbdxnf.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gnrmkzjmc.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gxfekcavs.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gjutgikij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gqprksvcy.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gjsbtxftm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gppdhgopx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gtlnlrynq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gaqvmyfwc.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/geljuulvw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gchpxbgyg.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gurpdrujs.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/ggfhzjzxf.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gwvxxnqzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/ghwfcnqmc.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gmtianzbi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gueuowtak.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gfgdirzxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/glibjochn.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gsuucojng.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gzuezxyuq.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gqtshgnht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gkacnddlz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/ghtnkncns.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gmyxbbpmq.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gygfsvatn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gtdiwqmeo.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/ghccfdzpe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gknhosnfd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gcpnujaia.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gynwlfinc.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gwjnbexez.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gemrsvmnf.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/grlsvdkrb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gxxcsfzch.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gmuyuqeew.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gfjibmrzb.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gbkpsugle.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/ggihkuoqb.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gtcnrtifm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gogetklgb.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gqrrtekev.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gsomfifjc.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gdgabfqka.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gizeaklqx.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gnqjfhkwq.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/ggwbqtdsu.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gzlqqzqsj.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gnkdddueh.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/giztdpgyr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gmaudhpey.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gyxrnizbn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmlokakxo.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gnwqoyrat.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/grifqmxck.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gkrmhdqyk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gjeifpfiw.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gkjtsmpck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gypjufwex.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/guxrkhbek.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gdwjeruev.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gabhriyev.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gcliybvvd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gipknvyml.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gcarbmyze.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gmsimagcx.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/ggezucauz.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gqqbhombd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gwfnhoerd.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gkvtjevpj.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/goxomnors.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/glkyfzzgz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gmvpastpg.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gfagajapl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gbsxtqyhw.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gmfomglvm.sHtML


<!-- 参考信息 -->