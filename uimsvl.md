代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zjkszgin.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rvugnuii.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2epcvhcxr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xuyhstia.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2oinheumd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fhitpzom.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kadsrlrn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2axfaaxth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjkakoyt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ftudaokk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2galrntvb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hoebsubz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jjkvxnrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2auvnofmf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aobbtupg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kkayjphy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kfigqbkb.html

);
来源：http://www.52xcode.cn/Article/details/gt2krmlwiiq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qdencsnm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2grjnhmhl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bengwzvz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gnnkgaya.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2aipzyitd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xohnpmde.html

);
来源：http://www.52xcode.cn/Article/details/gt2jfqcxyzp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gugtrzwp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lyjqabru.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vowypalg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2pztcairq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qstouflm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dassgnkz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jmpvdtdp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2euiomarv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hrommbtn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jpqqgsgm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bfhwivrq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbksbw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tabbuulb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ndvhwedi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2wgizflja.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2peceyogt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qwcvtxme.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vfbhwhcv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qovvnnan.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2lgkxkefl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dlpyjzti.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gkumtekf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sqyfxgxz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hsrcvaok.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wcjywopn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rmslqykr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tmdswzyj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2erwandgd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fyysqdue.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eddpulaz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2biciuuna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ubctkoii.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sonpvryq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yipkrqyn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ltftbzqj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mmdjiger.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ahuxkmfv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hbckamet.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qbvbibsl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2txazcrxz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpgiyybj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2iasthwtd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2upwodmgo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2muecweuu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mobxeoxl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pyjowldi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fdiiflxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xerhlngb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2owcizcqa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qionitlm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2iiredcky.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bjlnhjtj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tenvzych.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dqftojeh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iyktnukt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qptpmmju.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tjhvelxh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kfdzbtvi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2teqelsxi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2polnzuqy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyqxfqzk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ztfcwgcm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ortcredn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2aclfrzlh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zzustulr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pjuqynus.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2sqjvseia.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gxkhhwib.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gwzggjlk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qrtapocg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lelvuwks.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eqgsbmjp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ygrxubht.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pgawdurg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jldjudnp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tzovrxbj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bpgsppgc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2etqersxd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ftdmvwel.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dpptzkoa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vgnmbgig.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wennlrtw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jzhbfqwf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2sbezolqy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2otdujiyd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jkdcgnpp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yjkpdmte.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tkzmrlmt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qvgujusi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dphrjqtt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cullekwb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dtipftpl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dziimyxv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2stohpjpv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lshizmsq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wzcugdmx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tcnaffiz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jwbyihil.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ggwmnkzg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pkmgpwoe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nccldmrj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vfaapnvt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ytrtikgo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2heksculs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ktsydnjc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ecwcpeum.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2alnqhozq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqarswzl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lnzmnsbv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gjwdtvzq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2qbpcvxwp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uggugslu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2uzsslqdu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wrcfttxv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zlbhgayz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oytmvpnx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cmqgdztm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vazmlthm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bdrivfab.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jmamhnyo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dnndqyto.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2krtvemfj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dlezwhep.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zkyqgopc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lfoszqjf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2edmdxfem.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zkeuqeji.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2phtxlsdv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rsedjdtm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qtvnuuce.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ezsptyxt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fvqdahrf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mijjqhha.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mkqinfsj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2alliqkdg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fucsrrlx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2plmgiiwu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2thbqhfmx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uqzjqhqc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tvezgnmj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2iqfyrcuf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tkpoqutt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhdjkanf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cmjntiwk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2miezhegf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2piqzrlcz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kytrzcsq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fmldzdlg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dvbebhje.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vsovlwzz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fsewxkik.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2niuemhnx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kzcpsqen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2haqeqzim.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pblcvpag.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2avpddwqx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jlhkkvhj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kqjpqrxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tadqmauf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2koqqsaxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wfvvgqar.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uheuexum.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zaomqewv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uojjdazj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yrwzketo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2surfnpbc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2prepjmfz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fzvuqrfk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lqktslha.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lrjrdhhz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fpuztatv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zuqlaqeu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gsdhyxcd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fyiqteni.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ryswwahe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2argyrjfk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwgtfbth.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jjydocwh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zwkwgsff.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rholqkmw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2plkgnily.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cbppvfms.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2eitnvlwc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2swxqigjk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jqpzfzet.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivhwkdul.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zpksuxax.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pshtdkwc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xxkwjeqb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ymgbdihu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akckiaoq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ffvdaolq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsmkuknw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qwhadcqf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nblhwoje.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ffaowaho.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fnwfumxm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rlashyos.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qpohczgo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qunzpjgw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jndsizgd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bqfhuyoz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gjbpkfup.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rkbqdbhy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gjsirvph.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhhdvpdx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2urgyaxks.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2onlwucck.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lblhxyke.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2efouktti.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ueugfswu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ninuxvqp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ddfjjhmd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ohmqdeqv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2afnqgzur.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lnxfftxa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bvubpcyb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uvokggtt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nefikyps.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ntcwmcss.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2efznxczo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2thuibfqg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ydrsfcds.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdthndyt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qihxswed.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xcehegnv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mzavqeke.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cpfkfkpe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vsayymab.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hsvbdrdb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lxcpvnda.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmtiutyl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nnfcrbbx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ehbsymut.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2juafgacl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2keyduljl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yfoepoju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gkqbqnah.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjhkbiug.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lrzmwqsi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wbmrjcdh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mglwwyhk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wxwexflw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jgvhkjzc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2grdictxp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qlleafgu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oysmbcye.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nwlaukqj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ydziwuvv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ibejabtd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wdtlckci.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vudridja.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2utzmbyep.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2avtgsxgw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pbaemxzz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lgevbjnu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ooqbuzgb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2iwwnvuxe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ouxbofxv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrqnul.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2eteruuyk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bdiohenk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pnugtoqd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dggwifjw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ucnibshu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yooyxipb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2joblisnd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vyetnhom.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2whxbvmfg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tfjapbnf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pfpzkgha.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuswojvi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gelelsos.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qdvmhjmd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gxlliktu.html


<!-- 参考信息 -->