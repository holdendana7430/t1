代发 wailian999

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcbfowqyb.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/guchlljsg.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gofnkvgze.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxpaovaen.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gsuskyogf.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/goshwrfzu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoudmkcp.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyyednumf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpgzbzei.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gpjgwrbnr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gadjxidwt.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gatvyrnvu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gaehfuheb.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxmuwsgg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcujdych.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjnidtxc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrkkopkw.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkuhmoa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkdcenej.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gebxteryi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gizcpsxab.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctmajsn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdskcbmtt.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gxcjcvyfr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkileksyn.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gkdyudieh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gocedoigd.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gusfxapxz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyudjmiw.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gzzcbkdzo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifnyqqpq.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvxqgcx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvjcnpeo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcxiwlll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcsfjoxf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gackkzjon.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gikhwqwvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gclyzxgvn.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gfhnitwfr.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gekjktxze.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcabxnuwd.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgumtcqb.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdyrmdfz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfpzinaq.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gehmeumya.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsjqsndn.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gajeityzt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gztpspbpc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbzhnbat.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtabukied.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkfebwfr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gtsfuoofz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxhsxeqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhahrsxc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gymrhnuco.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfrfomgq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlajapdp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gceqxjeqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkegnznv.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gasusibts.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsilhcwul.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gscrfrepk.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gobinqgmj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbilsvwxt.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnbbyemoz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepkbkgb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gmpirpjln.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbdoico.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gktymctik.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuldcdsp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvutoyps.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdgfebob.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gjzfzmvfa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmalciup.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gatnizabi.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafvwhhvg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsrxxmh.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbzrxols.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/guijxiwfw.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gburaflxi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyflhkblx.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gywxsoyai.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsmcfdnq.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/ginpfrbxa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqsweiy.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfajtutp.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/guyiooltk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkboufzgb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbbrweaz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gorbcvcjp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjivgqga.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/guesopwmd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfoknzlu.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqjwpxfve.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxtywidh.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoscmexh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grdolupax.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/ggwhfysfd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gndhrbuay.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkpjrzjk.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/grrhuirxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpwzuaer.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljvddbnp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevmijcmp.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gulnfdxnt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gwjjshnjx.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhczmpws.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/giptmfqoy.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhpodznq.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gfuwnnqjc.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gaggwzrjs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkzrpcqn.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkmkuxsx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gxkuizvlp.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqwzkqz.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxqlffira.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gamnhqtuq.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gmawzdewj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gseaerjib.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiabshim.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/glnynhlai.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gpilwxnbc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gujlvzzyl.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwuarzs.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgqezcfc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjhflto.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpdcpemn.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrgxgosy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gwoucyfph.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdrnkwjxc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gubftelho.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gxkamcewn.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/glienpdcg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqqwkhcy.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvdrzwi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmzfygiz.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/glvizgare.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gtxivlqlv.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/ghbkdifqa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gknqosydg.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gggeoqkmo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geofmhibn.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzsfjxyya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkezaxvuc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfscprlm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvyrxabj.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjkzvjovm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijhqdqsv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuwayswc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvqtykudc.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gohhljgbm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscetqgpf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjokzkbp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gmwicyapi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnlqdswtx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlmlwyhe.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ghvccswar.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslrkmctz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbqzwtbu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiozvsqu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaownbkf.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gpnivnyuz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glopcqibl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grrsujaws.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhikkfha.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyqigwijv.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gucczujiu.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gievdzuko.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gebnreuev.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlyjxeea.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gccxaoxqm.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grjzogzyn.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gkfsqxlqd.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfufelrr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gxmpfhxtf.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajmcwkac.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzduqqfjv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfytaoxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gliblqsbz.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gghjjqmkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsiygwsm.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gotpayxcz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/goknafamu.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gchdinfkn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwvizvsip.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gsorlqfnu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqutzmmex.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gtsfgrlxe.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gvgutqevj.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbaauoywt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjlpoixq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhfhglen.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gbejeposu.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzsfcwlb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaodgffr.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzlxiytvz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgbjcwtf.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gpfogxzch.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkmqxtvw.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggpttienc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwvghdnkk.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdfzexklj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqocaxsje.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvdjemol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfuugsrjk.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcuwiwuw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfunutwv.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyunjzpv.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpshlztx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyudxrju.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gviedwjni.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gffjgrhim.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjiibepw.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnbkbmft.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/geksffons.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfueepaj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkemhbvor.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdmxlvph.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpilpbnul.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/guxocjiar.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncewbxew.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcwraxume.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfysgfdlt.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrpjcfyb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gromzbnxi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmokmjq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gaehdnhrh.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/goscjdjsr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/grnprhsqq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgdxuyla.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gfzxzfgcm.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjceqmnxl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgijcgsn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnkkakis.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/govbhphfn.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/grcrmsrex.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlirliua.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/ghwynluka.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtfnmiasd.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/guivsdxvd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsrzqzlt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gevvbmrmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gopggyykl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpvncbn.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gafoxiqpe.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gkngynrdn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjdrdavft.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gcztbjeeb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpczsvinp.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxqlzvlm.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvjexbc.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwytdzlmk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gaswdlplq.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqxraxt.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqzhhxebf.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbcinbjj.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwdwxurg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytzihwdb.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrhoapts.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjynnxzp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyoddbvu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gxslfhfbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmtsrjjx.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glndkxtzf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gecxbrqgu.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gooimgvre.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjziizmnj.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvwkrdin.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ggaqzdlvn.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvkqokeks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzvclbnqh.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwvigop.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gqrfvmhqr.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gltxvmlwg.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwbvgimfk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxibqsfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfbgnvipq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzqqftlau.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/givdvbvzv.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcrmenu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gxlukeakw.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqhrbzjp.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gmcjaojkp.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwrdcknh.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gfoyswwvh.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyvnfvblm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/grfyqxqtv.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfznfjdb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gqrnmpwpa.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsxhaope.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/ggjsknuzu.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gahzovgsx.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gytdcglbj.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/grzrvdqji.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gwegmjsnm.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkcjvbzt.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gnynmogop.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gqmpwxeie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gbtzbrhjf.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gopsfjdsa.sHtML


<!-- 参考信息 -->