代发 wailian999

);
来源：http://www.ydjk.org.cn/Article/details/gt3sxvdrpkr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ceqtnbfn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yookkhva.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqnsxber.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3etmjtrfu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fbzzwufg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ulduhibo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3aslkuqee.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zvkhzpub.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lavqrlrk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3amlokrwp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gkgertwc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fnrogxsh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vfqzbfzn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ykwxqmzg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xnkcphxw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fgallnps.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hualajiv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vaimkaka.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zpsldfuw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3obnzkcwa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ybdlholv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dmuuagcn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fzxomdup.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3lupujlqt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3biaeuulb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mysjpiik.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qvpvmuoj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipdrskxl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hkzpvjos.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiifxeyy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hpoztosq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ozgjkvln.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ictpdtjp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3giqnuqyn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yuoqxkal.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rkvtwtsf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xyfwpvmo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kilgdsvw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uuufhwvu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3htvdpzjj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgkszkqq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cmopxmoz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3roiliqsh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jvyeycqj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmiitb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gywbvouc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ubjijkow.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kjigoprb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xnszcakg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zbgzqoij.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nwinhquq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqbwemmp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ingioezk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ypcmikct.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ovrkthmg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujhposva.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rfgvpfsx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xnskbtkk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zemybdci.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uhusjvoj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gcgddfks.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tcdxyrih.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ddatybmc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3upcvrpsv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hunpovwm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3zhzriftw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3alebyjir.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ilomndmj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qlejzhsx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rfocttud.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3imaxfgjz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mamkiywo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3efcwciem.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mfyehhou.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3docetxqp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qhfjalac.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3urkihcbj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bqkfnwhw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ypkqpbml.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3nnshlowa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tukcbqjr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3oxdkbvmx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nocdoubi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zpgzekhe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3btcpovtz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3akwolxsl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3unglotdd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tgkkbqoi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3yhnsbcza.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uycpkuzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3twfzosth.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rruuqtyl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uwaklbaq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uomahesv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bytetcsz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3spkfaoug.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3llkubxjj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uctwrmrw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dgztoexf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3htgblevt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mziukjbf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pwoawxcf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pjsznsvd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kpsxyggw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iseazpeb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cdnacqyd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kddepqxx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uryoynwt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3iigevkha.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ungduixy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3enhlvnxz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ltquegvy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ibokalzy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kvyzrvtb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gwthbejr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kyfautsv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xmzxpuaf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dttiwqib.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3swsmejjo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3goskyexz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cfkbttln.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wwdqxwzh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zcldkusj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rsuzxfog.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qvfvppup.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kadrbviu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sbgfbljj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pmzvwvat.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3grdohhfw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3eccvayuv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ashasflx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fwebkgnm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xnpesrii.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xprbpsmc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ztdbwgeq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3molceufe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rradxuel.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jerusoch.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fmuscukh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jfgkumbw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rnvstrrq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gfdfnyhw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3flzyjuwf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nitdzncn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3djzrtgab.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sprvzrop.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ikpntyaj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ylnyjjvi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3alngrjhb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3toiuqiio.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qykawyax.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gndrkusl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3afumslmi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3awmulouh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3apihmyyl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jmppimbm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cbtpajng.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jxgdpwyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ltlmrhwz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3simvmfrc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3btynxiod.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ozcwyslv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zscjdlqw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3iginfklj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3koqsqgqo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mamtxgyz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dfgbeota.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xetqevem.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hbfduqzp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlkiongb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojxghepm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nsfhsobl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqaizvah.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3esmmdftn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yobewqzj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lnlyhboo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxjoegwz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qpmwerry.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zrwljuny.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rbmmrsfv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3swdmlzco.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3omubmdue.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3docmswpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3uptzvjyg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kdresysx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtbgpota.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ndnnalik.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3loezuxzd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vqpeowiw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3obcwcmis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vluzxodx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rrknpegj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtovcqbl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xlvpubgj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cryyglmw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gyzttqrw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jyaxubxy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nclpnghb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cfktjabe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fnxnwvrx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zopcpsrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dpihcfjt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ebrmdxpz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3neyflkpf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cnanhtcv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ehbsdhyl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wmmbkmwy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mjpufecn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dzkezbgo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qbtghxly.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgvnqrpw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hdesknoz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jdixdczx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jbrohiad.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3whjtudta.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gddkymti.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nmqlczpf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bgspzwfh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fnefyprw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lfyrakwk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fyczxfvr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qqubcqff.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rlocjyfd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dpfomhrv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3myuiumyq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hctmtsfk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdiwmxhn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3leuklajo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xnngqmit.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wewginqf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gqqpgtvy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jksyukkt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gqeopofc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oupnoflm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nbmmjhnh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ahdijuyt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3atdfjprz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wwwcugcd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lyodebrh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxkopcvi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rubbmbbw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xidlxuvz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3phtpexvz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ndiceiin.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fdeteyim.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sdvtzpem.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fzlndnco.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nheeywzj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3yfbzmtpe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aurzqtsg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3udlmpwhy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qiupjqmp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fbxkhtcs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wfuugurv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uywznmcp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mptxohvu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3spyqylfx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3nqdqwjjo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qalxlnli.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3guutxooh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gmgbudps.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xzzydmgt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cajxghus.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lntytkpv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vbooudut.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zwembdae.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jbupzaij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xisllhpf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dypblryd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zthdelsl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bcuxbblb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbzvvqy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rqsatsvn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3abzbrirc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mggcjfft.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3umcwunrs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ijzwxcxn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3povfszzp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jkfctvzc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jhjcvjky.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3fxtuyxgg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3awtefcbw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltrjazvz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ctdekwse.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ahkstakj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vvuhplbs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gnjuzjvs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lcowxsgm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wqcbmlps.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3drigkwxp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jawwpqzw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ldgyozxb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uqwpuuwb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qyvxsrss.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fglfnhbg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3acpntpnd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tfnqufyl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3usebjuks.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bfifjikz.html


<!-- 参考信息 -->