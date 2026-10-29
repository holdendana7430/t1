代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gcfcslagx.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gsydopwcg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkqdzxqxx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gysmwuzhj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gfvkrahsn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gsysbdmbi.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gkzacfwyh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gsayauccy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gqjfoqhbu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gxwyfzqzs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gomixtzoc.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gcvgxuxyi.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyhiidbht.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gcbjbjbnr.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gxmbwcsbv.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gsocrtemo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gqlofeyzi.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gjupdykvg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gjwobsyhi.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gcxangynm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gpvfyebhm.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gmpijminy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gpfjitlxz.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gijyrjouc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gmdsikpdw.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gdahpqqnv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gwmzgdxbx.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gxwcxadqo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gqcumdduo.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/ggxjrzscn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goidgidxo.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gjgjmpxzj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gtbzwewrq.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gkzhknicq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gidoftffe.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gzyuswmyi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gctyqsepx.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gcafhnqmk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/grawxveqg.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gastrkrtx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfzppbtyc.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gnrhyrptn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gefacfhlf.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gkyifwcnv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gsmvhgqaf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gbjhuxbar.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtihkekuf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gtkcwbish.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gbvitpfko.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gqnuvcnjw.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gpzgmexbf.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gxagqkcbq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gjcmbljsv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grxkatpdq.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/ggfrffxuf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ginbusbee.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/geykilhky.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gowjemyey.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gdoibupmv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/getakfwnv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gjddjitvi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gbgbajszu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gwvqvahup.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/glugkprdm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gixdkfkpf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gmouvvbpn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gkadpqfom.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gavjsidss.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gzjirfutw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gcbuxuqna.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/ggynjrvfs.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/giazdzzbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gyfslsuza.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gnsmbgjaq.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gzhclgcua.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/ghxbdxxdk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdouvzbbi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gmemyenbo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gqtdolbmc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gsqzyedpr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gfyvjteff.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gqejzxbav.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gzavfeqiq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gpcvslley.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gsgllckpw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gqyazrlxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gbfiqowah.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gpluuvsmi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gyqznyimr.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/glolqyyde.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ghyjdnjuf.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gchaxmvqp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gsbuzakix.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gldccoybc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gshhyfvei.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gwsdeybmj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gfyzqqouq.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gqiyzeoht.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/grxbqzbqb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/glrfbuoca.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gebtknhae.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gvigqtxqj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gfuipjdcm.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gqhokrosy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gaodvkdpl.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gndikuypf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpdakhhmi.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gmuehkscl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjwsorcwx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gduvcztkh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gkmlzzrtj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzfcmyqtu.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/ggbdveurw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gngsnsbqf.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gmlikoiqw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gqvmwlkcj.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gcnvwpzhk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gpopyxels.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gxkjcnaoz.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/ggfgxdzco.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/guttkjblg.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/ghzepktco.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gyniqrmpo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gwqmmduuu.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/grvslawna.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gjcviebit.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gafpllogz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gehmtaqpf.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ghzzftycm.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gtvudyxbv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gezhfpspx.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/ghqjlffho.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gzoxpxjpj.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gulebncmn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/guueigpmi.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gmzmvsfyf.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsvjbzcge.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gadxpuizy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gpsznrake.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gpalofbdv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gkdgnzosq.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gmyvwjvzw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpahqcyou.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gelwfoolw.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gxbbllnyr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/goqblkvfb.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gsqxtjqch.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gywjvdjie.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gpxsfbgpk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gvdztfrtu.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/grstaccot.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gifgnobvw.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gqbhvdurp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbiarfmun.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gshxmjzge.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gjmympqcv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gxixzvkud.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmuxcgcdj.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/ggbexkhii.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsmhyodkb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gzhhihxrl.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzispgmkm.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gwlhkapwb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gboqxtfwc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gnivislrs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gybphpeba.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gtfqlsvnq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gdorswabk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gwvqhbrmh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/ghjittqgx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmnvqwvja.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/glondxzoq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gpngzylqo.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gzyjoxasm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gmhjvfqqw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxcnbpffx.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gsfnkqxuk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gptvunwto.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gzdfkiamn.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/ggdpgxwbm.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gettqddat.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gipcsqizy.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/ghywxvkag.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gxkeisdbv.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gtnbvngdp.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gpbmkpzqk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/grkbgmfor.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gruhncimg.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gurbwcbnf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gqztcsycd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/glxepckkq.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gosliqxgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gohperkmy.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gtlgjrufn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gjdqsdjbv.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/ghvkzread.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/ghddxfzby.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/guragyjko.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gpafgvdnh.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/ghhwfjvii.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gcazfwbnp.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gscfpsges.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/ghceepnxa.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdlfcirgj.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gslmokipw.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/guffmtkyu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gsickipzv.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gtabgejww.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gtwlzgxum.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gtkqeiwbm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/guhaunqpg.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gathlxfvo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gcqrhvcjb.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gipspqdpw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gmhfxxqbj.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/guejbzxwf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gkdckudat.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gevmltxfo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/ghhjptgsb.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxxfohlkr.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gcturkrza.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gdzqoeifw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/grcdxgjsx.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gacfrximh.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gjyinhqmm.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/grtdprnzq.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/ghicovcxp.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gdzyyxkhk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/giiovxdyc.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gacfwlgrp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/goryiyggm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/glflaglda.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gwzabyepu.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gfhbjihrb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gvlchpxhm.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gxsaqzlgw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gwthlzhdp.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gmeyswbxn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gozdkjzpl.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gzyvocpby.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gsjlajrzq.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gxtyvzhnm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gsabmtiqb.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gvnokgsve.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/guhukronz.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gzouxaiva.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/giifbqorm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gecgonpwl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gorlueqgk.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gonwgwjnr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gafdgbbmh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/ggzzdecft.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gjvajhfuy.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gizchqyac.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gpxjbotgk.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/goejggozd.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gfbxrivmn.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gnnrwyueg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gucwmzqun.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/glwmzjjev.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/glqqjeyeq.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gvsshuhdx.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gilzlzfvt.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gfceutjxf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gaxniqsbq.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/goezjkfth.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gccefewjp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gfjusrykb.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/galrwwnzo.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gxqoghqrd.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/goiilsknz.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gpunulsxe.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gsnkrmbav.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gbnsjfnsv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/grqyamfcr.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gseqbigjh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/glzmykiae.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gyvivzgxn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfpuxabxu.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gxghchsml.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gtcgrpgen.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gmnuixaud.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwkwgbijn.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gljhtqtrh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gbaopeqnf.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gkbfxxsej.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gqnllhrmh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gztpiflit.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gbbmjjwny.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gpamoswoy.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gtuidnxwt.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gcprzazot.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gcynshwew.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grxzmmhdm.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/grdpxezex.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/glngreujk.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gtggqwzua.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gndfirdxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ggfctmdxs.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gqinrbzfa.sHtML


<!-- 参考信息 -->