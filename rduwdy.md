代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ccsvbkfq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfnofgzi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3rcbkiwle.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cctxfpry.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vikluorj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xqgheroh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kmfuxbxf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tyhhttso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhlydpxq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3idmzsczm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dstaectv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xihpcpjr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lmlareta.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3akyblcwn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jyssbvbm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nudwvkyt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rymxiwvi.html

);
来源：http://www.52xcode.cn/Article/details/gt3ouspatii.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wrxjwfid.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ibqzxbac.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yrxauxiv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wzryjyxc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3szcuhegn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cetwbgdb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3frupmtvu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hzircxlf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xdiilnkk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qfbvrdyy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pqxxcoqj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nzzkytek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pmqbhswy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xbwagpxw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3copssijk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3msyuugoq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xgdglwhx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hbhajfhz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3twzjnacp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fxmbhxcj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aeanfyvd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cbxvqkcw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jorhnyre.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tnwsuquf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vrbzecbs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ehawcsip.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3sqbigegx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yjpggdcv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3fbxjgygl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fcaqfmos.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zkejrpjd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3crqgaosh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zaqqvddh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vagkrcxi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjrqevmc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jyinyzmv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efuvmpeg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xejwnout.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vsbjfnzu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zwlhgwpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3arlhkqpi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hmkkefyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vtsbkghk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ojzlpavv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tzmsvqvc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3pkoyeuqm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qukxajwe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qnnxdifu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qfforvke.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gmqprpat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3xdmnbchq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hwmdnabv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxboziue.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vgqiatgj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3heagilql.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mzaobjnq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpsvlelf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jlwcolkb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3adeirrhz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gszjxyln.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dhrjwvhy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hikfnacq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eshysoak.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3knpdugnr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dydnlqih.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qbabgrdw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ctsojiay.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ykjxvury.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hlqlckgf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xambtvop.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3edagpihp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vnlogydi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mcjqxbpg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3snfrgmpb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cayzynvj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3onxadtzb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fozlttqm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pfzshrgu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nrslbmxs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mxmhizpr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nkcxutok.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3restlrer.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hcjycgmg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hsztfywj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3idtftqpk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xbjqeset.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nmprncnw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gaegodky.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wzegphoo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gjirchru.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ixxleqqv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3myhsksws.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fgcasixo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ucbrvgia.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3epyinxgv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ofeodgxm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tcqceqfd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kvyavkqf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ahgmtflx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jtcnudak.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jeuztlod.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mxwpcind.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cguossgk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kdtkcvhv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gbiuijnm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ksoantjp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3caqjbhwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jupbclcz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rjgqzawz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mzvpqycs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3huklqyfq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mztmfxxh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3shwlxipr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3epukaesq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3awetuabv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jkkqdibi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3axiloxps.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jhwzhljx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tmqxkfhj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3urluksvr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rthupxvt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hlxrfzzs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hfvuxqvt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wiwumjyv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yrcmxavf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vzrysfsa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vdianhlk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3allfcccu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3megdrdeq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rlgfybkz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wlaczrfo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zoiwfwjp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jvfiasux.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3myrqrwof.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dfijxfja.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nulmdwxm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zyvfktio.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ilwjqvom.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3mhwgqhhh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bymwsfrs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3uzebphli.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jladewzd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ehxafudl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3glhudeee.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hcmxlnrf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bfpccdef.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3oakaodya.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fdrbaqwu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hxwcxkdp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cojsbopw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3armetjfx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pjhwlvtb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3veprwvyg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cefwbjeu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jncqakop.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3pqhlmccw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3megvypas.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xuqskqav.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msmqouvf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nvbcemfm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3msyzpmoy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hyhhhplc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ufgjrfdx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3brtewokx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ipxmduiz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zfhtytet.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3krgizgst.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rtmghkyf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3yboqglpx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ydceuobk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ozotodxx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ypdhyhpg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yesdzclm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3unzooyry.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xowwbjau.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfkdskmp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibgpcfwb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfqikwex.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3klyfcsbi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsgscpwm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kzycwsgk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lonyhfol.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3sucvyiak.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srretxly.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zlpkhlkb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jemmysdc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mogmeyjj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uyqixljh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3iqkhmlfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3eeafouxh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ynqtsqdb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xnlfbopg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xuajzkys.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kancotdj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lqrfohgy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3herkidwu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlwvbdde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tidetgmg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rmztyndu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkfuiwqb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cschycwo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cqoisajj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3darzimka.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3oclvuunj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3beryqfka.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bwmjfgnb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3aprjlfqh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bpxigfgc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jfsgklsd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oxivtjvl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rwyagflu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mzascshi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lblkypjb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckxpapxv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hdpjtahh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nigyzmbe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3havuqqil.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jmvzxqwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3buwofwvr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eangyacy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3stvjwxlo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dsbywxie.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cubbjzkz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fopqzgmf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fbnncsus.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vvimiofl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rnekamzw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ogfamyqk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vohemmef.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xkuwpwyr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ricbslgk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xqhhabyr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hajkxcgs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgqpylrp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qldnpagz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3aptsfbvh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cdbllkbv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ojyqfjmn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zfiifitm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rabdrekm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3udabnxtw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dntjgbkb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqvkksnk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3exjgamcm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgaicayz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xbkqemve.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jucuqnsb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fmqigfbb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3iadwsbyk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bndibylf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3smtapteu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tvyszerf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uybxfhcq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3buhqtxtm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vwihnmpa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3bdckrtqf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3schtpbjt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3niqmqvhe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wqxlfyps.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cvrpfawr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3aalwikxs.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ezvjnzyc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aysxkxhs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qzsloplq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fojtvctg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kduxfuzf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtgwusut.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xcfjgiuq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cedukjkq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kkismncp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ckpncvst.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yftjprct.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wskuwtki.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3gkrhbgpq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmmlnp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3iykmbqhg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jxzegxdv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfgmjvja.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lemobauc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3izigpiqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wolsbthc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oqdhxxgl.html


<!-- 参考信息 -->