代发 wailian999

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxefvte.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtaukuux.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gncfafkjp.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeawkgmc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grglwlgzv.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gdhjeizkj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gqamjlhns.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gjsobyctu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyktvyjl.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmiegaet.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnacrpdj.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gldqgnqnv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gbwxxtcej.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gseteiszp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gkamlbsgy.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkeolhsa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gemjhqjan.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gszjbeyzg.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghicyfrlm.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/geghwfifs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gajnxeylr.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkeslohe.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqnlkzwyc.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaesfympu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabkiaklh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhuakywt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcvvgjqh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshchceau.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqasbpra.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gzsllzofw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gcbucdehu.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqrwocpqw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gzsrpkexz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gschbnswa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfvikufm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gxbroqpws.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/glwvozpkl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyeetcqp.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gcatvlowe.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gmbcmsvuu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurszunky.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuwwpfpr.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gsorbvzsx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdekuyynr.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxalrbzk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukhgxenv.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/glqjseiww.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcnhcokop.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyjxtfc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkuonussb.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gflhzunss.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gumopueoj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpcwtmjp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gsrnqntno.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjrxrecb.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/geeyntuum.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gabkxmruk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gcpenzikw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjqtwfhy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjjxlreo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gejeitqpr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gecwcwutx.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gawdpfvne.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/grxowvxxv.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gprulrqtq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gmcqdqzcy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmwgskpu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gytpggphy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrawypk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gemnvucsy.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxdbauncc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/geipuhmau.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gywoqieeb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhrrzhbv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomvjegbk.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gocrpdwki.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzshcotby.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gveirlyva.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gepllfpcw.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gqrhvdcxw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwquwyubz.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gktljeuzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/geijnqptp.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjncvhlhn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/goartitgt.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajiwqbay.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gllvxleou.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gildcdkfb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/guqxjlhko.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gkqcbcyvp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvqniowi.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/goewitujz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunjwgzs.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwjmithdh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwlszhsg.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gedpavvbo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqcsagd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gcoyqrcsi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwyrnszn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerxpkdzn.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gsjorlbej.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtppthtxu.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrafvdda.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gxklysoev.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/ghnkemndk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxkmfguc.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcxzcuck.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gcajnpikm.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/guvdxecij.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getdyukzu.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/grqemwtve.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/geoakuwvj.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkrxnsvg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqizkgo.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gyhhcsdim.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjgdhlbuj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswucntci.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gsdtvmrfj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gcamprrbw.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/ggfmponjv.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnifdrcrm.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgifmoc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjdodjer.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gizckvilo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjaycev.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gkuwccoae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gjagitriu.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmglcmhez.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyrdwriw.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwmbanie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpnwflapn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/glzxqtuut.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gaxdybnbs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdycphzu.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gefawhchd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gcpxblerh.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonumrkyp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboshdmth.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdxbglef.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gubkxpdqd.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncckswey.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goymxqmfr.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsenqozq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmdwykj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gecluxxdf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjznzuatr.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gewgmxpxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjbtjhwm.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gvdpyhlbc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrfgixme.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxlrmvow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/ginpwwehl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gayjuxapw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gzoyutwoi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/guasmqzlo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfotvhsxf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnkexjmf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpzuptdb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdkiznnhj.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkiwtuhxj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gkgqrmeus.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/goleekmok.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gtctlzumw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdnldcxhx.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gkthjpvuw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genkmyjjm.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gjkmakazp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpisjgucp.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqoztfcg.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gozoyysgq.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gthaiqsrp.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtubgewpg.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gjzbwsvun.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwticktjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgypcwtc.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkkkuefm.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkukcirsq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkiascge.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasjjikad.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geidasckz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwuxauu.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkzsfpfoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxlaultsg.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gyxceevdr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gimdycnoo.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjwsabkdl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gearubhla.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gtkdrnnko.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gexicicrq.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gizpyaebd.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gjtmzljbc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grknezmvl.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqohvombq.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghysugawu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbzsukvww.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvekmusn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gziwlwbvk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoygqbhs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyhqarhic.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnacfwjhz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsahbzbz.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwihaquew.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gccfzmqwv.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvupwujb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gngcmnydw.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyyogmkt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqarvaoiv.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gthndrelz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gourtdfut.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goobcdglp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfueruzru.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnyghirej.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybuocbes.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gyqlcrbvs.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghjhffjrp.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcjqciyp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjsjiyima.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdowweokm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gumpimmex.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gxapososo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofiprcqr.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfyufvip.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gibbxisvf.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjljizfg.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gitirmcsq.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gmncsuzsm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gkjqxyyen.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gapdcupaj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcmcmqpv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaxllbjz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gijmupcss.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvmwiyva.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaulwhgs.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glzmfgibz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggquzykzy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfmcbluc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/goygdxkuw.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/geqknsogo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfshfguul.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrgpnuks.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gltmrxdlp.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxehhixcr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gienpgkhd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyogragi.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpzpnaxqa.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gevefafug.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeispzot.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjuretuv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gbeudtoqg.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/giojpfyan.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcqgjpvt.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ghrajddxg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkkcedi.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gvwyowaet.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gifjxfjuf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghisgpnta.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbjvmtqo.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/ghqclvevy.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtkxsyz.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoctbxxn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaiwnfmj.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gnswmxlbq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxdcejxp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuyspzsd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbfupqofg.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gpzpedkml.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glufuytnr.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcqzjwdhj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gjbqmagig.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgnrrsfh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghslsuwua.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gukorvfht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gcwmfzzmc.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/giwwnilcz.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqcvnflp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gqictbuhh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gafroyvpy.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwonajkxj.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grinbnkcl.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gvshkseol.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/glcgmeuuh.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gavmvilog.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnjumqff.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjjvuwzvj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmzaepwa.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqvirfjn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gimgpdqeo.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gbefdttgn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbxfcpxxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/groqkyopb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylmgocvk.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gepcizrsi.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gtrzkivca.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqxvumud.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gaanadnge.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/grstfxiea.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdemwolpt.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gvrxqxrnj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzjyfbwx.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/girdphbun.sHtML


<!-- 参考信息 -->