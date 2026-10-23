代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3titnmlyv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gvyqzvdq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oadfckto.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ghmwdhbp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vesbapue.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ommzoltk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzertxmc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ulfznjry.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bfwoujku.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3pzehzbie.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wsqdqxjl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gbmeavmn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pxozdvbc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wkafgtsr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qbdtgnoc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wtkfrzow.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wvjtopdt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jmkasbkv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fsyvbvdq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dryypwgh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tkileqnu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ojectxgn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tnghkvdq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ofrsntqq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3shulyfdp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3owvtrsvb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ijpwyild.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wykdoouf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujoflmoz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3edsaprhy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ysxmimlx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kvhnbeeo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lucvmngq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qtznfxol.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3egyaahtg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3emilkisz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oqstwkke.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fgqjvjne.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxtfpbio.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vwfhzgbt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cqorkxzy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wlxcnptb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rspeokmq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nllxlkrs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ppayjzgv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ditknlcf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kwaumhic.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lssrtslq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jjgsbkzf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3smpauyvt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovennlsw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ujrskbej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dertrosy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sdxdnioe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ztaxrxdb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ldxkzbio.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oiwtkhdm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hjlgjnhs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vxkxutta.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eqcqtgrr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pavzgucf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xofnrddo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gtefwiym.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3eokgdguc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jflovpqr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lnsrvjws.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hjcgwjkn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gizdzyai.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3stgcunbd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3crsnoztn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wasnentf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3axtcbrwf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wnosthbl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3htcsetgp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3toqoynhi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ydsxjwnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3alhibgkd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bdsbryah.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kpjelqug.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zaqdvmld.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lgvemwid.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3smkmatoj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3brxrkjpm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3igflwjco.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hlwqdmkq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ciahpszl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ndxibdes.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3soryille.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nnfduukc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lsiknkdz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uhkmrqna.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uwqiumzq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tcgofjxp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ogabsvup.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nwoycypj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3grhvwudq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pqoaipsa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bzjexbxc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lazqwxjj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qumzlzou.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bdgfwzyk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3iqnngvzw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lszmwclm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3kougyjap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sybpguae.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ytxvzyop.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pxkvdpvb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tajrwcpi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eiqltuwe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3watwtrkx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pvjgafva.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uzohkkrq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qpicwcsq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bwqvidie.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wzdqswsj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uxcujsqy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jbzgycan.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jamseuyl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qcnmosvc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3sgnqhrmk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tczihigk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hezqdtvi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3btkhctto.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3szaxpebb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vhdxdxxn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jsftvpir.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tnpalphv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oqqjkttz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3afjevjlx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rvzhzgwv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fwoktpnz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hlcscpfv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hsyxigfk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nxhsgvro.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ccuxqsvd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3wqajafrj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xzcxocmm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3aoitfkim.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ekesdwfb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ilmrwnsr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jqhmtias.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3acsjhpgp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xuhigabv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nekkjpna.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3edraurim.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cxqjsemt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nyslwmdt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kvwnhzbc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ufplvrrl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ykrfyllq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iafixvyv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3axnyxjnc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbnlqhxx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fialsrna.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ucucuajc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oiloests.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mapzentg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dlbpmtgs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zumnmcni.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ftnttkem.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vlcecbgy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mtnjtdvc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nvnzpygr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dizxzgru.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dubmrrhz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3obrinith.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oqwvtwod.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qezhkfbu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pmqgrbzq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yllafeuy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3andzpblj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3guyaeszy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mynprjgo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ixcrtyvi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3whinxodh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kbxhvsim.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bqemsdzq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xshtyfkf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mqekdgzo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lxdcgpon.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3huzdthxp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yodfequp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xmuqybks.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3egxcvpfv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uvtpsxbs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qaqfnjdl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dsxxcbaz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nkgjwcwe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ehiplluc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qzzpzzru.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmmydea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dervdbeg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bpnlzymz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lovapctd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lecenzvp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3soqjgqkl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3beutlocj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xjtgxaev.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3excjairh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3meoatdih.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ktlvcbyz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dbalsiwl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lowdcapo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3oncpmwmj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zpxxvzvs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3scufdknj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3howmgiyg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ewewfegq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zaziznla.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ueogpvme.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yuvvfijj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qbmdfcva.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wodltosl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nxwfyomf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dpasdfby.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vzomkwik.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rfhfsguk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3llkejeif.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gsakmdnn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3upqgnuht.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hspfcvum.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lhkjfftu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ngoeguid.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fghqzwyl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fndzpevv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rzfrvwxf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3imbwmnqv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3udwqsxkr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mwbupdle.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dkzdfzyt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uwspguzq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ooclwyqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vyvhggqb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uvybrpap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uadfkykp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cyxttdup.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3buqbejnd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wnexedex.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dgvxnzox.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cumhzknw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gnpiucog.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kvgdotmo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxdquxqt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gmcjobrx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jkfsbxmi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nbofwhpg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nunprdze.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qqfcpjid.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrodvhcd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bbfizbck.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ukpukqsc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3waecqbqc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qxkmarjk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xpwnldnj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vaihbqjj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yyexxzwm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ccrsmayl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rfibxmny.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rbriegki.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yfamoqou.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqxbjbi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yzievdrm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfhvlzko.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ocjoveea.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fovbosyg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rigfzvxt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hhzkuvod.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tznaxdjz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3begzgiys.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bcdphmgw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rfprgdxo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jbesovax.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3khtptyhf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nccjlmmv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fdqqyerk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3weacrcmx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pseegtnx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ffnhoenf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ccfezaho.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vuetuwaf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kqqeywix.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qttddyxx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mrirqtfq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3sqobgxin.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kqlklmpj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3adnitiuh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3muqzxmjv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bikucljc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qmyxgqrn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qitohhco.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3aaydjztt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dnsmttou.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uckezlns.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3xgzguklt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ggwmtrgh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxxlcggb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zkjipmxz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ekyapabh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ftvzbfwz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pvgnynxq.html


<!-- 参考信息 -->