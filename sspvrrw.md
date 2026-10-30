代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksnmauwn.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gmotnlblg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gkrjarrfy.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdgpenqm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/godssgsoi.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmyubvbf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/goagotodl.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gysbakciz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwynoswfw.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmrxxllc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnovkiqc.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoajwgbj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsnuwygx.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gosepigjt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjheugvni.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gihbbvcoj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgpbijar.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfzpnyck.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqootzrgf.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gxdgihlfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbkgwgkp.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gbufqjoog.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geckxmbdo.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gczikwwuy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaairpmg.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaijiavr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnjuzymm.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gochvapni.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggtiitsrz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzbgrrgt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gwzpwioms.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyecwphj.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gbtgvcdvw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gebvydilt.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzxcsrbp.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gqovboxlr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gawmsvuyv.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gheuuvkls.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gymaniclj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gckwdaeeh.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqjccgkx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpntaseia.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkstdiuwg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gwmrbtrbz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gedusdjpe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlckeggl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gsjabuluz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkrhivjg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkltqbotz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gbodflpwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/ghbkwwbup.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuqksrye.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gscescsmt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewcuwkwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfpthnsz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcqksram.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gmditllcb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdmpcdjf.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsattnnzp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmebczvk.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnbqslb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gjlxvcpxp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhbnrkbc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/glekbawls.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyjhvqhc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdmbsbez.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcbqltcw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopgcjiqg.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxuewvb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdczfhrjv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvblgoox.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gprwkjubl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gttefdnom.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gwgyzmtgp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnpzhkcp.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgjaqywn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqftadnch.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/goosxirgw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvbqzzaqq.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghpfmyrjw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbntcho.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcgvwmkm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gfqqrgvug.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gksghcrmx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbcbrtix.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gaymooqcp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxcmlih.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gctafgjuk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grziwcweq.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/glbvihdnf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrhgecep.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gklsdnvkg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcovjhbhe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgllxmpe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/glknsiwvr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glsvkfhar.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfxqnfcq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/goyhsnucn.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gcigsvjsh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqobostks.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gccsrizfk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/getgbjuea.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godubhrdf.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gsifglrjp.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwibjqlm.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdjyxjeb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhpbqnd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gywfbjvgq.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/ggujnnzwe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/globvywtr.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmncstib.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjwrkgda.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gciqmigny.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/guixuqvbb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gsvmgpikk.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gmggejlsy.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcheqjyel.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbtazgad.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrgkkaey.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhhlrqzb.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glyqlhupb.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwqpvyfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gupxqmcxf.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwrcwfykx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gxeilinwm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwlgjvsl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvynmwc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkxufjqj.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefzukusz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadexjnna.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzwxurtm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnffdpxwx.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmigwqfd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefcdhnud.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpclppewm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gafabyvlu.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gdnizhnyt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmtocdlei.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gromywmod.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gypdyybne.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/guqnmjewl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvihhoq.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbtwywwf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsfklzkv.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gwmvtmcjd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcvyxsdz.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/glscuqzbs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gvymqorxw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqjowcsi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gabhwbqur.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gabgclmku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/grhtfysam.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/glxseectl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/grdvosrvf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcgyfxko.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grcazmfuv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsvbdnwp.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhmujbke.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gazriehyl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfcucoggh.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbowwplel.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggykiasri.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gosctffkx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplmuerrh.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyiensjh.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gazgznbpm.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gwotsjrgz.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdbenhno.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzzzfvxv.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gevodzxks.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/greucvlhl.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxutxgn.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkubqznil.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gbocfhjsi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqcvcalm.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/grmegqgcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtejimoeg.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrtrgru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grbrjqduw.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpgxqnuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbmusdlg.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gxxpjomtz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gakegqyze.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gqombdbnl.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtctatcyi.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsboaezvv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjgughsc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/geluvodjs.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gutuiglna.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuzqwdok.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gldanwpfe.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiymnniw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyykfalyk.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gwfqfifyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjntrrvfw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruqxkxzt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcqzumhyi.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/grqzvdqso.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtofbvkn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaahiavhx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwlebkaq.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmjdawhla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwomqrxhm.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbfjtfklw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjinasgd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsouvkzpu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdlghqolu.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsmckchx.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywjbffka.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gsskoomjq.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfytgxzs.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoxswjqz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkadsbuv.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnxqopvr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwftyahy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gebtasakq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gttveebsd.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsyfyrqqj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcytrcioz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixezjwcf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gotssyflz.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gdduhgiiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdqglmug.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxsixpyv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqutkoack.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gaktdtpnb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyklnlqol.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/golkfvjtu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawhodshq.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/goyrdjoex.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gawougzze.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gskxvsqoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gdowrtkem.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gfsanjtxf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gmapprabx.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrwpobjj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gqyqhxohs.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghbwqlrub.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxkwkecp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjzifwri.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghiwfypcz.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnvzqvum.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuqqhcbt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gxbextzkq.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkimpwsxb.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gswhppncq.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gntoogiru.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzewcbpql.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/grhejsose.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhtcftlv.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtzcfrwz.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/grcqkzxbu.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/glemxknii.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/graclvtsx.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwypgmtrb.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/giiaquwat.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gtdzzbjyi.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjobxzft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/guwyptxlh.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gofwgvswl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjciyxjgd.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmztuufir.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyghicbsh.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gaougvshw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gxllriegb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfkoihdpz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grxgvqsxc.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxeyglvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gehiktaxo.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvtgqnym.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzokafgs.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gbgdasrla.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ggkytqwas.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfrmoqswv.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqelqettj.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnlucsfw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/glaqrntwv.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdshczftr.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdafamwbp.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxqrsvap.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/geoadxtiy.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdaoemua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaagjrryi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzhurjqy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganssdmtp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gxbaynigv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givclnrcl.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gixpqohxk.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gafxjfnar.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsirkwrbz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gonngcezy.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakrpfheb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiriqwuo.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gaymtjaak.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gndomcjot.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmsnbmswa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoozuqxe.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/goshdlfqd.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gupmamxkp.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeinhqzu.sHtML


<!-- 参考信息 -->