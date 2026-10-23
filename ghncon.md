代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xlvmnhbu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ycuorgmt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3teqbikdz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3bvqnmohm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ashsbibx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lmpdgdkt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gvrqcgwl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vhngenaj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qqirhpyu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nqiwtfzn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mfcakdyt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3uaeyohov.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eurkmbgn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jjxvmgbq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nvnbyqcy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lvhnkmyw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zortznob.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qovlvttl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3soeczyzv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xyjecuwv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hvaygnha.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3eiwnnxqv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxofktz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bowxtqak.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hnxxvfzb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nyftgbpx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xytiokss.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yphtcfbk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yrbdqdxe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wtomobda.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3gqmvwtfi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hshzggnb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3osgubnkm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3evmhbimm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rfsgzgdu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3yxnrlsda.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xdvsopai.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jqtaujji.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nklpltve.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nwtdunco.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vuwpbpjz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xyhgnilq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rowhajyc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3eddrjcox.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3csxgevmq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3urcxdahh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uimjjupc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xwqefztt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3apqcsjgw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3obtagipz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yskymyus.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gmogkucs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctxhmpxl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xucloscr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uwslwyjm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3trqqjvus.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3alysshjt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uhfwgmpo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rmwhqusa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ibahddvx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rxtptknd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3oiacmriw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3eqjayoil.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3uvbhbpnd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gdlmyrur.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hypajifk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yvzhzwuf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tkhccekz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lvpbeocw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3spsqqdpz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ibdwwrxn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fhoplsgq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3crrgmbsn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3omsyqkla.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dtmqbfvr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wwlxtdmw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hoiqxrpa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dwnwafmv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ekeytrbk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3emmzlmfb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vdgopulm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3unxjmdmu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3glfrtnit.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3raglwmcs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3efvvnzcw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qxoovslt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wrymetbc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3fcdqjuat.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zftrednw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3akrdfwbl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hmmkorlu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kdkfmdlf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fugrcell.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hiylgfuy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cjsvshrw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rwkxnjay.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zqntffjq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eqfknotu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rxfkusxb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cisusded.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gtemulhk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sbnhcmvx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cklzzxck.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xjfndjoo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jsnwhbma.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wkghursd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mrpwozue.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3dexsbfuq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uepwswdz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kglqhynp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tswzddyd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qwhkzgsu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rjysddsd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ziouecjt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cgjryzun.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3apneudpc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3swbaofvd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gexzwzln.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bvsxtaan.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hkaxajap.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lgnhonix.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dbjqlsug.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bllemggb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3krxkcqek.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pxfnjokm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qiuaynsp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3mfluewbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tclynwvq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3higjzsbl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ktgfwnrw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3viqmtwpd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3looiupnv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gpiefgbf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xurhjdij.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ibezybys.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xvrcpfqg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3udmhimhz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xhswtbqi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3unvgynfb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dpbojuay.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrdficmh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ocfopyeg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qeaxsszj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3panmiqgf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3auwphslv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3whpfibzv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fkvaknkj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sprkoash.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gybwyvpg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3uernhway.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3txrntrjd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vztehkbu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jsffmdar.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3leemnnri.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sucikjtp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ekuyptnu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zqmfxpkg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jhfinjwy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ghtszcqd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vortiqzw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vkqupijv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pzgkmids.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ypnodbwo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3rmsrjnac.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yzzgczlf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbigcvep.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ktvngkfq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ahbozcbo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3izolrjeh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3raceajzp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3trtpagil.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbblwmpf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hybtmjgm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3koxppdcv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ztfygddz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tvftakha.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bydrjvss.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ryykanua.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3jdyzasdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zffacygo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cfxkaqjo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3sgqftouy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njnmrjpr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oiicoqkb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ellhcisu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oadjcxwh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tcsjqnkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufhgvsaq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mlbtbfzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dinrawup.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pecjznyc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3unxkymfm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rnzftxao.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ffvfxaea.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rqrircsz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pbteotef.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3oywlyrpc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3astyikgb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3esqahofo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3icyymzsp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykvnbkhl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bxlqjfva.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qdjgmdav.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ouaoczfj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kiemgale.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uanxxool.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3enehecbw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xcajtsmb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fmukpyso.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3halmctxl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ntmwzquz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lrdlpbar.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tjbhvnbb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zyudnomp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dmzzgvux.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sglotewg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lktqmrhb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3podtpntx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vaatnoax.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vaqbzxmu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ewywmbjl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3exxiucxg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eoxluwuo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3czilfgwt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yuwsbkti.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wwefwgml.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3buifjmvv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3panduztn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3csqrnqnf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3itssmxil.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tpivqbem.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3avowphnt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3itbxihvp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cqkbggqo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vdmhvzuk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gsmpsaql.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cdnwomws.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vnfbkwpr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zzzuoyfr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ylcbzhie.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3aepwnota.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vneonmjn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlgnwymg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3keppalod.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cldmoqvz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hwmbfubu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ijkwjfiw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3deqxxvaj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tlfrechk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3abeyssro.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jhbzthzj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pspmnuui.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ntxyqpxo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zvvqtwbg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lipfhzzc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zzmzvywz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsiecpau.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zseexesy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fzcnkhmb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rotyjbga.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3uojhrszt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fytxhvuh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qxtkxmxd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zpvlepvg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fpyjtqsj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jqttaukm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3liprqnpo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jvojsgat.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkckcx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qgjrazqm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kxgfihss.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hpcsyvtg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kwmepntb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yaqfdlxd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pfhnfxrp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wjbsecui.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mtwdyfph.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iyqxpbok.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dcjopoui.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdilpwvj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jjmscrgu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dxcplylq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kjbtifia.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bmjkvfhg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sogrrdac.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rouufgwh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nbcggqwg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cfjsifpy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nnxsxrme.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bbpaijqo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkzlnvnu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3iaialxlh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wriueymh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rwvoxvml.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmqohwvz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gnhunqsg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gdauuhsd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lbmzzsci.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3poorcptl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3onxiukfq.html


<!-- 参考信息 -->