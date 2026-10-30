代发 wailian999

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrtqtkzm.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgnukecx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisdvjflr.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gfdspcdps.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtysdwrmd.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gboolshns.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbmwzcqr.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzqpzpbi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gttfhvvff.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gphwudjys.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/genqidxzu.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gonstlkkk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gsopnbduk.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gaeffqphx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmhntzfj.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gfkrttipu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhxwjhzv.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gcfnracjt.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfcslyzba.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gszmjirkj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwdafxl.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/guhoszifz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlefvpjy.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gowifoauv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjrfmwxrq.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gxklvoqjc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/geotaraea.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/glhkplvlh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gswpmlooj.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/guynqfmas.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gaspxpnay.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmffynfv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadqqfsni.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grkgzmmoa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gllbzpdgk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/guoeduybg.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gglezxpjf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaszkelzn.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gyvvsfdhx.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaeguyso.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlfwydtl.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjrwjiyu.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gydlemomk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwqtwfly.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtalfmfs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gayfjxjhl.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckbzxflt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaisolha.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gvakndeai.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjselazef.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gupphmvuo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/ginagfsgz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtoynuk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/grfuyjjls.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvvsvhra.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnpmzlam.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gbexjwfrz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gsckmoqvs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxttnwse.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gqlhyekon.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizmrywgc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhowfuxl.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gahnjyvyr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyiptypq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/getyejyju.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/ghpouwnet.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/guciqhkkx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsitcwzb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdybrilo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnzifgek.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ganlgfbll.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmeihcna.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghazvtbyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmoklwbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexwnazs.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gvaptrdbd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggsmccbff.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gehkoxoha.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbihwxieu.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfbugaxo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grmoyyjpp.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gidjndpkq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gjupxehlf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjvfsrjh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/glifatatl.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gswobdknx.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjbnruv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gyqzukwha.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfcfssnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/guuwsuhhy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gosiywrjq.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gehxobdwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goxwevqod.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjozhyha.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzywlxnvr.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdznewwh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxpopzed.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gazizfpqi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gvwrzfzrg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmpfeteam.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gxkcxvxnr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghauvoslb.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlssslkl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gbcdlgmtw.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwnevquix.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkkrjwhc.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/grzwrzczc.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncheldrb.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/guqqwkzxj.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gphvlhuji.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gistohagm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmbjklnk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdatxrz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutocimlk.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gcglfnmot.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzgqqmj.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdomtdepc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gamieszrp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwbkewdq.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhrrbzwp.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpxokjbo.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gdttdtmzd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gmvatvtsp.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvrxkwms.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhegudek.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgevstmt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gevllyfqk.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/garnuivwc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkgtohy.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbjlzaqo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/guuisqqpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gweknondx.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttnxcyld.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gaydwzajf.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeqmupim.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/grfoyaiom.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gbadaprpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/giefbwter.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqddkkbuh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gwdgtgngx.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gtdbygjam.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzlwusgz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjavposjp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfvfspys.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdglqrdqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebldmcwe.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwtwbriaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gllzyvimj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuponvyz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrqshwym.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/glrxnpswr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacwicwfl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjagognkp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gjpqyetwa.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggozeuqea.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gvmtibhxn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwscbsew.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gqqzwkpjd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlnatkyy.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrhnnrts.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtklmvxyo.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjjwyxdb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gcinrzipk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gejlwhpjr.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifosllyb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqckuvdfl.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfefzgl.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ggtidbgzt.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gdkofhwfi.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gqxqyltto.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpklubfis.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdxfvnpds.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebipnxd.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjnfbwmeg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkjtrtwar.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdqsrkfe.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobdmnbwh.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsuoccye.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvegjxcnj.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzspqfruc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gtlxyxcki.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeebzvjh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grrulnmlf.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gipfxnctl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gagyjcxox.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsgslgnui.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gudjdvhfn.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwljeatc.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/giyisupjk.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/goiljihpo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyxrimkq.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gymjxllvg.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gwcbujwql.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gijwbfnzh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ginvoippe.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gceqttqfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbopzcflk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golujyrnj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gurzneyjz.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glsybgfui.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghkjbnrwh.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqqsrzsk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqmnzufh.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaqpbxxm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtbzxdbng.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtenpozwv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcpchzyy.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvowdjg.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexpbqra.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gkoxwemph.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbpkjrdik.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpihzbibt.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkejnjgo.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gwyfedxqu.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqmpxtioa.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvexlszfl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvehypgjy.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwrsjyvw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmpstqoo.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gycsqtizv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhvitth.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwaybqzfz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsouckfix.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gvuvaffpz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpnthypf.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/ggnqqnqsk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmgzbvnr.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjymytgq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjfyqdfsa.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/giusnomfo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjalsrglz.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrsjndtp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuakrycl.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gbnrnsgbr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggshfuxkg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gssruwqwv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gqnadfoon.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gicqkmbry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gdwtwofrz.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeabfjpe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnowoeudz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfxbicok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gecyrvxzt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzllmdqt.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gobddsmnl.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gapewxsrz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghluqpgau.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexiyjqdj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkchtewu.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghftkawaa.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxanqcjpq.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjabnzbds.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbkqfycw.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiqqmeke.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ganweawij.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeixpswd.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhsxyogy.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvtbbrly.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ggiviupxn.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gpevcubrb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshltkkw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjengprd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/geqhhvnco.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdbdnewm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdciuqnew.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gvopwbnpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwrxtwsmw.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyfomufe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgfdsej.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdvqaeaf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmixanqi.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gelijsldu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqxamvqhs.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumpxsehg.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjokgxapg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlnxmkus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtysluoxd.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/glzlaxixq.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxgpcbdk.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggelemtfb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjxlbvdq.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzakudwpx.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gaunbaxcy.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gtilqzghc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfbukcyz.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glbgpujhy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gnichmgsi.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gifoyzhhp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gmkqceffm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/glhtpcmop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gswtfsskr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuzddlhv.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/glpfeyafi.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrjdvngu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gasbfqzgd.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmonyyr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gkwglhmur.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdzkqqpo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gncjgotvx.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/golnbcsuo.sHtML


<!-- 参考信息 -->