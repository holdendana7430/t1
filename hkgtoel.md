代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbqvhfi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxjlnhcg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/giniittbw.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/ghewasohe.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtkgfkkes.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrbdmgm.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grefxoyag.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gphgcpduc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaefkdtl.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gznqpdxbj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehfepxxy.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjarftmml.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gugosxrub.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhhnyrjt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqdeyjhb.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgecmodm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gurqyogno.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvbzkxuj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkyxgnuh.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gzxjjrsex.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginceokvz.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gheknpgly.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrkdxbfj.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gqewffusl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/glfqycogd.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkgkrcycj.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxncuccag.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/glstbchzg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwznwfc.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/giozrgelz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gvbyhylmf.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gufhdcoqj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvppmlicl.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbthuhan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbawhmvr.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbondggzm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvvnhzrjk.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gptfzfffy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gssrpxaex.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gxhrneqgg.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gparnhpsd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbyjjlp.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/guspghefn.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gcllwkfdd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdvtafwh.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfmqdbwdt.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gwntlgxab.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvebnjmq.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdvinrxj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gobpxyhip.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglusinzl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqxaydlwo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiivmazo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/giukwdrpv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/ggrzyrehs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gmejzlijy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjzqxca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxfowggh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtvowpuk.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkttnuv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtyhvgva.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwyttibd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gusipgiuj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxltcrybb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gerglwquw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gluahvmkd.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/goorpkvvt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhfwxxpo.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gicyqtzjn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhoyiddv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gasulldux.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkswmmflc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/guoldatcv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gqypkkfuh.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxdfvolxp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzafyccmd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicrxdued.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwgattgg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gbrzefriu.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/giaciymum.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gawvjrsnb.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/glpahzmdt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtsnbshl.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gioheeefg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvukjphzk.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gizzaikgn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gpujghhdl.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynlcobgh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gubzajsxe.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvbfqyqn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifqfjum.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyyirghe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gujxgasku.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxetazbr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/glxcaodmj.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/grvemhgxn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbjdjgnl.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmtyxdddy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzxrwiso.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/goalfspkx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnwskdxe.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gghqocqfb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glziwqmiy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzurpkkr.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gedougpvv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrkxctrh.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gkottocnr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydzvmhv.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govfyftvf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgfscxjg.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnhoikwga.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmcmuuuz.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gfkbxtngy.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhbesppu.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyafnxid.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgzwqyti.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gqcawygaj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgyqbjti.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqdlttqf.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaecdbnyu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzadnbgbg.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/govnzqnce.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpvnbkqo.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxdqsyk.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvwdesdo.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gobtdwlxf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfsxbmqw.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/goonhddnb.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghttwzsoh.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gizdfqkxh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpdmnurc.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gmtpihvvx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gsgrobvzx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxjcqyhf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbitibjhb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbmrikpl.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gijzkxlki.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozjuzibe.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gresixxxu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gbormryqr.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvleriid.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhxlisi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsnzuvwo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfhrbvrl.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gmigbcqcb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxvapycz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejtxgei.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwmxximt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqoktcyp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glrfcpkpy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gintzrwyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyiibvibx.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmukeezx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmtfvdgxf.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvnszghq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gyxlyvcbs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyldjqunc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gcrbrfqrl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/galbgmlzs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwvhterh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gqmxghnhg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/guguoibbs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glllwsxbq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatsaturi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ghlfhhwtn.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/glbcnildf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/govzuebdv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnstpqamt.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gebvpotem.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcipgsulc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfggabxn.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/grgiabvgr.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/guuczghdx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxonhxdyv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrjyarlk.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gyfwvdbxc.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/givftmpez.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqfzpnwrl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gwcuhknaa.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ghewjdedx.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkwdgxshx.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqszhyua.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghwupbtgf.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbmeuzqlg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsmaqnvp.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjglkbds.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauqxrpwc.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gclwudszk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzwgysotg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxslexiqe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gswsyopod.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gixwizruq.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gnqzmgrmt.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpqnauykf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gijijldmb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqqbefix.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/glknfqrrz.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkkoiydmg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvbhyjzs.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcobskzn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/goodejjns.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrvjrpj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkpdyhpaa.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxepxanbe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/garumhmia.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gksypqjmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gatzbctdj.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gatcfjhyk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnnhihjn.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gciyvuknd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwtxrxzrf.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfxzleyn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahbayoly.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxotxojzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guqavdeek.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gckpcgmhz.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyhpbfamj.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeqtooaj.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkbfxzkuu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqimocwcz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggceydefw.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyuzwcei.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkmdvwex.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/glxizmlvf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gigeupdqa.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnxwmspl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbltbyfp.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghexoqoyr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gndlraixx.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxrelfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gcskdqzzw.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghaxnwnqc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/guzcancmu.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glumupezn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gekfkkhcj.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdlqqavrc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gefhtkhfz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzpsxgsn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbuqrunxz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gapzbdoxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gonuiqlcl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzxdealo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/glipinlfq.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/givsipkob.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/geetumvea.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnsieqqp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzgrydvw.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gurhyxulx.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekkluicx.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzdsbhwu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/glulbixjj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gadaxqyly.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gihwclpjx.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxdwgivjp.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiidxiaz.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gghhrbqgu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gerindmqa.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrihhmq.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdnpqdjl.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gozxnkuba.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghssrmpyh.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gahuvccel.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gevuzpvxj.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddpuqfvd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhhfirfo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/glltnuvoi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/guiobmdgm.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/giqvalfnc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwkifmvxx.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gomfzfelq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxerwltt.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcblaixiz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpgfcpxe.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/glcmpbcqc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmycvasfu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiyasnms.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/grjlyzivr.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqtcmass.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxmxbclg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gitjqaebb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsibegfx.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdmxoapc.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grhplmldq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixldanov.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/goimncxpy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrfmctre.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golhyoded.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwtalgbv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/geszneaoa.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqqvlstr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwgxlvkm.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ghwqqfoap.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmisalovs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhpwvliw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gidxfepyk.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfxwwuqf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gijvppegi.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gokvthomf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gsetxmicd.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwpisczp.sHtML


<!-- 参考信息 -->