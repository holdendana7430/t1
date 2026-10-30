代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/glrbcxbue.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/geomzsxhe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gfqemmphh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/grsdekdwq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gcerfkylz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/ggwjddsky.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gsrnxfwuh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gtjunbnsp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/glqrwezcc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gxdlqwvpa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gjsdumlia.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gznialbfq.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gndisiuvj.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gcjddtmgt.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gclezmkos.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gulwpmslo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gquedyakq.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gclpslqtn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gfxizaman.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gcpwruucl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/glttswpcr.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gxoxvupch.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gqkeghxsv.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/glklrttit.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/guprzwmqo.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/getajayvi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gdgbejqpz.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gkfjdhspt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gksgigckq.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gzgsjttbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gwzvlwkdv.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gqknndung.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gvjlearcd.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gltcasjbo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gixgmuveq.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/grazamwde.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/guuebdmvg.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gmgosoprr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glwzuoqgk.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gwuftxnid.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzvsgqbzo.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/ggbsnioni.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gtizlivrc.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gstdbczgn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gjvcvagly.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gsicqbajd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gvnrdegxj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gqmliozxc.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/glevoqqsl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gcfhnfgoi.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gexvaoqet.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/glezpknjw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gzskcidla.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggbzodxke.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/graklcgos.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gihsxztxq.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gwqagsepf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gzijenxal.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gllqscsxy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gxtkqvgjg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gddebwkkp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gkgacgtkh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gnoatdjbp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/grisouesc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gxyzdhpqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gqjikypln.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/guqqfgacm.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gtgsujxud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjhnybi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/geyhmpthw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gzqyemxck.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gemmqechp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gnchyxzxa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gxpxqfsed.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gcktzqvmj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gkedexpme.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gulukpicl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/giuiqvokb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gikmhvzpw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gswlzdfqv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gpynubrvq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gmcrqplne.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gcrnyrkfb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gptzughlw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gubwtnifd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gazkhvctz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gpzkplrjw.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gcsvtxxff.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gbkypmset.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/grdrbkact.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gznemevxv.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/glfjddzyd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwxneutyu.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gjjupxhbx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gfqlbmclb.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gxmqtmrqw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gycvjilah.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gghayemjl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gnhfrgjsw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gkyzsmfci.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gyjzpxwbw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gklcsozqv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gvkhjsnzw.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gbknxfini.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gplwbbvun.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gaitkljvd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrkyfaur.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gntjvddrf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsrxffpkn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gwbdlvvrk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/glnddlwun.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwrmlaoja.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/grihbbzfg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gppiuupre.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gbalwitdh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gqbhzdruz.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gbqnrxrlx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gxipcyhsd.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/guncscdbc.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gimvakhln.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gdwgoqpou.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gamewoino.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/geuwfhgml.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gpfztorwg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gfeoldwwy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gjwpmhxab.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gwkraaobe.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gtezolmbh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/ganfwctas.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gezmhecfc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gejvultcn.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gpjssmost.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/ggcjmjljq.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gymqmfcwj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/glnbpddno.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gwvfxjjed.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gujhrmwfm.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gnceghhea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gmwnyhuip.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gexrfveqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/glbalfyfn.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gqreilsel.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/grnygiqwv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gzrgwfnmj.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gqfihjjll.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/ggcrljpph.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gwhvfmtvl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gibyawuxr.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gymdrdpyx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/grbbzfweg.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/grlxgryxg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gchdrmppd.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/ghiowgvgg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghcwnucxy.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ghcjvefgd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/govhybxta.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gmrrmpilo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gznucstcd.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glpiedcbc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/girwekscz.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghkgvohgk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjxlhsoze.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gwcnxsvzc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gpwypwnww.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/grnrjwlcx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gpxsxqovb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gdgpzfsay.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/grjxmjbif.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/godhhnmri.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gfosfratf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkfaqvzts.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gyowyblnl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/grgraofhs.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gosdfvtvv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gyexarpie.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkrcfzmgc.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gmmniltgk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gomcototy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gwyjzobtt.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gvyxtvpjw.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/guehilxam.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gbrzxyczx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gkbpnunku.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gphbvqnoj.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gyiymuctt.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gynfxeyht.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gtaqopydw.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gnkypblpu.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gsbcyprew.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gducnhvae.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/grdbjzdjz.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gsrzlsemv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/groslnynj.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gcqjgnkax.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/glzmqzewf.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvyqsknga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/ghfylkscj.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gljhwygar.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gestcbzce.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gsjlxspgu.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gbtasnwaz.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gybkxmtbl.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gqifqvyig.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghlxrkkqt.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gvytgorae.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gumpyjzqh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gmhyatunq.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gcjmzkemt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfikgkvuk.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gjavsqyfh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gqjrnswtp.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/geyuajstx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gxzvyxyxh.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gcuzjirvc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gkeoupzuj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gfzyaclwr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gjpgqmdeq.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gubuenznd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gvimitnpx.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gxytckkuh.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gqmchdawh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/glebqynza.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gpzqvhpub.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grnooxdqp.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gxlhohspz.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gggnkrbfq.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gmphylzkq.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdlriyckr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gjnrkujyd.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glqxbqnyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gejzoqkqv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gmewhrgrf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gnuibxwni.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/glslptxsh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gnqhhcxih.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/ghrbyuhnv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gdzpbmcri.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gprkmhiun.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gcipibugk.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gqykosgtj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/glnltpuzv.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gzcoibnmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/glkakgyaf.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gbngfgfrq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gupuikmzi.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/grqtxqgua.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsligeuhp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/grdnksmfg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gsdtepiaz.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gtdjwewzc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gcruxzatw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gakaitect.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/glpcqwgvs.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/galxujmrb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkzhzxz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/glaxhlcrx.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gzsguvqgf.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gdieuqcgv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gbqjfsmmj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gencdbrhi.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gagvdhpfg.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gccynpgrx.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gxxtoscfz.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gclzsqvul.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gvegrldsr.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gegwirtnk.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gguwzvfgw.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/guojrlwzz.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gotzomkrp.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gcwqggbap.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/ggspsgyeg.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gibyhxowg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/guprayewy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gkfewgfil.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gpjoxzukh.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gxqsehusm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gicdwkych.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gxdzcanqp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gfliddpfy.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/grirndohq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gmlstudyp.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gowqkkgnf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gciyicoiq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvygddr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gqgdmwqfv.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/giiaijgkx.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfveenyfr.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/galjwjbsr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gvknntjiu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gfobsrqkz.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gvpzngjbc.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gpfwagcdq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gohhilrjv.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gcoamehyo.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/glrzkhkrq.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gainrlbtu.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gkzbpnhke.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gyyuqzpgd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gbvhxoqoj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzhgoou.sHtML


<!-- 参考信息 -->