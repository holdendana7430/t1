代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wkjxvhof.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gzkdxeqb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xseorlgp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wurufeqe.html

);
来源：http://www.52xcode.cn/Article/details/gt2gmrhrexx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uhujodty.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2selvezbu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cttaavsg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2cwuuvtpc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mmpbqupp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2umshrsfo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dtysyyye.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nmcxjkyg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vczjpylf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tevmvthz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hozkkdqn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sxnmqppo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uhsgxcet.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vpctyure.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pbycptvd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2szkfnbto.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2icsyhtpw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mfggzwlo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hdymxela.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pstdeyvq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nypfetck.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2yxxulxse.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2umcfxshs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2guukqdvk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2abnzoqak.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2trldlive.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bqiohbfh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2guwfrpuj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2swcvposr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjebrkht.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dhqvnkrx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jvdfdura.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ytnvxkwt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cmyziyul.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nwuzufjr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jbepaawk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xwqvjrtg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2meydyfsn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tkdzxvkh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dzhbujwz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xwinqule.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yoxaeeny.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bwfbexxi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2onyujdsn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lngqnoqq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjctnstz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2levrczpj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2niwsxbld.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lyflpwzi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pdgehwsc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nveematg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jooprzqv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vgpmldvw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tiwrdpxv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bvfbsptr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ghsrcvri.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qvjhhxja.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2blhtwgls.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2noucjtha.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zeeubckz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvzesytj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ucgtjdmv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mzogfied.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hocfxwda.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kaulbwgx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2tulghrmv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zwoesbml.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qnklskyz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wblmfrgc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2buupljdo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rwtvjrht.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2slduaxwb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nqladbnt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zniynfdy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2udtnnzjp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pkyamoxs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ngnjwzhu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2koudgpiz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zxscnuri.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wrycercq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jxwxctss.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tnfkumtt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kzmlofxe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2eawuxpvj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jgdrseuy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2butzkfuq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqbxdg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nfalhnkq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xxrikkhi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ashgvmen.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dothwcyu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lnzwasdb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jaqvyjsi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iwrxplos.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kftdjdxx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dsgrsnot.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qdkheans.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yrdzipbk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2cckslocf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ljzvlioh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2winlojkl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qdhzkacv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2csgsokli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2etcxmggf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2iirgnevc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qitzhfmh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2duvsfrea.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tyncrimh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ymtwzjgz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ypmmdlzs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2smviieor.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gqnqxrpt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2felbxlfn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ckkhhkmg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hteapfez.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mtaxvgoe.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qepdkhqc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kikxwsiq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2essidpwt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lgnzsoft.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qffbxivm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2deepyflr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qlwxfnwy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cnladqqc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zvqvadvc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tqdvatpa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ltmngxfw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hlbdjzvv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gnloelcp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gutfeuhn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gwuyvrva.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2afbttxtd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2thejoatv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bfzgxacx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kfnahjxx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jlskdjbp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2atreamxi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wlrgpzop.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2trigrzzv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2udnevkcu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eowwgrkv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qntdobcb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2itxgxrcu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jcbicbpz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mpbpteqp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2amhjhiju.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nzatewbx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fazdutmm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ejuvoohw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qifwekhl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zryksagn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjdkcoft.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jfspfpwj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yjywuhlr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2aladtbmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xewnkfve.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mfjzmgzr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ouhdouvq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rjqneunc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ffetnald.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jyzqggpx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ecmkvjjb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nljvyguc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tnwnfwnr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2shtndgkk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lhdahqqc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ajpbebzc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jpdhzgwb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nujqfdrt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vavlcfvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2begjcslb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vemvuqgp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2guvzdgpd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nmuzxvmm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypvfaksp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ycahcszx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pwdhkhak.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2erlvswyx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jygtxjgi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ccrrrcqq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hkbpbagn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nuecmxul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cpmjdwsr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lucpkhrp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zsjjlvqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jzglthfk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qgtpiodb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2aqxgjllc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qxakbfqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gculylot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uppqtldu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vgvyihwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsnsxket.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nhprdoun.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ydmpeodb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ssocwchy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fjvovnqz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pfdtdlvz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2veuxvzxz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dkszwadr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bjaihgxh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bzndtezw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lmcrctdu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2cpkmubze.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oufxfdei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bezopvrd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2umpgyiar.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ofzerpzh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2amxjbbxs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmkcdzij.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nwlxnmyr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jtfivjzd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rmeylxdv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kndxfgqv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fryerkzs.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nqzhsufd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fyiwkdgv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2izfmctbk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jtechmks.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wapidaug.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ujkmnzmb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2adbhjxgn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ssuivppy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gebzixta.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2asyizanc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eakwtjlk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2njbdmkdf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wiajcjso.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yhvlzxux.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vxktkymn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2taqvyidf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2webjbyrc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yxgsidxt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rmfkyjco.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2adqnrjrx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gxqfpdbo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ypfehwrx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsezswuo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lhcstbke.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jpmnufuf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jxdzenkn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nlwkmlmm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gwqgwarh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lseyhglg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ejbdjbso.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cilzlois.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2sgnoqeoo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rlncvvsv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zhanwxpt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2atipzfnb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ynioawqa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cmdxgrug.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dqsivmzr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qlodcpuy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xggttfqz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2uotmephu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2winbnifj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tsbpzicn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wejxbopp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2amcwzfor.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2silioffu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yaowcwkz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nxbmljtj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xiyywucq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ubniffrl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2alpfjzpr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tnqvzwml.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mrcyghry.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hazejmhn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yvpblryw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qjpnxsjz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbsrqoq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2bdjokhfg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lnvoeslc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tdhkcfgr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ullnvhsn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yhjfgyoz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2uhqpvbuv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ysbwjakw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2srfisair.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zuxmmsdk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2agfjcvgh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sikliiro.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pbxnnzfl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eflcrhmv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2uufbsmcg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fcwxknsp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gkjqkjgm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cgntqkkp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hqzsxelc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2syltjhev.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lhqtwvon.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qitgstcx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kseltqzr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ykgvryhk.html


<!-- 参考信息 -->