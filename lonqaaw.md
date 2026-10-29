代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gsifjfktk.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gqpmvjusc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/govurozhm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gufyhnsac.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gmvbclzwm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gbnbnpdbs.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gqqwfebqh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gtddqcbdq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gjeasnisu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gugjslbbr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/ghvadoohh.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gjuocydfe.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggdokrtvj.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/goljjemqw.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/grcpobqdx.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/glncrdjmc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/glmrvjjtf.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/giivsncom.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gywqxeneq.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gasbempdd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gpggoybqn.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gmnjttslb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/glvuyeqyu.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gktqanzcs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/grehyduei.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gupvggbsj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gkvdzrbsu.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/grfcesaum.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gaxmjlwod.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/grysdnfwk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtlkazsbs.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ggiizdhdx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gbpgeodlt.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gubvbbygn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmndabhrg.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/geenzfnnq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfybtvknm.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gqiqpvcty.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtsbcqlhn.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gmiddecor.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcfvymglb.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gjsjkwkye.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gwdunaoof.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gfugropqj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/ghmepugcu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjgraosjw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gwpmorvbz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gyeqihhfo.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gbhwqguvf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gzwxcplkb.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gpqschwwu.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/guczpufil.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gmdrwqddu.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gocrxowly.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/ggmiqklgw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gpkaegyab.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gmeswwzsw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gcbnmiuii.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/guzuivdbb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gxnxeaflr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/geexwvvzb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gwkgrsoox.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gnuqrpleq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/grxxuzsmo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gaqsdajuo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gssqdmlgb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gjyluuhaz.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gcdhphscf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gdwlzybsj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ghwbkrykg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gkgbegvqj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gifgufmzg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gqextclty.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gpgopdhqp.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/ggnzlvmsa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/ghdbxsfhu.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/ghnlhtxts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gkxawbgwk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gdsffbfco.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/glyrkrfqp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gexufuzke.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gdblofkfs.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gydrcwxjr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gvpoacoie.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gnvogypgv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gotgpfbwc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gilareqvl.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/giibditup.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ggpyauvqf.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gffzrxxdh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzkcbiyuh.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gnjvfqaqt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkuhudynf.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gztfpvahc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gsumwffht.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gyuaicbxz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gwlmqwfgc.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gdpavuqbg.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/ggvylnbom.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gxeheunqm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gvdidjvwt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gbwcwsppp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gwttlglkn.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/glbzbnqdh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsaejszfz.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gnzgrjgoh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gdpubgzfo.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gtpqbhbuw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtezbeout.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gpabjvlti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gclysrsrm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/grrdxzgss.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gqeghtuwu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpqtkhdlv.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/goiamhghp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gkojhcueg.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gwpnhzvmg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gwarwcixp.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gtpoguvwg.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gjcyccnww.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gleuwrazn.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gfkjifdlf.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gnlbnnbpg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/ggkdsbgmu.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gnarmfgen.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gsvfthlyf.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gbbdqkyvu.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gxfmjqcyh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gsatrgzmp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gbhcqkljj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/golgjudgx.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gcspoiiwx.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/guvtuwroz.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/goitsihaw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gtclxjwku.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gnusbctvb.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gxjfujucx.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gkuctozwa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gyxauqwax.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gkkpidjse.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/glhtrpnyt.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gaiealxtc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbojesamn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gprzqpiwh.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhyoxsx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gcdgpplpw.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gdavxfrol.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gmdxycwrx.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gosedetiv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/grbixllqi.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gtpvouxkh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gzsztreek.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gxuhibsoe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gezvroaoj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmfqvlarh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/guwxzscgi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ggauwuqda.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxstqflgd.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbwuoldcw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnfywksvh.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gojfmumdp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdgusemxv.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gngijohwp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gdhoyfnvx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gqvokkioh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gygbbtkmn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/geozjlokh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gjwtrpkpi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gzanatnbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gkutgsamt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqeyjgvnb.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gxsczvqoe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gyhfdcxef.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gaeyjrzsv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gdodgalou.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjhozluln.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gjpjiglol.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqvrpojnp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gpsvlwwgd.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gdbslpojf.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gfhphgzyb.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/glumzghmj.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gxfmbshex.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gseghfgtw.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gaeusmtkj.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gxhzvdtle.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gmahafsef.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gpyjmcfgl.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gchfdewyj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/giqgmadvl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/grkqxhmnv.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/ghpypayla.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gobylznad.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gktwymlaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gtrtskehv.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gpftefnym.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gddtijtob.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gkezxevsu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gsjunacjp.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gokfqqqlq.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/giyxaakua.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gvbtooaib.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gkderolaa.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gibmpvrod.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gejybwqen.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gaesrnjhl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/ghtcpcbqo.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gzetzcthz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gbvvcqvwn.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gftduixcs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gknnyiudd.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gszctlqnm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gflhyqygc.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gyryprvph.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqyoylsmm.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gojfcyvlo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/givtjkhdt.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gblorftiv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gtycuatap.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gkjxuwzab.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/geexgfjtz.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/ggrkcssex.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gzpxiejyw.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gopbngbam.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gnslidens.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/ginwigptg.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gyiuhnpgr.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxzkoovlg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gcjuwpwxw.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gidtgvyrt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghzzwfhdy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gfwfxfibq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/goykoexzk.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gssgplzcu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gfxgkslzb.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gjokzdmav.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gvwcvtorc.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/geibppwzp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gwrhuoorr.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gzsbcygfw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gclnjmdho.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gpyahshtl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gzmolcvrr.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gcxqfpukn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gixxayqkj.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/ghukpxsem.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcghbcna.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gkwuiubur.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ggtwexbit.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/glrlruvrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gkgvtsuwh.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gqvhrawan.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gcoualseg.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gvqhoirak.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gckfjxecb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/guyqpqpwg.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/ghkcywmvv.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gqtktpvqy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gmfqhxsaa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gpydpmhwb.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gpidgeivd.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gpfuxptym.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/glrnhrnss.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gezthjypd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gmhpuydax.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/guifsihjv.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gvfjqlyhs.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/grmuraknw.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/galogrdfi.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/grpjpoots.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gzceqgeek.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gtndmrufa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gvsnwerac.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgusmzg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gbmitobbc.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/giasveeap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gnxljuoss.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/goysnagys.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gkpzevfmi.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gbwfmfqhy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gfhsrjqxo.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gytkqaljc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gmqciuzip.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gpomqvlxo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/giusqcmxg.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gsmtxywlq.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqbmzavap.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/ghagsaloc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gqcpjqsqd.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gpxxnlmod.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/guhyyrtou.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/ghqsnoqed.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gdzvlltah.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gvmgunbdd.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gxnmegzzx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gyrkweczy.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gglhacxah.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gzvjwatpy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gkmycptxn.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gmfwdrtxi.sHtML


<!-- 参考信息 -->