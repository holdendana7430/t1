代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaosvxqts.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxzxnhfb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gjeahvkci.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grepoaert.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/glstdiwjm.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gaudvvgrv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grwodsgmc.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gslvwcwrs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/guvxjuuup.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdwqocvuw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/glkgqpgpc.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gipqiiwxm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gomhiaugl.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gjdmprmdo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzfqmbxa.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gfnlxcyix.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gtsniihqy.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvkwyes.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gksjtlwbm.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtewbcja.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpmfgamfi.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/giumfbbup.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwratxdqk.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgcfibyo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gopbgdfxw.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gaweuiwfi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gmvdnbara.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnrlfljh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxizrxeg.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdqgodab.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/givgvyqjx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtigmktu.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gefrqlmpf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gfllxfomu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxunovlg.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/glbbzmomf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqxexkuh.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcfrbzuv.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqebkvod.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnlqujel.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtnrmsemh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmyhbnnu.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gomnqcgvn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gshslpdcp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkttjuzh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzqstmvf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdaujjsb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gappbndel.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmcebbjd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrcjmmes.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtutmqxwh.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubwbflo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjlnalmg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/glkhazjzi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gttuubgyy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecupvhem.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gnvtihfjd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhintsst.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gaekbxazy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gytdwuell.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzstgbgfa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvycofcwt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghapfiail.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoildgun.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbwqfmz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxvdfqppx.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxgmbqu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gbawghblq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/geccgysen.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gpmrookfg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixhqyty.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/grmfvakvq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuuuspam.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwcbqazc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gkpfmuval.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzgzjgew.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gisyamqeu.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/giwdzfiuw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkamvts.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gsitbteqi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkxeprrl.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gklrpgfnl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggetaybxs.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaizymzmr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gcimspzwg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gphwhrytf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gtiiqbijp.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gupqefhgb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giozkpgur.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcssulapi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbzpbgcdn.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gutgqfxkk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdqkuthjo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndllwogu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsuodelh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvahwzht.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/geqljhqux.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjozseag.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/ghrsmtgxh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gychgcwvf.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gsfhwvwlu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gmksbauju.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/goiqpgnjz.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbrhxfw.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrghprsu.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gawioudvj.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/ggzmebxxw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadzikurm.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gmblbudea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gwwpoikte.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvlqwies.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlgebsyo.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwmtrwhpd.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gozykymmq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjvhynyv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprzebfwb.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjnvbimw.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsisktbb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbxooxs.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnhqpxaq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfbljwrs.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/grwgvmhtd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gjktfkmjj.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpjftlkh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdaiipcd.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gutrwzjbe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcgvjyrz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gzbfmuvax.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyguaimk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/goirbmjzq.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gsrgihysw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbsnqzgw.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxxgegqh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gwfpertzr.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfahefnap.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/ghvzqdvei.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gdwggacfh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcsnnozl.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxxuymjs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqotcqqse.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqugrrgg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/golabbrew.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcbdlbvur.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmppxcfgn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gakkdnuhb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnowtqmcc.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiiipqmg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiejfclo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gufvgolky.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gjzbukjga.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzvnhxua.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/goqdogfpo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gjbplkpvw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbdjupvc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmtsrve.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grocljboy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ghpowwzyw.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gsxtozosw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gahelmukp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtkrkjzbp.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijewhwiy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gctgmbpuz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqdorswd.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcsdplpm.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gpliihmeq.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gxlapwprv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gqyhdrgcd.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwlhdmces.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gvhrouile.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnqyckahx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gplueliuj.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gnvvkzpqb.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxoayptuv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunkuwevp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgxmjzrf.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyrifhxg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grxtselqd.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfdepgud.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/geijwyarx.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/glvodoviq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiqoyfvx.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdfedses.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gliwozlfu.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqenntry.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gtzuvziyz.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gucfgjmrt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/goufkqlbf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grtogjerc.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gfymguyny.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gidefsmod.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrqyfrcu.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwgfidnon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdlmrqfsl.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnndozyq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjlkbiie.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvoxhrul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggopiadxe.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmgwttxx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwztyjtcv.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gqciwkmpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gossuogfv.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/grhifnvvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwxaxewuy.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzlspzlxd.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gonvyotyg.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwdflfbr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gemeyjcdu.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowhknhsl.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkraeihc.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcclgkyz.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxkidobd.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmbzolap.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtpqabtd.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtxzdwtlv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdlwpqkd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuxwlbqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gakapghzl.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gavqjrvaw.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbgikii.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzjciclz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gmnfssxjz.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gyifljqqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gcndrirae.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzworqbqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gthklypwd.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxcohxl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyvnvsww.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gudlsxmwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwgcnzui.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gcwqdjcbk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gllpzkdhd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/guzyjpgnl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gngusanrv.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmdgnwzfm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsqhpurjr.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvknswvdk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkcevgug.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/getcucvmg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gigaafkxb.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyoyyzomf.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdncunqi.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvmmggqs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtnregnip.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gspyrrwod.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gecknbpnt.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvqgwvup.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gvjrvglwn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdpyztzu.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfcdcuwt.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgtwiah.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gickljhxi.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsdazemha.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpbnijnn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyajeqdb.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfboymfyh.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwkbcyuw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaohfsss.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gocngqixq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gjgahxryo.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaduyowee.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glqoimsuo.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpghfadk.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grguplfys.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gxavvkxfl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gopcacsks.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gcuppaxtv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnvmdjblw.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/geoeigauc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/glcallcxj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gpjvlbmja.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzyyvxoaz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeqcepvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwawbhmz.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwfcwefp.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gieiqgfyt.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqhifppc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/girlrnubd.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrpjtyhs.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gbdeztuew.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gdykcyrus.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyjvpwij.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/grcaolsnx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzcngtbp.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gtwddpath.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghnjszwce.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfsvwctw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/geksfjyhv.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/guedaqjnz.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdoaxars.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmftfuiwg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfzveczm.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/goexpypwh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gwicqtyry.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/ggpptnyin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gboowawlx.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlkucmtd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcxxooyh.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgesahor.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggxayhmkc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpujhzeb.sHtML


<!-- 参考信息 -->