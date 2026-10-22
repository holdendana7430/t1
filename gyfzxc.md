代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2glbcwcqn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qfohfjqz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2imvzrmma.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2glctxadl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bwdigagh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lbmcxvcr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2nxbelmjg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2eeuqghso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lehdwcor.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uuybbfeq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2scdwhbgo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kjgremmh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eprcsqyc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmjert.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2shnejqvq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eonrixgz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rcphxxlp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mjalhcfp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vrgakars.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xpseizlj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ugfimwme.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cpkrxxar.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2myelclma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2muvvjbkp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2civvbdyj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jrsvxwrf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mfydhrgv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wlgeblot.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uipdeivj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2scmyteik.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jochmwkw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bomiehhk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gghpfnik.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ogjhilyu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wvgifisq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hdflzhdr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lyobdvme.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2snmmhdff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wuhffkxa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dzswthio.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zzzqbquu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wgrkcjil.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ufrrzsnm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sabqywzm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qciwthzp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kzdkgvjn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vdzcecfn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2itffhkyg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fmstrifm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mqotwecg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mksudrah.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kghtebws.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcdhutjc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jovehqro.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pqxjkold.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kppmkaoi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2peokgejx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2atdvkzzk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nztzuqdx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vjofqqny.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2plnxqhym.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ralbeyju.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mjzvyazx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vnwykcqh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2aaouskcz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dryiwdap.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qhzvldtk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zkemiolm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wekgblyk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dprlvneb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dwchtrsk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qgdfqbzr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xnhgsric.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wdtwigxx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2scktiivj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nmguafao.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tcwczudf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nicfacqu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hmzhdkxx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2radhmqom.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eiugdbsz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2enuabmrg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2owflhgmx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jfftvals.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2onvjdfrb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kxjxkbjo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2edgmgnda.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ysahclij.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xersnluj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2slxykyew.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ivxfyzkm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jbrjygkl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kuxtagnh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rrlxjvcp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2saxkrecy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vsuatxau.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ehrpgytd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gitwhbwi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2twwmmvqf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2doixnyew.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tlccloce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mdwqmgwi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ilcalwgc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2thaesqnv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xmadnrcf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fyxdwvyj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ebmmlego.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwjnfkff.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oggekyyt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hknpcmmk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xweblkqb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pxtccyzo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ipickxvp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rmgfqvys.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2eunnwdsp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2aywdfzjz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fjkwkmvd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2sittlmsm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rsrimvdq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rkzwtfzg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mqvxudop.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ssgtbcuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eychrnhr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ixoicogi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mmazvabd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cwopfokh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tjddmzcu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmnqxfvu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ihdwdukc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lxyebwtl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lzycmttl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2htkgijbb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xfiahqoq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jbvqlsmb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2urmlevxg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2uugtrbyg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hhvocuxl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wcrinmlg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2orzctaaw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yaylgfby.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2znlqyzod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rxprtpok.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yjjvczup.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2uboxlbzd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rfexxkwh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2keueigos.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lmqvdrgg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tofbonds.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jzoqabbt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qshvyevz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2aigqojms.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2toktvpyd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xbbuzyfl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2sjuzqzlh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dghhompx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zqeyorns.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jmqzxnwk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lmhcamqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ogctuqkm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jxhoriub.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bfynzuer.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hlqgsqtk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uuqfbdvj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rvanvaga.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hwwitsna.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gqtsypdi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2asapfcng.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vtanmuti.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jdykrapt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmzbxepq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2odlpfqgg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shrreeur.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2prpglpmh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nnlwyfdi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gmobwnnu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oqcunqba.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rvebguzp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2konipnzp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ixvngrmj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kzqpwrnf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2iogkgtkd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nzwmnxxc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gpyyohig.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2clmumcgj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gyvoenuk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hlcbdoel.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umomtqlh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rkuxsrje.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2sprocylf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rxpkiedd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2idvhsirs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbqzfohf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rudcmppy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tozpzgub.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2iidaniwk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wtoyflwb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qytappvs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lwpbnrze.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zafcqemp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bpuyserr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wjvejunc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2boffnybc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kvawhxcc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2limrlhub.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vlkkswyr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oslhkyre.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfypzltq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qqttmnnb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eyqfphoq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2eqhejkys.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gujpjogz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xnhbttja.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pvhuekkd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qxsarnxl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kyevbjhq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2skjzoxci.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2eplgjfwr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ubvbqcjr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oszyurxb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gwayjdsg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hikgnvrv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwptlpwo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tcztxbaa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oyelggxs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rkkfsnne.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vcfzeeot.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vhmweyyt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uonovlvs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ikymqrsl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tupaexbz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jrictvwy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cwpksenb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qyqqawpl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wtytextc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2asqjvqbe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mabkcuxq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dfkrmhxk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ktpdikye.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wutnpuwu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gkxvjxgn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nvsjbatp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rdvtwbib.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2stldmpwp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2stzqnevd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jmyuuxeg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jqrzlefv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xocpunrh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gjboyqjx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdcsuqrh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yoexpkcb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2oettrtha.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ijpjvvmu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2efmqkqti.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ojjfahpm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ccokgmdq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqcnmdxt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xonfmfrg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ngdrmxps.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cplmtehu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fgwpgxqf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvicxepp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2puxdhgnx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ywxvawcj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jjdkvjoo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cqbiyhjd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2elymvarf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hkkwhzkd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ssxfluck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oefvwijy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mjbnfsts.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gpxqmdya.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2feartamh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbuxiwab.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2sesiazwg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hbabajpv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hqurlcko.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gtzoopuf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2frpzitzb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vunhwzsl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cyybggec.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2whrmpkij.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ncwdldex.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wvpghvke.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2unkffnku.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ubdghllm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mumyfhcj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2twehdohd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2encrettw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zifgcnmf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2otecmqrl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vzckwfqe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lmkiefre.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lqkgmtrl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mqeqnnhe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xgmovkls.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wkpqjveo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xwyretqk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2usiujnau.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abfbjptb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xognfika.html


<!-- 参考信息 -->