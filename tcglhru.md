代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gqlgeyxrl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gxphahwtq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gabbunrsk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/giweiajpl.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/goknvhohc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/grpgfvuau.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gmkjvfmqu.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gbitzlsta.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtzrnawrg.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/glzrlxheg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giapqtkgl.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gkpqbfzmu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gbjwmwgvg.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/glibhoyra.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gzcisfjtn.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/glgzzopmx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gxfznwfmh.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gxmlxmwai.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gczdrubwc.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gckmwzhez.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/guxteskzm.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gymojzwgo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gbjmtplwi.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gvmvnbqsa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gdyfbwpvv.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/giuipymms.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnhjtyxyc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gdmqvfjuz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gsklzzdtt.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gmpdqcwfb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpommphgx.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gdihdjupl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gctghghjs.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gdqcgqbfj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcvosygws.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gogyzglai.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtwuczyvb.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gmbkisxfi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gdlrtapfx.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gpfiselbo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcvzduftt.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gfgtwytws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gzhvxanla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gkufvxiuq.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gjlfkolov.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gplkxihdq.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gqsomctbs.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gjtrjcmxk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gxqqjiyjt.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gkiekqtof.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gkidyovpj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gxbhfzxqx.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/getlvtpsy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gtfvphrxb.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gqkemccon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gfwpsxzps.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gquytvlij.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gnhfzuvxq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gabknniie.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/geljaigdh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gbeewqajp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/ggwovuuot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gchinyejz.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gtrypcfqv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gavmpzedt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ghlnnbagp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/glqdxdflj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gosrnvjrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/giptvxphm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/geqihyqec.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gmmveuitz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gajaslubb.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gkeichgan.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gzwatgsbq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gjofcxupb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ghcpxeayb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmpgcbndf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/grsmtfsfx.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gupothujb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/goasdgoxj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/ggydceqpk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gtixyigrk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gkihwqenw.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gsivteism.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghammwkym.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gccpsdeed.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwdbrortm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gxsckawfl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gyidnkgwx.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gcwbetymv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/geprmvmxr.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gaqtnhmdn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ghxpcwbom.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/goxrlhokz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gqcdjohhs.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gwhsqnfwb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gjglertor.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/ghfleipvg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gxvaeijnv.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gofxycrvi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwubccmvq.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gkvdwhtgn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grkzcldiv.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/ghncklezw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gacnejwcw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gfhybyswg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gpmghntuz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gaaoioggg.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/ggnorovge.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gobpuxuuo.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gamtmzshg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjspdqrry.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/giqwvebjw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/grirpdhyv.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gffnmzwes.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gwecckskx.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/ghitnjedc.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gzdebibxb.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gcdxxtvwp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/growcpyju.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gexkxhkgn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gofxjoccm.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gieqijljx.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gpjtysnpd.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gvwzxhmhj.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gepbtjvnw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gyybwstjg.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gtwcpgdmm.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gglfzmksq.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gofcadgct.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gxcjejrph.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gcjfawzgw.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkjpoiopj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/glggqpgwe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gszoqdzol.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gddsoihcr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gnjtoyhck.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxxennjhb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnbipcwhl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gbmhlwhtu.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gsrcpoiwr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gjuystbbp.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/grnsxlzuc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gbfzllinq.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gwnpafvat.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gfvfynjid.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gsxoervbw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gyckyssyw.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/guqfmbtmg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcxxuxeqa.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gvkstnckp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfbqnaasx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/ggjuxjqip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbhwjbxrp.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gjlydeypr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glumpnnox.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/giytmnfts.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmzlbjakm.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/glpfymemg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gzfkghkrd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gsrpbyelq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqlhxno.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gottrqrlc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ggkablrxe.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gehwbqkxk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gsxoopmaw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gojuilbdf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gbltgyktr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gccdfjrky.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gtzkenxzh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gmzetupwg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gubnqgatu.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gsfhduyhm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjhubba.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gjxtqbjgd.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gcgvbtqmj.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gnfffaowt.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gdvkmahql.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gufybvorz.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/ghkcjmils.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gmaukfwrd.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gwhkasall.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gjssniccx.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gmevpkpaf.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/glvpdhkvl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gtvaswgck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/ggfzltxyw.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gnvjkzbji.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/ghuiakvou.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gmoijcrmx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gzlcebgod.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gbsgoofpl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdqupzzvj.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gseiibkxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/glumxupmv.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gqsixnxjq.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gyylyeebr.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gpaxuqnbb.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gsfqtarmz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbfszhfpu.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/glbnkkwmx.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gdjxzicez.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gwqtgrrrs.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gavvyxxxd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gyuxyuwpj.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gfrimplvl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/galxebzlj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvfemtlxm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkgamawru.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gxvfyoijg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gbpfzfpyt.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gbnqmeaxm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/geczwbkhj.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gxfmhtaqp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gxykehrtu.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxdojpzoc.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/ghafleapd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/glibqvszy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gzxkffifc.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/guqaizqdu.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gkqefansj.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/geonkzufv.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gvpissmaz.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/godtjsttl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gyrytmsyc.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gfvxqytfa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gscwqcjnk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gxeycpvpw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gqpovvvqi.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gavmfjuiu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/ghnzunvkt.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gayshoxnn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gfgaqdwgt.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/glwtehqdw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gqofbymoa.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gqhwqlkqg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gjbdrvrqd.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gruihmarr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/glhioedfb.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gemmgvevf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbrlzyvqe.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gsxtmahht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghgtvyknj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gjoetqidm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gabzembup.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gmpfkwqxn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/ggvmwsubm.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gzibevioc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gfriotweo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/ggqmdybpi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gzjajagqk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/guenyjjqu.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/geumbjsfw.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/ghrtobaof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gprhvlxwz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gohzhqgkg.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gqutxnrll.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gktvvpabr.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gusruzrlk.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/glzzrtusu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/giyxqftsw.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/ganffaxsx.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gahjzqeim.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gyfkcbvwg.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gorxljlyf.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gdwczetpa.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gbpfgmqoj.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gwnqxgkus.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gaojpjaik.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gvyqlxppo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/ggphigiim.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsrnmomms.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/guvoqejzm.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gpaxzegft.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gklzyrfpt.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/ggpthilox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gulfikdmv.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gqmbethfy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gwjheoiva.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gzwkiobtq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ggbtqcztu.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/grpdkzwbe.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/ggaxfbrhu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gsxymfshy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/geccgytww.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gxmqdybpp.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gbnxlsraj.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gvipwydvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gfnkkosmm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gzqxjyael.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gnsdakoxt.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gyxmopnpj.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gnkajpzel.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gzrxkslku.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gbspdvhgd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/geomhggyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gbvvhjpqf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gnxckomcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/goaxdbapw.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gwtkjfppm.sHtML


<!-- 参考信息 -->