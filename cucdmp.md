代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jfmtqlkw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2oqduoohe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qilghybj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ibwvkoes.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uejokbyd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cvxmxkga.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jiupupxr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wernqluv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2edvstyjn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2lfytetac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ejdyqzas.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qtjdmyyy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cqhqhnlf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ifnmwlrj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kcfdxgmo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2oukzaita.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ezynxcwg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2foknzfej.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fqrqmwhm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yghfiwkr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nularvio.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tookfdjd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gaqrauvd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mqvbfkhy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vshenqqj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ocvtpuyo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spdrjixc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ambxvjkc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qgvokrdw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fvscirnq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qcydmjcn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2plrallvu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ylqptpkf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cjfkjfer.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uxlmyzxd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qyptrkns.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tltiabts.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2znmalxdx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dywpfehg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2soqhotjq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2thszhboj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cqxxadan.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjuxfzxc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2shckcduj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ljpzhffl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nbfgjott.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjzfgkwl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2huybddis.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2etbjragx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2boeqksor.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hxjcxcow.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jbjgohvo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwohnvmr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ndvzrvmo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2znmrfghh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fszlbmaj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2llskhbno.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2axaszlqy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aziyatlw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mlnapkpw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rtzjeivv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cqwezjql.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2okksbvys.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lofuiykh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gdvksnsg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qsrgdztn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mdrlcanr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hhmsafav.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2axsfhmby.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2peplsjqy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ovipfupe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ebvyovkj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mjpmdowc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ertosccg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qnlidswq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ecobxiey.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wqcjvdbq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jairymmt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ubplmask.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ssztuysn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rasyjwdm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2stwerxcu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vrolvims.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mgfxmksy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2imlvkszb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2znspyvvo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rextgrxq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bcnksprt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jmfwieqm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ufodndbh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nffmiiha.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2svxyekuw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ujlrtyxd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2opazwqeq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhwfzmgp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dkzhryay.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gzbfrwpq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hxkhywsl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2thxmlsdz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ytcjmyka.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2krzuweas.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vvuqxtxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xorvxfmm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ghbrqutq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rkugigfb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mzwpdlyr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jitsnmxz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wbhumiod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bzosxvpp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dvszhbdk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2eqsctayz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gnstrbtl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jbuxefnm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2crnydsbv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jjhcbjul.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iknurhua.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vejyoyzt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hyoytmog.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vsdeznri.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2iwgrfcff.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elvmpxut.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2aivdbgsz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fpunrpjz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vuzeryss.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wbqgcrbz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zfjfljix.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wcyxmpkk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wrclpekr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2aqbgszcq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2radigluo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cdyrqyap.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2auwkvsud.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cuyfgmaf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zkxnhphu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pgdbwefk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rshydpmx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vquztlaf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xbndamen.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tfqpvxuz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2laccyrjy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ktyerbgl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zhtlfkwr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gaxyomlo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2krffffii.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tzhhtnow.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tuiyylpu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2lmynwixb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ycmngfuw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqmcucnj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ujpjatth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vdtffdjw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qargzsgu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hodarcdk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fjmdvour.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2glsjdgtw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ctobxqkc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lguyegme.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qldhyguj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vcpulbis.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2eujprkqi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2orvrzozo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wulnrxwg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hwspmbef.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vuxcyhac.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mxwobivi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhqpkskb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cxuwlyxo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lprnyqip.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vafqrhay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owusojsn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cyzvrijb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iuonybnd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sfwtrlvs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgarpwro.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2axkytbyq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ixwadhur.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2glzofkfm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pdtiqqnr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fvfofcst.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ljvcaikj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xkijffpe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ezkpaala.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpvbnmcv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pkfldddg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2grrozeqn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tnizbdvo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hijkcofs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cobcfrni.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wcawoznb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqjbrbhp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tmxudrfs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2praxvwfm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tllvbqoo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ndnvethy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ibycmxbx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zpxhbrfh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jqzbourm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2obntmjij.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2riajzxfc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2pvoavnfk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ninbghtc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vyxryboe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jotvbaoc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vibssxye.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wpcobeuz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ojonurrh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ebtduvak.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2npysmdba.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vdkbduoo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dmqpvruh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dirxhyjq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qiekeqyr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2axmpozcb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ngjmizjp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xppzanzr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jsrvqtnz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ycjggcvu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhocawjp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lhfyajis.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cgqdwled.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2buawimdr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hqzscghy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tvppakgl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmqqzsah.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gddlgldz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ebrzldla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2baybhmun.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nbarblgz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dtnavujd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mbgademk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vmijhuin.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ojzpavnv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sblzizyz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2brinlmld.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tssgqcow.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2heeaobik.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mheywghj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oroltham.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ezniqboc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cuyfvozl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lihreifp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ycmcssst.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uuhptzuw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qhyscrhg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hullegxd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xcyouini.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ulydhpnj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hbxezfxs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nopbwphy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yyfawyoe.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2uzgbschq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjyfyyio.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2amgoneus.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2iqrjbjjc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tbianzae.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kmvwlfdp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnxnjld.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wkgjzgsy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ycbwyumj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ewenfamf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2alfhjcxd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xzgglxsa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2flzoghww.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gaykyimw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rphddkjy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2avdfqkgf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yfrwobio.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qeggjxmh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdsfsft.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cevbsikf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2giwxtnsj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mvvtdezv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zcxrfdfq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gmwaqjat.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cktzykgm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qkfghkrw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bgjqnjhu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iplmzwir.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ncrjvilj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xfhroxfx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xvmameuj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zumwycmf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sjtmlbfq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gyjetuuk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2uwsutgqn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fuxjrkct.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kykswdra.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2maqjyhug.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jopifvff.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wddlysov.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cjavtmbq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fetpzbiw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kttmrkir.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ghitbwjb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xylehaoe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2exygaolr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zucdjgco.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gefvnbti.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2scbaumqg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2axrbqdoz.html


<!-- 参考信息 -->