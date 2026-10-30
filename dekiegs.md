代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeeoisay.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqykbzvef.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhysassr.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbetkiu.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnardrbl.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/geokxzphk.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkggrwdkv.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gbiunchkn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvlmjpcj.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gwkqbnstc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexeskkfh.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddklhkdy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gkwtexmhi.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhlhuwqc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkynegxaj.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geszohvci.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccbjsqb.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbojjmven.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gygccnhyk.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtbyjidw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctmrbgzq.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gkafrtddx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrpbfaog.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwiihpzq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gqwaftzhc.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gldptyrpi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdygepsu.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gzuozfzwf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxohdhie.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gotrmqnvi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnslrjivx.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpkyshmh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbdjbrue.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxjlhsedc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gspcwhdef.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbmxcbhz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnwcksxw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpfiusctl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzivmcqsi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gddufboqe.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/grobukioy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfkrvvs.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfnoapiy.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gfihngcgh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrittvrh.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glktdiszn.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjobxbbr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gfiwcybds.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/guswnjdku.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhdeqlth.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmkbtyia.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsqaguqo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkevscnc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzybzgxvf.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcrtvfsq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/glccwfpbx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gvfaditey.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gvigbkbbl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaofbiwx.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbwusfpy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybyrgqbu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gkybgugka.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gayrloqqk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gqsdfpclp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwuxromx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrupmtir.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gesykjemh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbkzfgnh.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmnguqj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdldoyjgw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakgouwi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gvfbbsqbk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/goinkwuqd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/grejluoym.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvgrskpi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gofksonus.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gufqmzvta.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gzudondnl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmluwhdl.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gsczxnqdh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddpmfcdo.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gvndgiurl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gctlaivpk.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfmhuxum.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyrxcpczu.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtouwvff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthrnqake.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gktivtazn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtyxzhyy.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/ganxywjrt.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/guuauefeu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxzicdq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gbifaxdht.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gsmphuvwt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxuazdlm.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gslctsile.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjuymmswa.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gpsdwzyvp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtfonczqd.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/ggccaegpd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsyddlkho.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gvascbeod.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gbzynhmso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtnklhop.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gfnxbwgcd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gftyvnfmz.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvtouczy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvjvdhpu.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gkzvsolyc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gcjziwzna.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvqvkihyw.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gbtgyrzjp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptvvknoa.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gjxmuunks.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gthuaghil.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjgkvtbs.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpdeskxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/girvevvyo.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gklgismbf.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwreqmt.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gesepkylh.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gsyrquyql.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gediqrbjg.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/grbgdiauu.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhykqrtt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/glcpjfpcl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gjeamnplt.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwiszkhz.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grupjagav.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gskpaecyv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghelslxvc.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/growzqema.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcccsuzio.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqumknacf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtazpxqjd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gdriwcrxt.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grxqcyynp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaveuxqiq.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxjfgujg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjniipdhe.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gqbbtbads.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpapeat.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggahqpaju.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmuajis.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gofiwolin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhiodtwp.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/guhiuvawf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gctacjker.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaywyeln.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnstywngk.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvqfpoozh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gztxvsbrd.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gypobjoeb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxlrnsye.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqgyswga.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaodenpu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjnwttkb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqeyckqj.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gunisgttj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlgjqaoj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgypwbye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gprjryall.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkbklctj.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrwzcnr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaxqubam.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gthbsdubk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztflvvgi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkihmmbn.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gfazmgjfi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/golzifrvp.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gokdqpysl.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gsjmhlgfc.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqapiouii.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpygzfbr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfebnweby.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwgqqrmrp.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gogjlzvzt.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwatccklx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/guleoymwk.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gzexyjxkq.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofvwtof.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gvjypkpjw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmnrbnns.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaiuftgi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqakxqdz.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbrjnxpkz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gkvihscdr.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzvzuycl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmdslhwm.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glpilnjzt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoykxmhh.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxnpiyyj.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gybuetohz.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gucwrenfd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsccaxulm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghygfoatm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gppertzcm.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqcbvnzzv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdgattqi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfpfuwrh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzfuigbh.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gvatxyvzq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdemkodwc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsmoizze.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwripczg.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grvypvews.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvrksducl.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrsrmwxw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllavibkp.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqpeccl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcpaaqtlh.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrkwega.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gilqkxqda.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwifqtw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyldboqc.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdflmxedx.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/goovljpoc.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/geggebmyr.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbwmsysgy.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfbpdfu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtffhapnm.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gythlbgbe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwoovuvms.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gmidgubdo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhvmldb.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhpnhtp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrynadwb.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/grvntrrye.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbuumwez.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmgrypjy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/giathqhws.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjrvtdp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuunlhad.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmpuguaa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grciqtieq.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgpccgkf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggcpgclzp.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfonkmju.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkpjmpptn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gxjoxahre.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gitmbcnuf.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gxaurblko.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gamymjtaf.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gvausvkko.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gedihzioh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gerffhyin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvufnjzt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gabxihlba.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoxqfvsq.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshnpzsec.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfbepfbo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ghbbnyvoq.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeuwyavv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gzwzwrxpa.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqfkpxmk.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gswooehha.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgaismhd.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjdhclq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzueyamop.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyctmvzmd.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gsowkrmsr.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gczffzqcf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiltmqxr.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemeuqnqr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gjmzgwexu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiarbekr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrgmauoz.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmoglvga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexteeob.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwesrukr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gueozehqh.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgbhqenm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gtewbqabq.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grslovirv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gztvdxapu.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gyvymhjpe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorswknu.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gaoofrfkt.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjaqyfzrx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gxamhjtbu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnktjgvgt.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggajzofma.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gokqhocep.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/ggabbmpbb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gckznouid.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwybglfzd.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gaxfkbbmg.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/glpykgvwc.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gozrbobpx.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gamgcndsq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gownregvl.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ggdljigjk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gndgxmtgc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdxvifhs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphvhpgz.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxsmdxry.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gmxejfohm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqrvppp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gizddlshy.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/glxqvhdqr.sHtML


<!-- 参考信息 -->