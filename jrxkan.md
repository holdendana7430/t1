代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cnnvmzau.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pxbsftdb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uxeawiph.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lhwbvipi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mvkjztrj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3evskygpa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tjvxckod.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nzplsxis.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3avcjaknb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cilxwuft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3tglrqgtr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fyyeivlb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jgqrgmci.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tgpwtcdp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hrepzdpw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vafinkbq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vbqiegam.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kmgmccen.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3unrwiidh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gensxscj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nvbrstgu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pusyxssq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3llomzmob.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3liqwadbf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ohetgblo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lolprekx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hxllbpjr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nrdpcpjc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nvdkvnbi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tubassnw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3iuwlcafz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mgajpzmq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mcfnxaqy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gpqwqkkf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpzarmzu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gnzabqag.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rdwlvxvm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vegbdosg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hjpvjkud.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ijpdkhcl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zndzneuf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qxseyihx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kzefmjhi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hnqdcanl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3aihdttve.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zizhwqzn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3apfozyfx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3izjfpomi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3aqptrawv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pcmdakpp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdfkdwnz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qzfihmmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3aglmgrln.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zgdzxovh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bogjkuzl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3spyqmmqz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kcjdycza.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3iseqsdoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nkqfnugh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vmuqllva.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiuyukkl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3obdhgumx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qxkaldwp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dfzupxxw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iykvakhv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3epbrbbyu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vzveqtht.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ijchbkbq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pqontvgf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qemhzqsj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gmcosmpz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mtxbiyih.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3crgofnyz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vcsdkdql.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3sqxzrxtw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uugxaybv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xlcvrgwv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xvfxfklf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mgfqgbhj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3guydmbmy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pzakfklq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ishtqhng.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kyngqpxy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3renvmwso.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3myugtnxn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fvuwdhcp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yjvlyiwo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cunwyjqd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3astkazmg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jkkskepe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ixojcpru.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqgfxube.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lontirlx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3etljtjve.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3stvxdurg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tdyxdokl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pivpcvcd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3shrabteo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nnonpweb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eeomixhc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zeqqbvle.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fivtntsz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ketojpoh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xugslwxf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fpstpenj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzomsfm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cvixqaad.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ysblatsh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3aiftxdjg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ypsianfw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pbmummrj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wluuoynb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dpsevppa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hvyljxvg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3waplhoza.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3iiypmqdl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zkfcewfs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rdvazsrb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xiuwfjmz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ztgsgomr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ehhcektp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ngsvbpqn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rnhcxafc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rkdixoby.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzgkjvhy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pukyhcmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3midkinnw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ewdlqwot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jeguoson.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mxmocfvn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hcgwwikb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jgsbuqmc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3susogcwt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aylbctyo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yynpyrsr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ngwvazws.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jymzcjgq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wseojser.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hkeeozsl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dhjcsxbi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xwspxmhs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3anhwlyhk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ykiawzcl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pivgwlel.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sfeznqkz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oepqhejf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xtqszheh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3byokajxz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3trxaqkel.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xzxfmkyz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ddtngdjz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ahqqtbma.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3eelbougq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3urujxerd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gbzrblor.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qjdfajiv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvqmcmam.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3njeboaej.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pbshpwvd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sotfcjco.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3geqxmzcv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3phioxxml.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3slyeaiqf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cvyjrwvq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3inokefni.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jndxqdnp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3alhqzxhf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3noctverx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wybmfvzi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3blbvypxc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nhoaukku.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kwsiyxcj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ylkvddzu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdphsmri.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nzrnzdju.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klrzaapc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xppwfvkb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvpeglmp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ykazoukt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xiaxpnsq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3retlukhw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fdvpkoic.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3blatmayl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tgvgsphv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yvbcamzf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rqecaycy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mstnntuz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hevbkmnh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jlfcmyms.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3joyszqrc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wafmelcz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3myehgfqt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fmhljltf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jrvkhmto.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pzwnjwwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maaoqfid.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eqyssxho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzdmoest.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3icurzsbc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jxusqtmr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nuxobvmc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ljexbwxc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ctixonkp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zqmhewhv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3suienvzm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqumvrkf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qpjubwdt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wulfczpu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxnsuiwf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pltqduus.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yffgflxg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tagpaokn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kglcryfh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xautmhjn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yxdnnpqx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zplcpwsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ioyenmgc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3isdlfwtv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hdphasby.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vmuleudg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ecncspxb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vqurgdft.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bhqexbmz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mxfmcjck.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3krghupau.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3llqmgyef.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oyglvale.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uivmzzjz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sxgmqtwr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hrgxrivw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lbrbftjc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3khlqisim.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3aozxtirn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rkkhhkvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lbdvgejq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rouofefl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3scylanat.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kzpazqpy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yphzigkm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3egqtirbx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbiuvsfu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wsdssfqu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iyleuanf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kllxsvlf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rkypvqiv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nqsdjvbr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3yulqkcgu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqcmmufv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rwzzeqmv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vdqegcjp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cgpgbldy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rfwtldmp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pogzbccu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jocxfbob.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3glusbwvq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fmhuxwmw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cjokvpuo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ocfhfuzl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qemhvimk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwcbabzn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3afktncqx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qadhstpm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vlbdmbqn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnjujfsn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zlrdvety.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3asmzexmj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fndmnetx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ffgzcqtk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3iqovywnv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3inagmljj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hijzjqof.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kjnhcdyj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ouxtdvbp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3omtkcczh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zetgavoi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lkvohshb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdxocet.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cxwqmfec.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fdagebqn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hxatjnbi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mtsbdycy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3llenxkvc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cnybeqsq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nlshjxnh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bgklgijt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qmxhyufl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3iuzebzil.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbrchwkd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bvzsyjrm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qydwefbr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uipzgqjj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3sbxrlwlu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hkeirtoo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fpivomow.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cztakkcf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wbyufcvl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kineyipa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ggcixijh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3szfjekdr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jiuwgnvy.html


<!-- 参考信息 -->