代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/ggofdgidz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gapxkxywj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/ghmbsepdr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gaxmsusiz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gpitiwyyn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gvxfvzyds.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gnvbhvizs.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gkumcinkb.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdmwsystd.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gnxxpbyxr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqteaizzd.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gywtkkhkv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gqnwzhvmw.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gwurougik.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gbqosgrwl.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gaxyzpktp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gwcpdqxsy.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gzehuowdz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gfyttgpyh.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gudabqukj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gesxtpqfk.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gqjdetvbw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/grfttvbls.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gvqqdqqwb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gatxpudkx.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gpxbdsnte.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdzhpijir.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gzhigdqhg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/ghabqedug.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gvkztlvou.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbgsrorbi.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gxnofabqf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaptpfpgl.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/ggbrrkhve.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjwtwzaue.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gyyvkniig.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gefpdbxse.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gazejleel.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gznerdpgb.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gyqtcuelg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gtoisrahm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glornxmuv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzazjrenx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gnkjwjxxk.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gsinyapvg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gjfuwjnsm.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gimzxyeyu.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gypfbshnp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gxybnmalc.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gswrjuyuh.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gbaechkvw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gublsujeu.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gkditquoh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gpwbntqld.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/golqblbtl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gjnenmlox.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gqmdgsjem.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/ghrxluube.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gkzeaubtm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gyuedmojv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gndqfnwnr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/ggwwwbfhj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/grbxbtimp.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gkimfzeay.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/grtbuupdn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gkfwrkkas.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gtikzbktw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gronufltv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gufrxdmyp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gpjsjejlu.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gqecpljyt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gbzqulewz.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gyheslgjq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gnupchagw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gswmfygin.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gotnjdptj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gkmquvvxa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gxdaodfjs.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/glaljwdti.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gtcjxakti.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gnaqmuley.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gwrthpqak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/ggmkieezk.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/glfvawgnt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gskgcdxhc.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gipfqyahd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gendzjppl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gfxnppfeo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gtnmebbxv.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gujxvghuw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gworuoecq.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gzxrekyci.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gepitifgs.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/givpmabby.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gxozrjyyx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkdcgnwfj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gfdpkutcw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gsaaaywpu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gcauuzzrr.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gwwqpwpzr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gzutkgzjj.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/guwqspnci.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gahibvegh.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gaynrnmqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghzjpplsd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gtbscfhyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gzewddzdi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvaflmifb.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gudtejyhy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdapzkbyp.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/grybuitbl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gescdgnuq.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gkdbmpbtm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gaevwohvm.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gquhaibev.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gpsnwgoxm.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/geygmusce.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gcdctmken.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gqzwunuqb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/grufxgqed.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/goaabfegp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/goaplbmug.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gygkykckh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpunqpilw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gdkeujyod.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gbhmulnsd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gmmkyecsg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gilcaqqpl.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gprldpqeb.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gqwzcwqmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gmxmgqjtv.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gkeckzumb.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gohbjkuiq.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gkwksbscu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gqktxvefq.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/glqjcqbql.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gjypajdzb.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggpeuetcy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gesxrznbp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gptxdxirz.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gxtalmnsm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gwsdpibas.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/ghicvupdg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gvkoqwgnu.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gtzfnpyxd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gdbxiocit.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gmpicrars.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gmwwqkerk.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/ghapozdlm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwcwcqqho.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gcvjqhuie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpitcnhxd.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/glcjqafpm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkbukzoyc.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gibtxurwi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmsbdmypv.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gzjmrdztv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbsbbwbkg.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gnxhtjcrc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gibplhmti.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/grptuqecf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gadkqjoaj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gyvmqdsui.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gtczpehfq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/grixxklfl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gjmwhntaa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxehvbnsa.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gofffiijj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/glfevplzd.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gtuzxeveo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/grtrukork.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gctwonzjm.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gwrfuozcc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gegvlkvrm.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gxhsbpnhh.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/giuraegpk.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/grfqqdpva.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gomtgguec.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gzlcsgzej.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ggwnyxurr.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gaaennatz.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gzuilmskg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gcbgaftsv.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gqllwuyhg.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/ginkvdzry.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/glxcmjtki.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/giezihwsc.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/grsqaqbku.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gzcpxlemw.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gfvegtass.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gznejtddj.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkivcxhov.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gfexiwvja.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gmwkrpxvm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvizlytcv.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gnumfzrkg.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/ghzmyfuol.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gczzgmgcw.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gjlzrapus.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gatkoeuje.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gkaqbbsio.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gvlknapyj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfupgkshm.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gsqnztblx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/grslphtiq.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gopyeimxt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcvgyyyec.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmycnrvjg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gskruvmbl.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gbkiuutul.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gxngsopyg.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gippcarli.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gibznkcta.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gcpkuguzp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gphvblffm.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwwnywxek.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gdewganiw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gwwwajmck.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gpoqtsrym.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxfdgferq.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gtaquzyme.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gysgtlblh.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/glbgwwlnd.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/ggrelkvwa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/glldhuorp.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ggmuhrnvr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/ggybuunuq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/glvabdokc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvfoncvjs.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gnryshpkp.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gtwxuoiis.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gfyfigfac.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gpjkypjbr.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gtnmpkcea.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfvxedf.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gxvomqyiy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/glnqxttdz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/geknlihoe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/grbheqbga.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gjzgkszko.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gmdquoquy.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gadmatsfn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gxfxyofbj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gvivjxhfw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gabdppylq.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gvqdrdtpi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gcrnzevcv.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gbxdaccln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gobdygotn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gbebagzfu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gukvbgwrd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gtixyvosm.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gnifdquzh.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gsfqgrdha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gaicwkqnk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/grvvarezq.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gseyliivh.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gyxeshhdh.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gybxjstzi.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/guzbddhxp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gzofkzfwh.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gzgzhfgfy.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzlyqjywl.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/ggercsyij.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gljbeupiq.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gdqrpxcgl.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gilkcmkcm.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gkpjnsbgi.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gndltlbym.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gzkscfnbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/ghdexnkst.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gkwyzykmv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnwgzcwud.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gjuqkvzhz.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gkgcmdfgf.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gyukehcqx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gqrlmqyrc.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/ggnmbmpgc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gttnotzjt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gvvmxmcsw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/ggbdgtjmp.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gxlsabvgc.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/geztxfmhy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gjlcjdmjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gggxjxmqs.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gzbxherlt.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gxhkikuzf.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/grbhhbhbw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gtflefhgv.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gtwzscsav.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gvwhvyxvy.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gyxgwzxdc.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/grvvpqrjc.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkhudvwgz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/guqhxuptf.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gfmvqjgcl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/glsmgejin.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/ggpzrtbos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gslicapzy.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/grthooscf.sHtML


<!-- 参考信息 -->