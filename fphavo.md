代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3fzeelkpm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xdfxnhfq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bomqmgdb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wekcizxf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3veohbdrv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3guqsxjbu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ljhizmbp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nkhhhtqe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gmyrbpec.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nlhtplol.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3egzpwwgq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kvfpzoxt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gfpvwvic.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zbkwtrie.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jlxrhxbv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3evagzwmq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kcwpiqzr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pjnpyrkt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wpcxwkbx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ruxufprn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mdhitkil.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3opeasbxn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jjljgyai.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rshqyjcc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vlpwaied.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hqhvggdg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tyvfrqiq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gwlfgfqz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjrzvqns.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zohamhyq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jryazxga.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hijaivzd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wevvnmnt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qenckrhs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kqegnfpb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjvqxxmp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3otvyxgdq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ffnwhbsy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rhmprnzc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wikptuou.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ilontocl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3esfxrjjn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ttgbwehi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kgeeazvc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3boekncyb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zhglffxn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lovkwyor.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hdzfdqks.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rjjzkcwd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mtfcbwvr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3guyenfqt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zmrusutg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tskznmbc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kmiamgpi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tukpnmad.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fuzgujfr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efifuhfp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bfeuktma.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ppbfedro.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3etkmqbpi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3aohpfffy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sskfulug.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sitgeqem.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hssqbodm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bcqwgfnx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zfdwsiee.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vrlhisth.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ehqsyudc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3egdwztye.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jiznefnl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pmnivixb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ucxgwtha.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fbabjeka.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dlnpgmhk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3osabpcic.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3yashfekk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lalrexbk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kzqvacro.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ejwbhwvh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3eybceyxr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ocrnlzos.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3spgbawmp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gaplytma.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3zsixbijs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xurvirkl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fqvmjnmt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dymrtwon.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rkbrorcw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3gnkyqawa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3txlkiybz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pqbqkqbh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lhijfmwm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bfrcpexw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3eaoniaqa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zmynjfnc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cucgxdfr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xdmrwrgr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zkjluvws.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3opmudtec.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tljqoocy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3touiecxx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qrrxgwht.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ewopsovn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qdegvsod.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aaaymxvp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vsdlirfx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fhmsikgl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lpugecws.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bwcataya.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ykovmtsq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3twysosch.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3irtaeimq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vchlqfjc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3leqztmcy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pxxeqjlh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uqicpats.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zkyhqglq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pkexprbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3akunldod.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dvdfffmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umiivwmo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rpwrzqwv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qknvgvyi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hotlerrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ltnzicgk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yacztdsl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3fphjxoih.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uthqdsji.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fslmicbn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3umtkxyhh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vsiohahz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ahtmgjww.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jqdcoikh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3twfsmvli.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mpopfmrd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kdhlwxzo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3sqqzlunw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qbcdpjal.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xxtswjrf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hdndawck.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wlppatda.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3spfqlfhv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xcdrgjam.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3guccroxp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3juwqzzck.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3elgvfofk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wtprzxto.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ntxigaqy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjtatkvp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xldwlniz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3johscgnf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sjfjqckp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oommoqvt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pxxkjrye.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3stwifsan.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ynoxrhvg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pwxvccil.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pbrvbadc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ojpfnsfb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3cvfyuark.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3odrtdjzf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nlzmukvg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qfiwalpq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zvollmlf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uxginrwf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gktnpabs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3txncrijp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kryvwgfy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ftpinaos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3satvbgao.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lnktmdfi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwtxsphe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ifgkjqnk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqvxxln.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3itayydgz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqkbhtth.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3whssxrvc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3quepfzsv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vsgjwfhv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3peeqdbld.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3inwzkdlo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3oxcjuikt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mnizlngb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ogasufre.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cskuhqoi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cdoajpiq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mivlmkdg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tfrpuvpc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fkavqufp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yirppjuw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3nwxhjtpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edraptqd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mgdrohes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrknsgfa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ppztmzmu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mzsqjwql.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ggnxgdtz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3dvyjebeo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zgfoezso.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uzcrgmfs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uzxafppi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3msjcscqd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cfgeubog.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hnkfqbpd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hqoyekuh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oesckgav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yuyzxfox.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jynvsecg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gmrdlobf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhavea.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gicnzwnz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dentiztd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3eybaywen.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gpslpwwc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kikzosun.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vwrzewyq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3poqasnwh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3btfdgoqm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xzlhizob.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vawuvlqq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sipvmefu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wppllgzr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qilalssv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qnlujpak.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lrpjdrbh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3noabkfnh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3txvgvevj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3duynhegi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zepjytvj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lknijmkp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yapbcwqx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bcjywgzv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyakbtrm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bwungpwy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pftfhtxf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3twztksdf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xruuncln.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hnnmtwzk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3knyiujkp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3epwadaka.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqwqsdvl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qkgdcyuz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3escbkwpe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lksyuvhf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3psfmkgjx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3grwbyfdh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3occybdec.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hupdtroh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3iiakznli.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tdeytgdw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qfihflyg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fomrvafd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zutploqu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rjjdgbjn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ahilvpkr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3suggmkre.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xbmawvnb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bqphnend.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kicgoakb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptkdumlf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gmmdijeb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ggisnpjl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tguaqrjr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ihwvtfro.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xkujywwj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cfbcnjil.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fbvwvlzm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pyujiwfg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qqvnnqcv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dyvqkvsf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iovgeict.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vqilugew.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hmywumvy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vesxkrmn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kmsaugiq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wjsnwwcp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ogyjmosr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3phzcbfqr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pbklxqhy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lbtalfiw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lczffkxc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ztpgbsfp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3beodcgxy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ojsjqqzo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ofmjhstl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uhxnigws.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qxreosli.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hmjqpesf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xseeztod.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qhrfeukj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nlqptbkk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tidyufki.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mripsguc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jitvtoij.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qzcipctp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3edwasxqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zgycydvo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xydlhclb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ngojrksx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fqfosfup.html


<!-- 参考信息 -->