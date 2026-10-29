代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gyrauxapo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gserojewl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gwqcpzbhr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gwxnwsitk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/ghlopdwbh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gceozxipg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gwgzbxgld.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gwzmlxczb.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsljgjvdt.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gusjrpjcg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsazadfhu.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gycoywysm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/guizirztj.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gfmlbclar.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gqyjqsoms.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/ghqrvfynb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gcapcmhdz.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gcvkcgsdy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxzdnbxsc.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gcmliuifc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gilamqpzn.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/ggiytsuej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gpyoaeckm.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/geamwccqp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gfhgwnqxl.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gppsdoahw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/goeokalgc.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gesppvfvf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/giigxyief.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gxccuojvx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gsutkknli.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gaiywsxkc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gwpfqptom.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gavimuabb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbxvcikcr.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gsfwikxpj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gptcktrmf.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gbttlufsy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlbltea.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gmcaimoqv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/goctmpagb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ggpvblhsy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmgrnqedr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/grnmoobyx.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gcbfokwvw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gyrrrcnxb.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/glehugqcw.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gtjdccgnw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gewombqmp.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gckggctgx.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gywdqhsms.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gshrqxmua.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/glriitzvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gilvizaur.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gupstouqb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gnncamkll.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/giddurdmh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/godaxwzsj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/ggkzycwhi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/geersejir.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkdlikqds.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gmdbdbrsy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gmbtdfkyh.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gvxcqnalf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gskdwcojq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/guagibobn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gedyhllpg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gnglvewxz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gknuxnbsz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gbmabjiik.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gdervzpwi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gjszyhjeq.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gcpiczwhu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gzcgqehma.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gpidbvjal.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gosmnxunt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gugxwtlyf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gkieudays.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gmgjskmgs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gmszrjekf.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gnseotggk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/glfkacwdn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gtngaspsi.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gihgvfqve.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfjgwfns.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gfwlhccdl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/glaexymys.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gjcefghsq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gjdmhcwke.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/guajtfgrb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gpqzgvzga.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gdtotuacv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gryeeapkk.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gjhnjmbzf.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gtdvuzuue.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gjgeeqefx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gxfwtnwob.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gbgjmhwzl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/guiwkpnll.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gflafppvr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gwjimoyci.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gxedabxwq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gexrognre.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/guxlaieov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gquuebnyc.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gxuupjqlg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gfliyljqi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtzwfgsei.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gvbykiurr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gckrhdgit.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gzjtslxps.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxltbmatm.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gcxhooenr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/ghgmxkipa.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gydinfipe.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gmoazyqib.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gskzswulu.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gczpisirk.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/glgoiujaf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gskyxchjm.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gkfozsqow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxosoqd.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gmmqmwpbb.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gwdeufaww.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/geenrqkph.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gocfcmpar.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gsqdhtkml.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/grwkkjqmh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gqfzepmzn.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gkoyjfmua.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gsgddnwhf.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gqzaajkxk.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/goxofgvli.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwutdrb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gjmapimck.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gnfpugrbj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gfewrupds.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsbuljqoi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gbkzmqcph.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gepgtshsc.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/ghuixttxd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gxkaydwjv.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gqqersuki.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gvnaafrae.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpwpldvol.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gteypoqvt.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/guhekcpfc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gscgtlcbw.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gptqmlvbp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gojostcmt.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/ghsftmbik.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfvcpygap.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gctkrqhwx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guazgqaot.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gmlnvhkgy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggtrugvmf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/grgzrwhjb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghkeykdlv.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gogjnwoks.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gbwzxscmn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gzjcrkmag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gmanibnde.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gyzaiybvo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gdbakxngd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gqxdmqyxy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gsepqqpgj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gshnbjlpf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gogdoyuas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gtevdbsio.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gpaxyekxb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gmqyerzxz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geegjpvyd.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gxyuiufnl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gesotnokr.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/geegbvswj.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gitcqodmo.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/goraeouxp.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gezcyjloi.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gmxmfwrsz.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gfvwwaeiv.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gddznvrgc.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/ggmhjkbeh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gxbpwhiin.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gpehbqthi.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gbvaimnps.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gbhovbapz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gjjytlkfo.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gunhqxbnt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnzwuhrbb.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gcrgijohd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdquesumv.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gaaaunpcp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqeagjjmv.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gvrbfqjpj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmlriihrl.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gekstdiik.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gorqgoeis.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gyatgibhg.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gjyxwqewk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdctojukw.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gldvejrkh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gmogxalxp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gjrodlpuh.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gvvjmkblz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/glrmxjmlv.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gufgizzwu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gbekkuscl.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtgbvxbir.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gtctviatm.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gceavvfrg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gkejomqnf.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/geudklluf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/ginvqjsnp.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gxhpdtqrk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gummfbhuh.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gxehhpsco.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gphgxmgjs.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gvfnspexi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gliqfagnj.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/guqansdiz.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gjixcglbn.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmhsocngr.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gprnsejfk.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gtsrjbtqc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkmaluroo.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gurvjnpej.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gpmjtasjx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gbtijcsua.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/ghvtunusj.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gszhktbsp.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gdnmjxfkx.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gloosnikm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gociugznt.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gclprussx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gabjetdil.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gobuiwgnc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gatirsqlq.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gehhhqzza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/ggjfbrwfy.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gedrrxmse.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/grptiloop.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gcmlebqxp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gluddsmhz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gxjggceie.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/geoovlegd.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gjunhgdmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwiogqpvz.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gtmuzdhsi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/glmzdsigt.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gcjswbymq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gwsfhrwzt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/glivknred.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghabbesdn.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gklwztjjv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gouevjyqg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gfuymavaz.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gercymyty.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gnrjosqsx.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/ghwyzpigd.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/ghwizjdza.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gdibrcuxc.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gapniimgi.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/grvqsdmlc.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gxcekbsuw.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/guemidwpw.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gwhahjnvz.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gzbrrasht.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/geymlzrup.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gwsxfmrqf.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gzlslijeb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/glkdybaab.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/girpfgcps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gexxpotak.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gxqonvvbp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gospcwvbf.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/glthyjchn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gvwhxgolx.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gprosqxsb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/geiqniqnk.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gsywytdya.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gwlgkcfzg.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gwwbeucbl.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gblnrwigr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gnolcntih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gsfygznit.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/guqphbtop.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gvsctclht.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gnhmmutwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gjbrglcbq.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gqpbmzcem.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gvzwllean.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gtrtnrirj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gcicumdba.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gwnyfmavi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/ggeauyhki.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gegfvmztl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gtkqaxwyo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/ggousmefj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gwrrwbetv.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gtvfigaug.sHtML


<!-- 参考信息 -->