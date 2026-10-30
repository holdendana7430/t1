代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gbzncstxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gftoqrqzh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gkhfunufq.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibiwrdyd.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzbloty.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gujqgacck.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giwuihqhn.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gnwflbely.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gymnkjvqv.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoaszznk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gfjhgamkx.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxpiutg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gponzchic.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/grlhjwwli.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnuajurl.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gnpmyqfbe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gdbnuctuv.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjosdffl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/grturyhdn.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/goxgamgli.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/ghxsignft.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gamxatzxj.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghlowwnzm.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/ginouflrj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gedoogzgu.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/greykpjxa.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrlyoswz.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvqzuwkk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnmtwnu.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gcemtmznj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnrigidz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmmxwfmd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjgdbqcb.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gngychllx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthnhhvra.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzmqtsfuy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssulwegc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwtdkbovm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjzdbgfq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gyicarzuk.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gsueqfrdw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnahshgy.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqekffgt.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/goardkllx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gyvpjabna.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqeccuolg.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gfshijjmy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvaulejf.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbuycyzw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gonslkhdp.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqhlvwxan.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpihajdqw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowjcqpfh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gihuiexne.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gzrxndrom.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobxfyvv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtnhfbix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/goepxxdln.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gpitbeuxk.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/ghlnuapej.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/glujfbhkb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/goewieiej.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gursuuock.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbzghgbt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/ghucxbqgw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/grqixkrqs.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxzvdqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/glsdnfjvc.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwdpydbpz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/giogpqrpm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkxnyxml.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwufutpkf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gctpldkxo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gajdxgxqt.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghmwrjmcr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfotiohyi.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmklarrmr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gladccoru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gxjgvcxcy.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/grbrdwbwr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitkqjcxf.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/ggybyskkr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gmcnwnpja.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gbezatvox.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcsskhrk.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfurricdb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gzpyrbork.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gubtqhvrc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnkcxklb.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/geipmserm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjivpdkc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gahwfrrsu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/ghxmpaxxr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/grahnqafy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqdhdpep.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/glyhowpxl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grhavjqfs.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggegqamhd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxqcqmsa.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqurqggb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmldgrtu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwssjollo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gobbsrzee.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpsmliawx.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gjerdswvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbsuznhp.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gcspbfyfq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjwxkcrg.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruvyinwm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxqtiexy.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gsbbevgud.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/glhnkjemj.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gwrtxzrip.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/grqqagthf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfcrnwz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/grcwzirhl.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/glansuiij.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gpmsmlnxh.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gufhyniuq.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gacsprqjs.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjewptzm.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gzslvzobf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gjfmwjlxn.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/glqctssqc.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsxvzqg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagkfbjcr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gyyenuzqh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpnjpwac.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixdogtpc.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/guvkjjjrp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gknfmohqn.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvskzbiyg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvzkxizo.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkhahyfjh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqsfguin.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gwxanbvvg.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkirenstm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnejmktta.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/ginjclkpw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/ggcqongbd.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkkcdmxt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gndphpzgy.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gsofwdodo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gnrwvjtmh.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsvoaihi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyjvctzx.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvwcsvube.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhumtycs.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/guafogyvh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gabuczvxf.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqvektod.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvenxsdwq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaqojoop.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcymsmygh.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gazqkskzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gykgzcxhw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffbufgti.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycrgbcqc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgobraxi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/geyooptau.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gfbkeratu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfhpyahp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgftzwwf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrshivwf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslmvyaix.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gmwtewwlj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gxqcvgmjk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcmfmjgdp.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gjtedqthx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwlzdblk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhtbbqzu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsezwngwd.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxsmykcr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ggknbuefz.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gyphyawrn.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gybodyfbr.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/geogjyvtq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgjkuzoa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzebpxudk.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokbanocn.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gffrlobvz.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxwarsjze.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gthynuzxc.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggliubjnr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gtdxnaiul.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpenafil.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvbavvrj.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/guxxwcbbd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gautmdnbw.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghegfyckz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/grfblaroo.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gwddyswxh.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvpbivhdy.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/giqqbzmfk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifflxzxm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmcsledw.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojvyjlxi.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gungagksl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaicbqtg.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gcttoptml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/geflkoeyz.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/glyxivira.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gccnwewak.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gywxcjgrc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gprhdjvze.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/giyugryjm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjyqbrpby.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gbuqzwudj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsajyxjhw.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gghkyrgzo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzorlibtb.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtiqqbeax.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbazrskn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvglouvg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/glsrnblbf.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzpldtfp.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gptxiehgb.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcvblrbh.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjnnubdd.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzgtivsux.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggifqpnut.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvdwcebdq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gclfzcpwo.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsdnojti.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcneunnxd.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxwnehsv.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gmsfyvnpg.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbovosej.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibvfrxgb.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxxbcrww.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gefmytvfw.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyaoxkroe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibplfzji.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzkelrzzr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/glowvosww.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/glfqwcexm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqtndbnx.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsduxsln.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkwndyuu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjcvcgnz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gxujwrwqh.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gpzdloavw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlpjtdgx.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gkjvtdtwd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ggaltycau.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmwgmafa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gogfahmuj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexmzlvg.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gicufxquh.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gpisypgkz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/geckjwija.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gzwrixgeu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdswlzwpx.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gaioydicm.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqizkif.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonymkqib.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjicfvelv.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gsaazchrs.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/goyjbwfme.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ginervhth.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltzvftek.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqmxredg.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqqazdhs.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlgroqe.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkfgbkfx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxxgnztw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gcuvowlvi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgqrzxtj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyfuzrmdi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/giqopmmwk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoechtgb.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gieqrudia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gdudxgidw.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijgebwjp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdsqaqwvg.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeilgvme.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gnusjeepo.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/glnplynjp.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpghjktb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gvejsiciy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvcwiast.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gltlxqjnq.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glzsjwklb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzagyhin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gxaaeximw.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gozqimwyh.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeolehdh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydwnscek.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gegzbdqsv.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glqksiujm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gjepclmis.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gngesunod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/getqnfequ.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqlgciz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnxuagjp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerfvxckv.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gkcmsuwiq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggscnlhpb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnjayrfy.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeagrbat.sHtML


<!-- 参考信息 -->