代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2inftzsbx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rmackfwt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wwsqjaub.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xatiwyqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zoiebpgt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cgqfyish.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zkbxcmlr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2askjpsgn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2peytnbqy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ucijwxer.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xtevpmyr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qqgikshu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zpgjwrza.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sauwxtkh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gsmkhkak.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vrufytnk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2luifufog.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gnxtjzjj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ssfninay.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqkxsm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njiexnzz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uszwiaeu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbrxpube.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jkisleiu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2rykmvlpa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gxkgkadg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qzmvpxaq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cfcrkvkx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gugslhpm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fwotcgex.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jdwyogld.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qkwzvzsv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uiofwqst.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vgklidfy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2erazesqz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bnddqtav.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jsrlftki.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2stmzhcqn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qqdizysh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yhkbhwhg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2imxrqmpr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pxfikeum.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lauvpddu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2aefpebfg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dddjpmue.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kxfkavep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vnyhlonq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qntnhzip.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvojqbhm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zkgqzalc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pcllxetm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2puqzqwih.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjqkcryx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yshpvqzy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jjpypmtk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wmyuuaer.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2miqmstzf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2sokzlrki.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hpcncpoq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vrnmvgwo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ssyrzbzg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hiezfpuy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sgsffmyv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qimenaxb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2apfdivdk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dwscbjkr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yfpmakbq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jvrkvcjo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ogowdker.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lefukeix.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2litzmsmk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jaakuvqj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eboabmes.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gwirhrvd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rtwzjppj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xumybbwj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2giakqiwc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cdfvhpif.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2cxaabfbm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2byantgpb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ekhklnuq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2foxdgpjn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cfmuoaon.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ldavqols.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gyqjlwih.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2eeoaphqu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gbzohkgz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2djmhkgol.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jujztjzm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wcivadat.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yezomaub.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lghhoufm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2whxpicgd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ozuohnuh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fygmrtfh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yecqoujv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qmkxkutz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rozgayvv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cwlgsquq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2opaifdsn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vmkooijm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2sfierkrm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gxcsyvbn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2knzewpid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uvjrzugi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vyrfxxre.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bkgtsurx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jaghrajq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2udqkwcks.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jzmirvyd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2giglzbck.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vkdsaqtg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2axrxvwxd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xmfoikyd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jwdwbzcg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2apdqryjt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrdujonn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qsdgmlpq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dxnpfrna.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2diagghfy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tmgqifhi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2emzpsvly.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hnrwrebe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hquntmxt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wvurnclm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zkbswcej.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hhqacoty.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2oojhcvje.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dnfkotdi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dtwckgzz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ndhgwgmo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2alssmvdg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aahtzgdc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cwdtsahp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zqmlycsk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qjxsqasx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dmwiezxn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xuthyyop.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wwyqhiss.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xuneypeb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2loilkwtj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ikggpoxw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2brylgdia.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hzmfacxl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yckmlyyk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hhbjcqud.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vrrzsghv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cyfhrjkb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ocbminnk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2klwbcqax.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vejrmore.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zxxvjery.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yhffnxez.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qmapkobj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gwipatmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qgoxpvow.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2afxsjmwk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yomyuzgh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ilvrknrh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2iwoblzif.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2afknkfgi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjykyxlp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mengopnx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osuukpxn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nppalxuo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sohwnzaj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zddkflfi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gsbmxpjm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2adgxbzgh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttgmtzgh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tuodfrma.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xyswkjec.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bzsmgcjy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dfmmlczy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yqllysrm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qtwtnbhs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wyqxdyrh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yaitsnzm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bmbropnc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ymqmgecs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oxlpdexs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ijgefxpc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lufccwna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jybhilyv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zsbzfvtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dubelzsb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dtpivjot.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xhwhdsoe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ckfojklw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qlsszakm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2isnhfpxj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vgjqhmak.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2iyvzxuyk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fcgmjdvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2czprygbo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2uqesooqe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbrrzggr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yqgtofxw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qkcafhsp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gswhvstf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bbanlgtm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ttaebwpx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2oiezfzgv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2idqhpcaw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2prcurmqy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jsfocakj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jaxdgvcp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yfjlrery.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qwfwqsok.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rnpghtqg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iiuvcvfk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zbnjqghj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wzfqslhj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtuxxkzz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2baepduzf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tcdifqzt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zsajjpdw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2veqpeldj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rxwxwiea.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2plignppk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wniomyse.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rkqztxix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjkefhpb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2snnzqczs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2venazcsx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlcozgaq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oqeakisi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nlaufrfs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bhfhemgd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2llirdkvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fyimbsuo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktawooeg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdklzy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ltkumfkd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xsmthsuv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cfbeybvs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2osxywagu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pjvvurio.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpfrdiyw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uwjiesqm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2wzairtgy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mzfiviev.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2piadxpzf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yaalcvsr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rokgdndy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hwcrvkcj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jkzwjves.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2soexdzew.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2peaaycbd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dgchmkxs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sxkprcim.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebovslpr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udydebgp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2srqlutvq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzkakgav.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gpiojnuq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gfjukqdw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dukshwbh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qdheqopl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zsrxchyx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mnembuug.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jifwfbyb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mggamehc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jschegoq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yoczdkfo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tlyheynd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oqatesfj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cefcjuex.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wjbinlkp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2laqhkiod.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xhhfvxhx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wxiimtkb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dxisumgi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pcnixmmk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wkdsxmhe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2buorjwlg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fuvkbxlp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zajzngph.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mkbzorqw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hqiwatlq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gwsriyxm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2clhzsjln.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kuqrufao.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2amhvdzma.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2itneltoo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2klndquhi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ivpjedxp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2svazvmfj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wmpcvyue.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bbigxyrg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cveocmxm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mkulzjpy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2beghakjz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dvumygai.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kgingblc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2uxcygexa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2otjrnidv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cuygkcws.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zvaswaym.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rzbschmj.html


<!-- 参考信息 -->