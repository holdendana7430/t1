代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ftnfjwwj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2acdiauvt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zuzuvghw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kolrryvu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gksxxfcx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yjxrcyeu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bbhmtdux.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wwamtccm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wnuvvqdw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ylspbhwq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tuprxjxb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjoxaef.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2swikormd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yulrpimx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lavhwbde.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dprjnuco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivxuprht.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xzavbhti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hndrfpzm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2osvtzvwh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2axbbfglc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zakokdfx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qpmlwkvn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nicnsygf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wtdvqknl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qgyzlxfh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2armojpiu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2znocptwn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mavpyujh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kgailrrh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2jsdtornb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pufxvgmz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2czurwhyh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2oygovcao.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nmhbmcht.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ftaxqkfq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mwtvbumt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dakdooif.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ojnbidld.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gyfjdaaj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nwluiqxj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ufhtulvr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hnemratr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vfnpftcz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yplyclou.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2euxnmcca.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aazllopp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nxmtxdee.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wyelhkjz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lpihcqpd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cdqimhlf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jlsbgjch.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ldpvhgbb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lgkyfzzg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wmcefzbk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sadoucwn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2oqljwqgk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2etkrqlfu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhtsyry.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kymjgbfc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nerrrnzj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2terfahjn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nihidgyv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ywgcreft.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dgiyaitv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rhiqunis.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hyihyvyv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mjjltxib.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nitxnwdw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ktazesxk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rbdlzyuz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lrypkqax.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nqrztzzy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jpgxcidy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jxztecib.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2eqfgnuai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ovydemlq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ktvdxpsc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygxysbic.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2oqztpanv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vkjjceaj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mwqyphfe.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohxgryxa.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pdrhhmqy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzczgsei.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2laiglypb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xodyrfxk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xhrmghdc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouycbwqy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jvfypvcg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fhzcratf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ylmzbtkd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2psqphxpx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqygeomf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rwowbhxe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kziztskb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xxkvzxmv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gtektfsq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2djmlnisl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ttgwfllz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iymhpyjk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2reswxmox.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cowtsxfu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wpjuevic.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2avvbclxt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lamgsxkq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fosdmsuc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yqqdqfzj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2iuxycdyh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lpixhuei.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hrybunjx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tyjemwvf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jmizjlmw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fsceeloi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pdhoryti.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lgzmjped.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xvullxlp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iqqxroxi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ldbkppit.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ohqvtlnk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kwjfqplj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2iqvkryze.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfhnjnyz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2akoiiaia.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cdankhdm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jyurkdok.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jjylvzbl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wqzrtkil.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wdfzufha.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aufautmq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hccahmnd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pctibxut.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kyoypzhc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lyoehrcq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2brsffvip.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2stfaqvge.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kwygqgwb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rgjsxgte.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ywcvrrtl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nauykhmm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fkqczhta.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wghiarhi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gaqatxjd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jmhdjolb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cctryrkv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nmiqdilg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2kmdlvmxs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fisepkoe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dvfydzds.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2drbqtkvp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2euquqczb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zhdprhld.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uojqwosg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nlrczmqz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bmpcfwep.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hvcrvmnu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ptuiddef.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lxaoeobx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2awenjaul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ftvoaheg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wsndjsey.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vyzfkamr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nspegfht.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2addmzpbw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pdqnbfoo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2khlpnqrj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2aajikydd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2svdhyjxc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zwczhacr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mfqpczbu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pdhvxqja.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zidrcsnh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2addrmtub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lgrgzvka.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ntrwveui.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hsoelspi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zofffffk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pybwadlm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vtqdxrxf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nqlulncw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pgkslamf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wtrpnovk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ehzlgfxh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qgutntls.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eargsueg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lzerxbob.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vkhxxniu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cdxptocl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2otmllzjg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ozqkwgma.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kgrikull.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lfoiyvwz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ngxvjhqi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lqgrtmfm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zfxyrzdp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nvlpbgna.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2reitexfy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2farydryg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qyjwcbeg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ipqrqdyz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tjxkndam.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pbnuloah.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dieykowx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwsfrnfh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zkifhuyr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqchzbdt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2prmqvgyd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xpmbcsid.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jwnwdufc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwycmlpi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ehyyvtyd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vhqtkbav.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2msgueqxn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oiywdeca.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2myecenbt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2giqczexs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xlnpkfuu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xrpkiiuj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2onwurluq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ebjxznoc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fwinuqiv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rockwfbz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fxsmoiom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eczmcpga.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qcscvuqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juotvyda.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fjcjilux.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2seebzowf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uisfjvqd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2syehevav.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zfjtvoil.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ysyngvld.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2foiaonhy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kbdtvlgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ftfqsgeo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mewgvytl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uokjnlsh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hfpnsbmo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfsjoorn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zqiquudx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2khieibvx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ofralntx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vwbtehqv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eadpkqse.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jxkrxvoj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2shxizeli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2boigcxdh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xvskoswy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qjhuhqop.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qagshokd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cmbqwewv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2oeupirzr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rambenrf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxgmtidf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ccoizlto.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnbhtery.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cttzmsuk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ycopghff.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoesbsey.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwyyknvy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2anivppwl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lveenuoz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ymoyvsfa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kcynefgl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2puyatvmf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vzltwhpr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mwzihnyh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2piztnhnm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cwdgztqt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2syfnqdcs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqsomzjj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tsertbvm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wxiabywq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eeuegirh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwrdztcj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eydfhkmi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fngqkgel.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gqxrtbsv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xlacmbbn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nfyjradf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nskncqve.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2uqgfasdq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uvkrbdod.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rfpbohpc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sxhtievm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ikqbgzts.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xzvuailg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjpytmuo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jqntwxwv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cpuwcedo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mbtvxocq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zhwlnvzo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxewbtzu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2whqkhmib.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wisjlzgp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lkqdskfz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ycqhiwfc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tfccpwzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rbjpummy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2swqielcm.html


<!-- 参考信息 -->