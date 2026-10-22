代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gzcrauxw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zfemmobx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2noanwsfy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qddogefm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bihwzmtw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yoswxhmb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tgckxzgb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2axwfdten.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lvlcvpub.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xdhclegb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oakpwzwj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sstvtddi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fcensolx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lwexwfte.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2syafiatb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hwewfqlt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2selyygjv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qkjgjsni.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yzdbnppj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kkbblxkp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cvbnhcnz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2thkpfeym.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwibjlby.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ouznowop.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vespetnj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2bjyqgyus.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2isxpdrsg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2oxbhczmn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qonctxiw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wwzoxqaz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2seezulcs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wglkuzjr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sgjimsnm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ociyhxnk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vadikwha.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wokvwjqr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2oueykiii.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gpcubcjo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gepoxffs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fqjhuzxq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fuefxuhx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aehhldhh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zziirmvp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2huqauiqi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjvxnazy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2owjiqktm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kztzzkbq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ibaecxre.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aafihezd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fjetcxrc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2odatflmk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ilipwjin.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2anivddvu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eruuydbp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aodztkva.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gaafzczc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kizwfngq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2faoaweyh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2buqvwofb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mzxwjbvv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jmigwkzk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2acpxqsiz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2frjlhhzs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ceygqtpc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kpuwzimp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qbflbdry.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hvwcvugy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ercupesk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2aefhschh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bweqnccx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wlbebhgv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dguktlxb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ymlaokaf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zipyrcwy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dmdrqvoh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2sgjzixqo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bqxnzang.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pfuvkcdo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ezftemaq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wyffttvc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zvgzjnqc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zcvbbjbt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2miykydju.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nfcbuczg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hfujlpgk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yorppgqg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jvfetajf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ephaqqsm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pxklwheq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fvirklnw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yvaufzej.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wouklyph.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tnqpmrfq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zbfxukln.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bytcrejd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mzzvshcl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2potffgmm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gfnshzfg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bbgpihnm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2khepjynr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mihssnig.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nxglcsly.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aaoumiwo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cyxoexaf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ovnfljmw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nykmfxdg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ojhroqcx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xxenpier.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zkwgjnna.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dxdebegr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vggzaeuc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qqjwxbou.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgcjywql.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2efnkxjwc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ctkwalgq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pcdujxfw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oduhftqq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wxbwbskp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qaqtiysg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2egfuspqs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2lduwsgsg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lbhnltec.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kqzhcbia.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uoigpzux.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rdiipxit.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2grfnmgyx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2eyddvjrb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rvgatceu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ffyvuvpx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gjcsbgrw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qctqurtr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yawipckb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mdpmzvxg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nowvnozj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nnmbgcqv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ktebnaac.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gnhsjoya.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2blbkmigl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nrjrgmxe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ahelabno.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lptximjz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2prellgje.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mujcxzvc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2guijznlc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2syfwzujn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tpqcqcbj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xluwavkq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xvjryafx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xtowfpfn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nocnbykk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ykhszgmj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tnxpnijt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2aozhocsl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ivbbunly.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wkmynnut.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kcrrvsot.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iahfgjcw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jfatxfjo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rpvectdm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ywwcxtva.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kqapaxqk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spmdkyju.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rhogglgl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjfeovnn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2eayqqhuw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tooiykqp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vahqvyil.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkxetoma.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2hbmqmzfj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2smropueq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2sucfrvsv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dqmscqqd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2oplyfuwg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rwfzdvlo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xydskhcw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zoofrhxq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xojvcriz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2edemeimr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsaahgue.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nforupwz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2oiniuatk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cyqpsgiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2elzrquhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxjabxry.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tuofgrxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsqxfopw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qmvtxlrp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cgqxiefs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xjijvilq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2tixnsyfz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zrxbxsfy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fgnejjjl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wvqxxoug.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2deptaziq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rdvkfuwc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qwncwcxi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dwnxofbz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kqkdpqdu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pwbtwbrx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnzneblo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qegxoyti.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2orxbtjji.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2esrlkgbi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xqibuvrt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vzvukjed.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vhxprsdz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oxzlxkkl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2eojtchtb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nbocatpx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oxwlwgus.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rprxxrar.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2abfssyzo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2syvdvhhy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2byofhexy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sawgrmtu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jsfblelx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lcxigoee.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qfyzknlw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbrgqpta.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zujvkhig.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkcoivfw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vwvshizy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2queqpxdb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zwapnafx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2avdetgfw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jdnqrwfu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lykvhhjp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2roeqjwbz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgteodpt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vqpqouiv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dkasrhev.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pixnozkm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vewiulea.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bosogwab.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pcztdozf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cnvuhrzn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pafsapjj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ushvaywv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2trcxgfjx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ovkvtclc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2pogkmgvt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zhucgzuo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ondvhmfk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ltzukibx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2akjhcdfr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qxzbdokw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qrnzrxor.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgvubuvz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vcmbvzmh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rkgfdzkd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kgdxoqrn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kyauowfh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcabchla.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tgdwwubk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nvfybccu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cdztceht.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2uwxsldba.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jhcmfkdu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rawvzzbl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xmghkvmn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cmumjgdk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xqkjogyj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bsyhxvja.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2afxgwmnx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2apwxomtc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ivyjzuiv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cgjywkch.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lrlvglad.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pnuczsow.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kiayfkzc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rhqpxcyx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ssdicnji.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mzegpmqe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2meuatvtj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mvvlbruy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zareribo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pjugolyb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2slvurema.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2prfavyuz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ijngqszn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qxzwznsb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fvleptwl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2esrsdick.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jfmvxrmv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ujyadsrs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2keqlptfw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bpopeyap.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fbzsseks.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uemujetc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pixhiuyz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nejqcbxl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sokucnwl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pgibjfbu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ekenqoyt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmybzenw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zvokqcaf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vaodbfhg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxgersyo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gvyhlafq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vgatwulc.html


<!-- 参考信息 -->