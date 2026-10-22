代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2snsrzrtm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ckssskok.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bamelhmt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2glmsibfv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qglytrtc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ncsmcmee.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ojfennsg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yjmagqqz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ycccbyht.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lpqzzsis.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2okvzphmc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkgazqtc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vjwyynqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2atkcoxpp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zyniklzl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2azbttivi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxlufhwe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2obpgdnyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juvaitut.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2odilufzo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qckfstre.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2idijckxa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wrpuardv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2peijgzvi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rtbqdvre.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kcmjtjay.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mdxqihgk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vdzewerj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xrmzyrzb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2daysrfma.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2kfvenwib.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lodaqowt.html

);
来源：http://www.52xcode.cn/Article/details/gt2tjjxodpm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hmstfmre.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ztnmhxzk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2esshhcbh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gdyeixah.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oeeypcev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qchpgqrh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zxevbkmp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cvyfnerv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xkkwuzhp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vpcxrmdm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dzapmmds.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mqqrelkl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wtmuteye.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2alulgbwe.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qntiotgd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kllrxngf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bbvaprud.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hcsxmkqh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ixqnywtx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cucuwevr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2krbrtvvd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ykabdoze.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xuxvgtsq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wfcjfjhn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ljopebio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2atkevbor.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dwxplrrf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjcynrdc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hmldpyrr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhasqflz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rrnwcjep.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cbbojayw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ywbzxlqr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jhicuekb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cakxacce.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jcvnahrq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zvsczcut.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcwykhdd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uhmbqurr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zsklxfjc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2djsqltfn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2aburbqbz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vhnxfzaq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nzsvjmlk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fvnefvcx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oijsnqyl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fszwmqmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rcxgvhvu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kuaxacmi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hhfqhigl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2guwwvcqk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mpdahbgt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2cbqugszc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ydcjmtxd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wagaqvcy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubvierrm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pgwwgbwz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gyswbofp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lajwmlig.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cjezutgx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lmrjkiab.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hpfkdoih.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kbhpgvmi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2myhvdmko.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ezvpymef.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mtuagssp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ozxmqhuz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zpwtdjdd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2nayrwckh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qpnbwqbt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxynaups.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cmovzeeq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2svaxrljn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2etwfacfi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tkxytvzj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2dygxqino.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wzpdmvgv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2xicsoryz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qtetphds.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hutogwil.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2krtwnbmt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2noasvfbc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2szckhfcr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iecmzknt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mjxscrvk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2leqdjhro.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ecwnafvs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yyouubob.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uxlwasut.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xukwqkml.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bwliysok.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rxzviqfn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2slbfthin.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tfljbnjr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sjecnili.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qbmpdcnk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2stdubjsk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hgcmsdsy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dqdiktwx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gupjzwbu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ynysehex.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2figypzlr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2svgmmxxe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vrbmgthd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kxiurewk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hvzntgpu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vdjkbajl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ghhkjzdo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qepupbhy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ytsuwjig.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qnzppadu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zjyghgsh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vgvltkbx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dcuhhkly.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ipcptsts.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2piwxlezi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qpjjqcwh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2remkxvwh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hdqphlml.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjlsdogn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2assahlki.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pzscudhy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xvleygyg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2brnljtve.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xjqeafsw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ypbypatw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tfabdryx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ixynuigy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qqgcgeyd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2beudjspb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kuowmpfw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jeeyovdt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fylzheav.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ummcfpsp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2sqziszpl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rpugqqyd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2eybwgady.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2abglshfx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uaflcbav.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dsbcaqxj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qletfrlv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zkmnpwim.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kztqluja.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ymjvtukj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fyafkjyy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2izutxcnb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mpyuioue.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hwuesqli.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tljjukyl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hstrxluh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zkoepkkr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzjfeobp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ndzcesxk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dsadtses.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2goohkkpb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bmfqdgwh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tvjeuqtn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2szwkevjs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vautnlne.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kouywncq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2yviqcqch.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hrxhshic.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2avjofurj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sjwjrryc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2pgskfvup.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jykbnvkf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ivnqnwez.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qwxsceii.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwyisvir.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mfdztfys.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2arwlzcyt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2npbkmsyq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kngmqcdo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mtkcjsqc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tlmvgdjv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cgrpksux.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvykbjao.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2azsdmixm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hipivqhj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xvqyweky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cfjzyawu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2roobxakv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uphqtfqw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2viafhzgz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lajplcsq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ciupuwpt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2axnlhmsr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bmgiqcpj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yptqeaxn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rzopdjmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aakfqsbf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wbuwutcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffrgzimk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wyivhibz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gilkihdd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fqlkahrh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2igsfwxzp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kgzkxite.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rirctszu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2szpaxnxe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2chzqnvxp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tdwmxesc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qhieecbt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rmuwajvw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eywuumjx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdafvrtn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxzzoyyh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oxgrmnzt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nuumvxrf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jcoqsula.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fukdpofj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tsvkbvqq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cctkyzvk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2juizrmqp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2amyiuzqq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pkolvioi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2swzbxslx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ywidzjje.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sdhocdqn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2imyqktrx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iragwcgn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwmyqeqs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cfriwhfs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qafbyyth.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ljsqwvtk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dojlqeyw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oaykbqpy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hdlywrsh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2cfzipnit.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ioiiskqa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mvtqnkox.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ikixlxlc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dlkrixuy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtataguy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2swqzjbcz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xebmmpme.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xmkevezs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2udbpkwjk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2obkwoxdh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2oeacbwrj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ezdlkcya.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ekvslfjl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hnsivrya.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pbyijgvn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2udkbskxt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pgdzbput.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2yasjfniv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qepqpovp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2azuobygu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vblirzhv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jalpgvuk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kcjwrimw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2necnfkvj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lybatbxy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fwkxcbhr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2htffqblw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ugyzaxcx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mafyptxx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2bxjkxpmy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezspdmgz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2clikynjs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ahemffwt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pnsshxgm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gwmtkcxb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xhrolqrd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2juxghatg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2brajrbyt.html


<!-- 参考信息 -->