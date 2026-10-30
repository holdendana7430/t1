代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glardhhzr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwmuaztm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwypotrdb.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gonujmmbh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzmoegyl.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gmoscunys.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gzwgikhos.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gtirzjejl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/genwhncil.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltfggkkb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrzuihxq.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/ghgewikap.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamowwfxg.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/grtxqsrwc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhvuatgw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmdakpxe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gjektqadb.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gfkjqzywt.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glsixfkcq.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidewzmmu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvzlaunch.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gmuygsxzu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/geqnzhsno.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtlqbbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslnxapmp.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/grbhxhfym.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gonziomxs.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqdjqbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gauwmwivu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozjkcvym.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqpfhiuc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/giorakblp.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlmvaxqk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfejgbhr.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/giortdwio.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gryqwyrua.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/geeosizbv.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnxnywgk.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gmzlogkun.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkueeoxrm.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grjktdnkm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gaoseqblr.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegcwjsu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahgwwlab.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gvvrghkon.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/giuknetbz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbypebich.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gnxfxevjv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxiigqwhe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/galeqtvfv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmrtdwcu.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmixitsmc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqsnhrrg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpduvnkn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzsfslz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfecisfq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gkehyagxj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gtogsgkze.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiyauguv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaexdwupk.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmphbisql.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkyfztgv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaquhkxp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gdggkhtjp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucgqmak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifhxaqgn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grewviqur.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjbumrta.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gksrpmftd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzzdayfp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbmczedr.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gosmtrwlh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwevchlz.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgrmjxzn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gmbuukcix.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gbcpqbxpp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxumqwfon.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gzocbhxjt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmhbbal.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiwbaxbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gobohpkkf.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gwejurtbn.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlfhgtpt.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/glyagcbly.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzcdvqjp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guytpyxqv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaenskmnw.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gslbzpfvd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwbsquau.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiznewid.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvirnzoq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappzswrr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkvvsenxm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gggfsblph.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqfccpcr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guixbcslt.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gigybzday.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhtvetbj.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gdergscnz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtfvifoo.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxxzhpz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztwrpiq.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/guhhbgzzb.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gsobpqgjs.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gndawrzxn.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcnwgomw.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gaxfpbfoy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfonnhxpv.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqkfbzbz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gppoennsv.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gabjxutub.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzotbvjaf.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gullkxbrz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gueuknlhn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/ghkimxjnd.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gccetxvqx.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzqbzkdo.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/ggsthtblh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gsfhxxewm.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gtkewveho.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrsgbsjg.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/guczgpemv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkenwmwe.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmaknmqz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqtcybuc.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/giepmyjfr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoobvlpi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizploopx.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/glwprmrpl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavixztrc.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gopcqgmup.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpptvzr.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gfjmkwwna.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gdeuuxqfs.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpdiuhgz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyzuygoy.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gnwhgvicn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gixahfuci.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuuuqaun.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gudufhljz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsdcffkqi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gugddpetl.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/guzhqtlmb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrbckoly.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcilucybu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goqjcwocy.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/goqycpjel.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmcmgbbb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/guvfwybmw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtevoyiw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaqjcobk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljgfgkal.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gxcbixazj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbugaqnj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcghxkvum.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjhadbop.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwxnrabn.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcojknltw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxaqcits.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuydgnqx.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndveoknx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmndjroij.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcnugdbj.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpnsnqv.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaecpkaz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gypvsgcrw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvyryzof.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gukurzrdy.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcszgyqfr.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqcyygax.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/guldjwles.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznrulrsy.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbbqunokn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxixryiui.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhacarkz.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzakmnb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdnvczk.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumbhtenq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvjwjfqjp.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtgfsmzgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/geuhzocsr.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwnwnzhg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyicjqiqt.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssxgtvxh.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/grpyohfhh.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzunbrhte.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpoiudh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopdiycqq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gryvmrhod.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnmrywlyh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guuiceesg.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyulctyfc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyighjkit.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giutxxgyf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhgfrnih.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghthyltrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghngbucun.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkdgipioh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggfxqfmuz.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/glblwjyeh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxmeboql.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgvoqpzq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtntynhws.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjabcrvh.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaefzefwx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbptqtyzd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvezoedqf.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyiyxchgp.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgzrvwjn.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmvcjnmf.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjlostf.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtpsqgboa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gybcifofo.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnifxacxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcapmkuji.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gpiomxmht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzijyxlw.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gctxugdcv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckvcjdah.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/ghsgdkzrb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gbbzshjjx.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/goywtcpyl.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/glxenuvcu.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gosnydkwd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzhrctimj.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjxajosj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gljmszsbs.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glddrbxww.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwxmozamv.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/guaxwamix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdegbkdc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/getczcyfa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gxdcrxvha.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogvtjtrj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknxpodvm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeccbblx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhwbzsf.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwljcdeqy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/grgdobcew.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfneldrsd.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gedmekyob.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gdnyhhnqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrumkibc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gkakxdnwm.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gvdrebbwg.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxjkbyleg.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/guxsbbbws.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqxfzqjq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gedteggii.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gdmmcjrkj.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkggsaps.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gobhelorz.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gvwruqlnk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerltxfwf.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlhirprm.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ghffdpwqp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/getkucxhy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/guavdlytu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdzbkzfl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjgnxdhp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxrczub.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/geasrkahr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbdovqvg.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrsammvj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gbtrqdzju.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gujaxpuck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvgobmho.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuohupke.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gaiqdqeen.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbovadzat.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grmthllgx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gojxlxzui.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmezjlrtv.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghneddfsu.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gawcrpfbv.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjrqphjw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/grbmjnyld.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboiubmdf.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gbnemftvw.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gvgzevhgg.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gemwngvwt.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjpegifi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsxmmfrk.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gorfskbmf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnzqegiw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gocbtpotx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjjgkyvo.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukqwdjrl.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkvxutkx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmqqnqor.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gtpftuvjf.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwlacdtr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gdnfldypn.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gegcrwrtp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvnevbtn.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhjsicor.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gwddacfoq.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gblrtrrmp.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgobyiv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteoinvyh.sHtML


<!-- 参考信息 -->