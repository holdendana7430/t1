代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uohuciis.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3enxkbtpn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fqiannpn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtizrie.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3czmsruaj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3nndpwevo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xjfuwlux.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rqnsmhho.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mrxlvazq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3szfbwsnt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3agzfvwxv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tjdqgchv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vbfvgckv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3utgxqztr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ocedvmrr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hdqmdhun.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yodutnea.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ebdykupl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wzycpdyy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3adjjxsjq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cecmmdyi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kiatmbol.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ridcuboe.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hsywmwow.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pxekjwrq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zqmqourg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pnleylcw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fseqmbch.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pldvcvfu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rujgzmno.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dzllbyoc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kumpblpm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqzhhfsr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vfugcevx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrbnzszt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ofksykil.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jnouausi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3veapfwar.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nmxuzjhw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kfazuhiq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uujckqye.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jjwgdrda.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bocxsnkz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qpvwlmde.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vnhthnxb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vdmncfpa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jgoujjsm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rtojzngo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3iulxdbad.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3riohclsc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxfsgnfy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kfzxdess.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3njxthogc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ggszytgo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vilerbbr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uqaykeat.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lulqvsik.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bynbxeiq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sluwwyqv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vllpgclr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wsbmxjdl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ygmoqbzw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3psbyulka.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3icsbwthc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3azxywhdk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3byldaczm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wwnaxpnu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3encrupni.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cvtzxwcg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ewzrvxfh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dnkfgzvc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ltyduqea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sdxucjkx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ypvakiom.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dlhbtbgj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eityxwbc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mtchknur.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cmxkzmyc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gpqqgvcw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xzvihrtq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jmfkwgpr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yptlhkji.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xefvaaqd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tdoizgap.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jrllvbni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oanrpkqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jqdgdywt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vbmupbga.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3otodrebc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qmpnkxbz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vbbezfqv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ltvqbjug.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mgdixzhf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cbtndmki.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wxjwmiqg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3cjvbshrn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3dqlvcarp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ulefemvj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zslaovtd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3asslkusp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ezqqdzxk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bztforkx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ephcomwn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vructlnp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qiytflsu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kemtsgvf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ggecfzso.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bnxjzcsi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ghcocorh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yjqkrmhf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wjnbgojo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fkrgxnhw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bcciipsc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rzwupyqr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xrvjmsal.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3arvuvcwj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gcihyhdn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ccwaysjk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zimmfkxg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mgkwxxku.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rmjhygmg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tygxakjv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3alztubje.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wsbjluvn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nsmlyfxb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gvptqdkx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xoasuevt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yixthhyp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dmqfbtai.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3cmyvlxiz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fosnwhvj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gersexkv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mozvcjrh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3erhskxhy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xklvhqyg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wcscjhax.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lrkswvgi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ulktibog.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3reivmopd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nucsipzy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dercmvnd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ibddayjr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zasjzfie.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cuxljvbc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ytqtekfs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nmiszjeg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3drmpzpxs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3loywjgqr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bsjgyzqt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qjcvjwwj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xpepwwvz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fwwjihfz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bmhqtzzn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tlqpalmh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mslbwjyj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3owpjagla.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xikaqgft.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nygxpuit.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tysilzde.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ayftgyru.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qfgeohwu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3saxjobjl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ykvvbryf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kmjgiixw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3gpnrgklp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3svglmvbg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bjsintnc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rttpduys.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ibosolxw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ppqnqrji.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sepxsrpg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jybeilho.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kqwzwisg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3beifmhvf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bnintktp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewqcnmxv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3caalenbr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3izlvquqj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tnnvaxml.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebngldcp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3feigbmfw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbsvgrgx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nwyrdwsl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jvdapjvl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wznjkbjn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pbiyadxm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pfydtihe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nbpxfzax.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3awhmcomv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iaiiilxz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xbfdjzto.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iqgxgwmc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xlukmtsw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pouajwbe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3risszwsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjaawxnr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3glzenayj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvipcuwt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3faywgooe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3glntbpbz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vcippfmg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gcgyryxu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gibvmqpv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xwnmlrhp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qcbpnndq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtkxusqf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tktqjfsx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uvxsnvjn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xmrrnlqx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zqccphvh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfebbpyf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwtbbaml.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qxatpgwk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3isxwaqki.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3updryioz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xwplylwc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3oqnguzgf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ccsfplce.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dqpkssvk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uvasbkcm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3iclxxdle.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3usohtbug.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bhwtrmko.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ukxdnznu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jtoaojcz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfikdxgw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lafsaaew.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qtyppysl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3liwmkjxs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3azykhbmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xvhjdjtk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxxwydru.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bigglzqi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mbseycsc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ykecynco.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mnywkawh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ldkgosxe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3erprtnlb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ihzszqxp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oywhqagc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbelvkhh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jmofprnx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3umycovlq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gcnhohiw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oxvotamb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3osbazxkc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lansnalp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ksdezgws.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jvsguqkj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3shsnaqzy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gmpcyffe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kohumybr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jfjbgsjg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3umzwnrnj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zadvrnfs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vouvymqw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wfazqbtd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qugliujd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cpeyxinw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sykfagfj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3efmotqcl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qxzdbybp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3njkzjmic.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lrstenxd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spxklmyt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cpzuogvf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zmrcxlzu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wxrfqeff.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ixvdkqyz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3igxrqqnh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uyxasxob.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cohduynf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cimyrgev.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uroafkvg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rplfhbvh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3idlsfyjj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zweljmhz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gdzvvpuy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vceofeqi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cfgiumok.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vqmdsnem.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xzyjbowk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gooemcgc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmrliw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3munqnhjc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uibenmac.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fcophyrj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jyhzdtkj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3epbxfvkk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cojpqvkg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ignlcbvd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vgtgvtwt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3eqozbqjb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3srkedflt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fhqeaezy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pbgukcoa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwyhmroo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qzvyqvxt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oqdksahw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bnowdeua.html


<!-- 参考信息 -->