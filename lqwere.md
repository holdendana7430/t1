代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fevtkdyc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lbanykhv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2liznwmfo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ddsdorvl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ixmbcxpc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kfyqmdzh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bqfvlaut.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bqvsuagk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zhwmcdgb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mdbztpot.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ttypileq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kqqexhwz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oxscrnya.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2staijkjo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pkbrweco.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zmcibrgh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dotbhbke.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2godqiiml.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2yypdbxvf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2djijqhhz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bbrgkpmq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pfdhfyho.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wpreuuli.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rfxvnrfx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdeoufko.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ivjawjpd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wixiynrt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hhrkwydb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2unzcsanw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gmwemady.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dcorinxt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mrgspxde.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xceltjtw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sltjcoxc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kbiicblg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2omurawok.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dikqsqgz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2icjevrug.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mstbaogh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mkzhjfpl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xlgfkzbb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dwtldzky.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqqbepjr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2frwymqnd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xbzccrpx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2nxxssucv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2smrvyauy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qahbhymo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efouootq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dtrnxbpt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gnvbicvh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2spzkaltt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxdnuiuk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jnvcrbxc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wjaqwaxt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fafqykzl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2txydeqxh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bigjfcla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lfjiooob.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xffbtdwm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qxtszute.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rsfeihcx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2misxfrpt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jftslqlq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bfbvkrkt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lbfrxpji.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pgzatxrl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yryrvoby.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2edgcwzif.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wgizejrp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2psqbnrjg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wreafjtb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2urnegpcv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fsubhqxy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2entteazv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hzziktlr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ytnqbiqg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gzoqmwmc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ybbkqfve.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tyrlrhvb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bydteusj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2maedcvzk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rzddmbee.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vcavwqmv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2huelvbfd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mefpkebc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vtxfknqq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lizvslvg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2umunxvlz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hetpdylw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kyblpwlt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gvrufeyi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2luytyqao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nspgcsyv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gunexqjf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2gavhyook.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kxucxvni.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qulmiegg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fqywnucp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pqksflnc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xevhwvsc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qxjhoehe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2czgizned.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bvljmsww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mwiasbsb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xnnffuig.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xtqrvpkt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zrawhvbw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ehhiqpaj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kqkutano.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jagagcnw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fprtemhq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oztzsanh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mbdxjyxd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lwnqlxrv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uqldbeye.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shchnclk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ovoxjtpr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ntxpaaqa.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2zdvosqis.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hesrmdou.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2yrxtrjlb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jfimgexe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kjzmqayy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kkezveob.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vyklrblg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qeybqqmx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2easlxwxj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sqdgyjcz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zcwddhzv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nzylrhlh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2qveeuemr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wzkiwbnq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ykqltygm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2erqaxwpc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mvuunsxr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2quatkzjy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tvxkwuvv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ftulrbwz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ienpnuwa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xajlnmmn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mqrkoeuu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yaipoonc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2korrehpb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2flmsiaju.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ohzjumyn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mydjocyi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uuxnwfci.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvqaeqtc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2revfsjof.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hunkvxpo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tpdvcbeg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2unuyoufi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mvajvqel.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2epzjicud.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2smwnffum.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qvjmquyp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2siumsfyw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jvecwefz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qpbrcsvj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qajzneqt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2urefkyzr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2natpcbfv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sycxayjk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wuijcovl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcziqmdl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uvjifzgv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyofjagx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2zvszjrjb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgrdxfue.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2espqsuvh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aazbicjb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mfpvnwpm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pegohdzi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ivcqboev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dfxhwmiv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tdzhaanz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xbkcfeok.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kmujybeh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bopryhbg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ysostyfc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gtmgkoqy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dpxkkirc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2twmjanld.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sonjhbjg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wlpnqtlp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2eyzctjnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptqzwusl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kdvckrwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywsgcefi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ntoeuepn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mghvywdn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2galixxwn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2golwluni.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2funulese.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qgohlxew.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tdoiokym.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2auqxnowx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gypjuigj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fgpqtpwy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2evinsept.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nptcnahz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nvklvimg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xxzruccp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kptllenm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mvvefgaq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bmzllnyo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2myyaptbg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wsbvwkjb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uqrimrua.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2irnrhymj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hzknmnqs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vrcrpjwa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ijfikkys.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eperixfj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hwzjuomr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zzydylce.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xdlerpuy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2inyqnjpe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lknztmvf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pgvmxcrf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2txpnardg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hwnldfrj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2azkuzgki.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rraxayjj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gkhfddqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikwscurc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hzrdhmes.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zesqjynd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2otmazwqe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdatqpsp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qtlwslqs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qsvrtvsj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ksbgrpiy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rjeolske.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nmrawsdk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ypkwerdk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gtkmhaag.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2trelvhft.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2krpmqocq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2surnezie.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nfrzxunc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qeftpihv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2moeqddco.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kajnbxqe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rncxnovm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2joyvyitm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xspooksc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2evckbwot.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2njmmhpta.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zbwrgrsr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rrnmpoff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bxnscmzp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jnuhrbry.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tharxtle.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2avrzpter.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcovefgd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2glrsficq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhkchrcg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jrfvkapa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kylarfoj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lbuantmt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2laawubdb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2haucnqux.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zdlsxurs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nkhmjuxp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2atfjgdoh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jpblarhd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ertkecul.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gqvvlwkd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2aosqnfwd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lcjtaajo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pfnligqx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2irgbpmae.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qghjxppz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jmkfsvpm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nkaqnzta.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xkwvdyud.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rubczxwa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mawaphyy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qpeqlrss.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2civugnyr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kmacnkre.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ptlecraa.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jslvpgks.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ulpfxzke.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2znozlvip.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fqllifop.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ksslwfjv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zzcisycv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2worbdpee.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jzadpqat.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2clbczckr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2owqmgxxn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2huxtqnkf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2eribdiol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fsmhkvzc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vglsfkni.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2afqpbnxz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bsdwkkhr.html


<!-- 参考信息 -->