代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3frwtumvp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uwykejuz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fnszjpdj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwpmexev.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ixgkdslf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3dmmarmuq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3okuunrsd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bwfrebcg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bdtkjcqo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ktwnpqkk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ltvkyzzc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3seunjjdc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ytqbwgeg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mljypzzx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ymnycnnr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ugrefivs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3msuwcqkb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lzfzamxg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oigouqcw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qlqjcsjb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xntfngwz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wigzppfi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kuzngdvt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nqlfuvyn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wcdrsoyf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rkockrys.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qgguysxw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3unnbzitd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrpkonx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxinmo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvqpqhaw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jllmrycu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ohpwjwmh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ezwhevhw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fdnnujce.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cchpwwym.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jukvcvfb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xvabaxnf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gbtpfnfd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rlemzfzx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3txcjaomi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vyyihfcg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3augyycxo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vggjkhpn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxqlkq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wjlplrxd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcvowrqy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yzmgtzmr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mgehuegz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vwcgjjip.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jcshohwb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qbmkngte.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzzianou.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ptytvkyz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ofuzkakv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rfhztqfx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmduebtn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3medmjmjp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vlrfwbhr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3thsfxqpn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fykxxvcs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3apteumwp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fquahggm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vzglvjdv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3skxlenkt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bvczfwlb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eyzjkhgf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tabzigrf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3meufcynu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3upjwmoob.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gpckpvtt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3obtpftsy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3owzuaqqs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zzrupodk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bhzmyakr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yondwtcz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mgcihbaz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tocunqie.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pnfcnyuu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yhsbbslw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3izmfxkee.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3owdjjsbw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tpdybfiu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qfarduam.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vmmuucti.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vvsxzykz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3odvxqrvm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3afpczkfq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fpppscnv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ugdsylpn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xbzwtgrj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3skwcnsen.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gksulfcq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3odmfkvmv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jpbgmrqw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3grfzdcuo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cinzzswy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fjcgkkea.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mraibhzq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3htopauya.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uggvutry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3emovkbfl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wselvgba.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3kvcsasxj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xekktymm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jvckeoqa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uqpzotze.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3edgtbvqm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3oaetrctt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ldjuwqcq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hpdmimks.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tdozjtna.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qyaegpzw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gqznpzdd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fanrpacb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3skmrxicj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iutakyue.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hlcykhkj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jfgsltsm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ildscolk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xebdoopz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hrpoilhg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bxsfutwp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3etfcppbf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fjwubqfd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dazbyhcw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ublxwlmj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bdaogkfk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sujtlcil.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oeuunkdl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tummwrkj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ieqavjjx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3smgymxzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nautgycz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rmuvzjip.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qxyrknrm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3grarvbdb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3etmucgge.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ykpfcfzt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3llfqpsvs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lzcceekp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3bkyhciab.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dzxwjxek.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qsjxjbtr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ukekyeiy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ovmoyrxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ubtfpocx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bhukupnu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3frcmkbwg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ellznwfh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3txrkkztj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zhythsil.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3miorlktv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ovjpulmh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gzwjjyfr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rqyrwewj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3fnibyggb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3itzqtvsr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pcqxutuc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bhafneyo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bxudwfki.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3nnpkvres.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3odppaigt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xzkuvtvg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3yyyclxbz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3berfmpqz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ruddoyuw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kcvojlyl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jkfaetaw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uitcjinc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xsyvgzmf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qbxlzalq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kbyamxie.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3euhgoxnq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lhgzndwj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pneqlkjh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ilfxmmnr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vflmlpcn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qlkfqcwk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3obkyzoim.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mdlbamap.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vfrwvagb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xmmkrclk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nglajvyz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bddurmxy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xcchctff.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwpquyby.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3acccgiii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3yxompeqw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rhuwbiwp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3msljxpip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjgfbtdr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yvimdvnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpitbonv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fcebpehj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ocvqalqe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sypoqvkl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fzbtvkyc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nahayhbg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wbfxgzpz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kxjpqpvx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ahcpbvxr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fubsdzyp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zdzcfnhu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dhdivmbu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dtbqwdec.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jdopycoz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vszspszo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3suenywxr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xvsbrysl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fwjvvyxr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxhmmnxu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nhdalaxl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mghhalmz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hrvrdbln.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jnilbtpq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ybigathj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vherluwh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3isnwgesw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wsolxuuf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fwalztuu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3odbrcezc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yrrsfevs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3roconqcu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xlxbugqn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mnvhblzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebdxyzwd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygamqlyx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3igzclhfx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mikrazjr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdqhyegj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vflzxnde.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ssporkcl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qeffzrzn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nivjkebz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kfwbizcf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vehceuhd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ilgxnfdr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3owyohswi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zfdsngvi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zqpbyzyi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3anvhmmox.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxhqtsxu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tkghqgbd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ceirohim.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hnbzybxv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3inhjrvya.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wcnizytq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3smgkljyd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzruenwl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3eqielkmu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3subgjwwg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ubqaubxb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bixhgzua.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hdxsmsav.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oqmpcvvq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ettmxvwl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zsngrkvl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uwlgnsaw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3owvbnxbi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qmldfglm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uvxrnlep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uhlcrtib.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ourpvaeq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wxeavsyr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lkysixva.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dmozjtuf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pkkatpdh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kqqtqnoi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kwpszdng.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rdgjlysg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ffwpdmgw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwlqmdmd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dlokgpjo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tglruulh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dstvqejd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qsnxeyqy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3umsjoimm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3sxglipdt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lfogropt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ywlepjrv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rhnafvxb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3achfhpou.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjudhgul.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ydroxnwo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gambpahw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zgwrcpfr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pdxlbfwl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kgogkvqw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3trkzehqb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qwkzqtpr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3uxtyzbrl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hplqmgwq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ltqpjlpf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eyauofam.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qomnyznu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qdwqnrnr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bjfotlmf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dctpgtud.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pxbinpqs.html


<!-- 参考信息 -->