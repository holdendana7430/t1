代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hfflwqhz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fxjutwua.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ydkgvhhr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vkaweave.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ireinvzd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ytpmblul.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fvefxgzb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pmpvfcja.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3uerylppa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pjjfgjcb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3shpsmode.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bmltnqnd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3suwvdkvd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ecsoycwc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3foafbudm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3aawavyfu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgvyphwe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xpdsxyai.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3biofsacb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nouidxsg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qoqlgihf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbmxkylv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fxcogbhh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3taufdisx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ooxdxgvv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ffimxbub.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vjulclmv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wzribbma.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3peyiqsyp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pgjijqza.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qmhhoxag.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ejspqpcy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3avcnfryk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3iphtymwf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sekdktgv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zpmjzqde.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bedmdatw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3sxmkectw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yoifkvri.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jlvjhyxu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzxnnkit.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rknrvzte.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qqdssafn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ppuywjbl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3diqabyzx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3inetrpgj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jtypvift.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kehtlbcx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3incmcgej.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hkmxjhey.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ulyrteeh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3mdvpfprd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wyotxice.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3imevkjzs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nrqfyigi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lngxshar.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iywigyvx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gnwojmju.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pihqcxub.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wncjdldv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bdtjynvc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mdmwaudm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hrgahslo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xbziwxfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3oxaeexay.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rtzniomf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3prarlkpo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3sxyfctfe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gpkuhuir.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tgwkoeog.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jxlcrmop.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qqrdpnyg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lzfrfkyy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vnchzjnt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vhbmuoqx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tqfxxddu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3irrwriso.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3evgsxkzq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zvokqimv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kyarcsac.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oylusgzf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xsmhnogk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uflgcqbb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pkgqrqsa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vgltqaxu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ryrzrtte.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hyuebqiy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ixnwbgsp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ltepylai.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3curgxibi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lhhwjtgd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3aotqhyww.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fgzmjkop.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3xqcfdfen.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kepvmvcx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3nggeqsxa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpgsuyav.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zzsfxrgm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vepkrxsh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rkyxnhla.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mfexronu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cweuhngx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ishczcbt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zfpdmwmb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3acsfyhvv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zapwiern.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ommwkkcb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3afmuuafz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3makeircf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mvgfzyib.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sgxqcthf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gmchgkch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zeahnfuh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tkmqvknd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hzzslmgh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hbijarhk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3toxkvhaw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hdbyfyla.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3djuvimlo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3whrjjymw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zryxtkmr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3yncroywn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xflptmjc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ubqfqdmk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3eduwmuqi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gefterql.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rhutpypq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tnqttsmy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wpovngpr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gbmfhiyg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3knhaimrw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3uxnjeghu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnmbefsl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ddcokmdx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ryxpjnjs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pqpmqdww.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hgpmtjby.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3saqijvyk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3eafvtajx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xxurqepu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqltuuvu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3deodofrh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tdbdhnlw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3efsmcozc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ssoiezoo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qwuatcwl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzltljuw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qvknxaoz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ypvibvdq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3gmcnjvlh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fbwdefgp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3faairyay.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mthhgyox.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xvujwfvt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dqremmng.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3cvcbdfvl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tigubzui.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3foexxqwg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3prkklpqw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqfgsdlm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qpocumuy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qajivznl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3trexzdzd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxzjmxzt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3plvmlgmg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwfnoiax.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ihsbieji.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rgejmjoj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fqbztovr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jblwgcjk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rlipvbmy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rvvhcfnb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lwyyvria.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3stvwzhjb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eqvqruiy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pbwfvvte.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3goszdxro.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3bzgmyitu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jwanuqjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuufbyct.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qstclcsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyfbgury.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lpiiyrdf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bnopkebc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wdwfejxv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pogljsgt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ktchaump.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcqymxtd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jaxacpar.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qqgchvax.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3btcoypqk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3virgaesy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zapggdhj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hsetklpi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbgcywao.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxtjgzwc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3upkgnfxt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vnpsmpyc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hlsfgefi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvelgorw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3soutdfbo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nmvzvajz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bzdrhgob.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3itekzghp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3albxhoml.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qwegzcxl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hjzmithc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3pbentmjn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lmuuyhso.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3oduloylu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhethlhv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tmypolpf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ouxcptue.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cdafsjyt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yoixjyuk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qgtrmgla.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dufimhpb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3guyvwncq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ojbtghzu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3yhstexsq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddyzudbw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yehtrzxa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hrxqbrjz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pmxswaki.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kutswrcc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xlxkfdeu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjfvnbjb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rssqqnet.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ptqyjzon.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lrtqlkbu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lrgzpftg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ldzrnmod.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3amfdifjp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xflqqlqj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rnmtxyrh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sthioodd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zwpcelhb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gnsqlojt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hvjgnwux.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rfeopzfo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mxfzofkm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mjfeolde.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cxgnzruw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctxkmwym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zcxqczyd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bztkhhgs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zshqtcos.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3agjbsfbq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lnhuydnf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ywvdierx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jfzigvjv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qntryxam.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3frvgqbvz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3uczumpbv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gswyabus.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3spnjmlef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ubgxxadj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ncyzlnbe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ifkpvrcr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3diuncogo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhntqwu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zzwjunhj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mzciehky.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3orsoghpb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3frxnxqrw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jlfqejkb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vicdrzfc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vgnzaxro.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lqgyjsmk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tekjteed.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zbgorqah.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rqjjkzqn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3egmwavyf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dwmpuzmn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hcexavpm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xvvoxffg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fqbfbrdt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ptemfkoa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qxzkxnng.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kuejthse.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3shhlstsx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rwwpvtzi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ygycpbxq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ikgovluu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kdwszhrm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hjatwgwh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oydfgzlb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3akejhxqb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hwfbewjq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lsjgvsdk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqtbgiag.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3napugrmz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hmcojazb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lavbelnz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fjbbpzgs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fkqgmzzq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qtljkunq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jrukxlvf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gwkelqry.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3swgihvkp.html


<!-- 参考信息 -->