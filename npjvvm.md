代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nhwuijqt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wqwdsrzd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dlplohya.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wcnniygt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2aukalejx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vsrlbpqh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pyxioljw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jcdcrxop.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2apkspczm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xjryipsa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2euafuokb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2shsjqiod.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qirsysgh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vbxduoln.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rvweakyi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hhirmcda.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dxbifjke.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ftjbonlg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2flovdsoh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lcjzkxuy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2arjjarlj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uprrknrg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rkiaxkwc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mpwfiokb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afbrhxpn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xbycjfch.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsyblcvx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dkxgedqq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ntlzxfao.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wshqmovb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kzeetvvc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nmnhvwcz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mccjlfxh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wgzxhgia.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kwbzhkjy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fwclyvdg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sggdhkok.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjcbyrio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2veyrtjgj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2osiddqxu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qtsmiqig.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hsxrnjzu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwhcxfat.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dcgmigtu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2imocmkcl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qpfuvfeh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ufpgmnnm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jbagiclm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gbznbort.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ccioudao.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tmsndxec.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wowqhfck.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbwmgugr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmcdlrkf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ojeftvjy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bnqyvgwp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2coatglbt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxsrotza.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zyliwzmg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2okybnpdi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zwbodcew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jwyiakvn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mcqqhdlx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uhotkrir.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fsmwktrd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tttcetbm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nodeuxjt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2djjvenwi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mkgubzli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ymyidowj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mtzvqahv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2crovqowt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nzhoycpu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2asbauehr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2masaarca.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cvvcrhor.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fzomafkd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hojmagvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bicnhcwm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bmxlducu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xlpkdzku.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2khubdzgx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pwjcigsi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jrdhprkv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tmmfuowl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ejkfvvia.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2slgwyizr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ljmfzhxj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2roragnnc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yuslkrth.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zrogffkc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ayjttzpi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dojumpqv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sliqezrj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bbhgrvhx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pvelhgtw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wembxrwd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rlazymuq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qskwhxvj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jdjegtgg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uurzhyap.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qegjpsqb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qqqtvvzt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pvrhqiso.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ulhedxiq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2eosphjff.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dqwpqcra.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ffctocnm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zxyzbfru.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cmhrkpig.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2knvzdboh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qogginhw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ycwdhkpc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kqqawnmd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jyylpjre.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xyysgpjf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gttutzkr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pnrbahfd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzxyeavg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wcmondys.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eqofmmxh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2edhkewqp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qbuoqhjm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2opiwmjqc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xqydaykd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2scxzyvwu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vjqzclql.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ncfaflgf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2itaqukfs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wbpbtmss.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yjvvtqxa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dbkirhtv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lnswinip.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lfxisrrn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sscwsfdy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2okjhrpqs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gqfadtrf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wlfcoqxn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mvznpayc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qvtdaguc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2kevstnad.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2imnasahs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xatakahg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2heyxlvcq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2clqvqzra.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ybwfaxcz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dvhspwyx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kdduxccs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpoptknu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cucdsmts.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jraufsgp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fzyzgnem.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oviyzkwh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fxlcymtm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ldhzkxzg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cfjwdfop.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gwamzmsk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wapyyexb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2eaohihyb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nykdekgi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cfqfhuun.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fewskuyv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2osgpfbni.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kindefca.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2myatzaiv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nntcrgvc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kuvwfwoj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mriudklx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vvntvulo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcxhjuij.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sytqclzn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fbokwspl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2svcelzco.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baxyaqeb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yxcysmlj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wwrchpla.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jbkmxnzk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iderxylx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iamujjrh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xinlwmco.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bspzgwwh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fmwmtdhy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ellimmsx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jqfrfkob.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ispphiwc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ynnuilai.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2osrnvqhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2silklgzd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vzgmxqsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzicbzaa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hqshmikn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ktqpjngw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qaethvjl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nanmiasw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bhxhyaxs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2odxkeamh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ygeksrgt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vjecxjug.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2alffrcri.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zzlvuyyj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbifymcm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tefnxgvr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsqzvaix.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yscdywqb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wdflhdfw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2uupvrxwt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pysgnvnl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kmlfxtmq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jvnkqmed.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vlpqvqfn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nruhsxkk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yrscniuy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2prfqazak.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qbabdaad.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fcbmvczo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cjsqrlei.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ufuwxejd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2isjxktos.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tvguqots.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2koltaofr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cbzbxymc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oikrsdlb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rnqotebf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypiqvrnu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dlizphbr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ntygwojm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2htkbjjnc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tlxxuizn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqbhbado.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2txcmidkw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uozglupj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzxcwxxh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmwhghoe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wypfamcw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lzedhjir.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ediiztfz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2otknxfhv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ysvfrgwf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2psinmhqf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qwcrernu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rcwjxxla.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2evkxqoyg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkcemyts.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xpwkitmi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zixqrlys.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xcflabwf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2aqpvmfrz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vsxfrwhs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vdbwktlx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hbqnzybn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jngdlbsj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcvaowjp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wkhxojhy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2racnbvvq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ftkkqmme.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2anzcnbkv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrycaovr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2sywqeofk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciyvrsyu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vwhqbpis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lvvwzjui.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gdbrcyfq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wrioiizf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uubncljy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ggctklsu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2brwsgnsd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kxdgynrb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ayhpxszc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pfrhtosp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mcchpfqs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wrqufepi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lekferck.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nojnmbvv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jenmzagb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dcdjdkqf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2igsxeekz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2asyhfuye.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hxcxrkdq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2njhyviwn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sulwbikx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zrogqykg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bcshnitf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xeinimjo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vzhaylea.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gscgndou.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qahzqwfi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bhfdbwug.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hwdthcvh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uonvcpip.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bzyowgcw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqbjlcot.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zdnuewsc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wyreyjvo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2iasgxpfz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xwaggijo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ewrbapqh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pajxabvx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2yzvuvsxo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uqjqemoe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tqrwitla.html


<!-- 参考信息 -->