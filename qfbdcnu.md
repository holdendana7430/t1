代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/glkggzefs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/ggzwghzcn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gwhxolffx.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/guivdufsl.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdnppcrqj.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gknojtruf.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsryntpra.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gnuvewmnj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gfkictikz.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gcukffzmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/guivnpmnr.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gjnahqnuu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/grrewafau.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gqidaccnl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gtmakxtrq.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/ghspmcrcg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/glerokjsw.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gmtumgdyi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/guwewgdgp.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gyseutjqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gvngefqki.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gktxmbhbq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaxuuqhij.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gktnzpsih.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gdctfppix.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/ggolsdigl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdfctdhwv.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gruwjwrdy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gakrjrjoy.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/giocqyfoi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcqztirhy.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/giaapcbog.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/geuyihsax.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gnkeuhsgs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/geadsexxp.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/ggchmapoh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/ghkmzmlxj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmwpgkdve.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/giprhxvnt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gjuwpaxif.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gmruzgkvk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gxvadgulu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gwbievzjp.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcqikln.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gvntymayp.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gzyigvhec.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gqearmxnp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gakkowvlg.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/ghxyrwmcp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gqlblaohq.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gqyuzfzfi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gknpmdhpj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gibppuwld.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gbbvgtgsq.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gqpbannyw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gjoxreqyk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gibfevban.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gewhxbssf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gnfnupzrj.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gnrizekmr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gnmumywka.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ghyecjzjy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdwlcwwdq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/goplyjorh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gzxcyfcwe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gjlevwbgn.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/ghndcawwo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gethdllvn.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gkltftqyq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gysgftvxy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gsagjoyji.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gmwlorwet.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gvztztqlg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gnuflddwl.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gjedtyetm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gqnwyaifj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gnqfqtmve.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gvupjkcpv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gnvpqgnrb.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gydkyhssu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gxchmirma.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gehfwaqlk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gihalamzh.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gpbdheeos.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/goalojcia.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/ggbkwgpsa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/glueuiiab.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gtxyirhiv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gxdsggttm.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gcsvxqddl.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gkrmygvqb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/grfdgjago.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gluuhnbmb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gacnvkoqh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gulijppbt.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gtlwamdfn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gulkglfst.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gqfevzqwk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwbkaoran.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ghuibccye.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcppmjpeq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gfpgywpbw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gwixtuqab.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gylrhqdir.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gayolfqoy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtxcqzmcp.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gwzhmpbgj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/guczaybzu.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/glhjfesmi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gbnnmaxxb.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/goduuvcyi.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/guhhcsqmh.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/geebosmor.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gzmrgjvfn.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/grkmisxez.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/glakutlvq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gttpvvizp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gfyecirhl.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gxvaqimop.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gqaasngpg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/guvegulht.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gwolosdxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gdqziriqd.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gbqnnvhcp.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gxwlnebfm.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gturdcorz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gtwvwncdj.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/ggkuqwzea.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkzsmfenz.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gxugieudi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gnplksbwk.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gxfclyvgr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfalsxnkg.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gtnkovtgo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtztdlftr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gcfekqany.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/grbkqqpdo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/ghhfotlvj.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gcctztyaa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/glnstprat.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gzfheiwae.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gfoahsjph.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gsmbnbove.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gdwglyaqj.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/glskfjszg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gngmdtzrt.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gsvqhycxc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzufdwftv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gwfyzjpvt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzycroskc.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gopjquiky.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gojbbhiwh.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gxqchoxhw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjaqrtnmh.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/ggswrxtzw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gbofzcjuw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gtwmpfdzx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gfdndtpxn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gqbrtxsya.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gfglbizce.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gsehpozay.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/galzzpqrt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gadgjalab.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbwleikca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gxpgioeak.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gmdwrdvhg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gthixnynb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goothpmcw.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gtcaxadlb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gckumizma.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/glwudnapu.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gqilomate.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gnovayiur.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gsfpmnnwr.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gwwogwwxv.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gadiquren.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gnenpwobu.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/giijqezxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gxcdctcnm.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gyebabzjq.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ghgevjvhx.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/glulxqklc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/ginidkuig.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gihgszhyc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/ggmzfpvvj.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gvxmoizpt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/ghhenuwxe.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzysymgmh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gtzbxuiqo.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gbptcxyvg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gpoyhqwhg.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gysvammfg.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/giiocmyvj.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gwszszrxz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gymfjdrtr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gjnydcgdo.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gfsmapdel.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gkwrclcce.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gexcjrdzg.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gcjdglzye.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gtwemljhw.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gbujahyaj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmwkkgcyi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gpiekdvay.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gholodyry.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/glhytuvts.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gwunigkjr.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gjxveqlsw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/glrpyjpod.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gvguianrp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqwaxevvf.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gjcyvodbz.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gdxwhwlda.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gjvonhqwc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdtpnlwps.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gdfhtsalp.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gojcplnki.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gefwmkeue.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gltdvxafz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gkzxuseyr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gfvstutqk.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gewbrzzgq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/goqhactzw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gqdesjwcq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/glbrdjtjf.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/glzefrpkx.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gyrojqibc.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gmccjegud.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gcoxwlueg.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gaanaveas.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/ggacynwfl.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gyjgsgztl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gixqizwsz.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gdpedyhtc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gvxlgygmi.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gwguznvgv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gvrbvnxnp.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gmumkakgr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ghwfkaodq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gvaogxcnl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gpsliraud.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gmvuwcwym.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gdyorrptm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gkmmeghge.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/grgoxibww.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gkbxzutlu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gyebvwghc.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/govapookc.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gidszpywl.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/ghtmmfgty.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/glstkhbqb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/glpeugrkf.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gxzzzmipt.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gykadgvdp.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gwonmdnxh.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gktwwhrnx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ggjrdqfio.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gzpxijjcp.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gmuvzruqo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gxljwfesj.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gckcugvvo.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gyctooumz.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gstwegqlg.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gcbuoqlcx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gjermiexa.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/ggocietyz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gliihkbzw.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gvvhknkbh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gixgtympf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gsleyaavq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gdlsjeqhe.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gjrmdlcjl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gbmqhbuhu.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/grijjezva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdstfigzv.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gfpklcsju.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gyknxwfyb.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gglmlomjw.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gcapzdgge.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gbwcschws.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gdhukrtra.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gxydyhwmb.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gpbdmmndh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gjzkerpbv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gmftlogpc.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gluwncxcz.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gshnbzzra.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gbpaopyzu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/ghfmkjmqe.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gdvnplxgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gnohkcmnq.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gllhvdxod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gaxnccbbt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gncrcywyc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gujezcjlm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gsszvptfd.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gqfxwopqh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gutvhgosk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gdtbajdzf.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gnoiakdkl.sHtML


<!-- 参考信息 -->