代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ctmyyzmr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tkctdgpr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hdbsmhqa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3abffzrti.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bznugflq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ytnhygbp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qvdjlxgr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jncdfdzm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xftjrcnt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rhmusrpz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3pqjdbcoe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yvrahmqa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jyhhctrb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kabbirjr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qcvruszl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3giipshwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzplnusc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3phlxjtmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efrwlxvh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kkrnmgst.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3znylzdjn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jrntlhnk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dqjxijgh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yugmzups.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3pybpwglc.html

);
来源：http://www.52xcode.cn/Article/details/gt3ytwbalan.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hviwzcwt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xeqzphuw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nwdirwkg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dzvwtizr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cyxzgvfk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ivjhvcgx.html

);
来源：http://www.52xcode.cn/Article/details/gt3yxbvgwfg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ibhukzxs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3znsxjhlc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ubxtwqwu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jnmbddzw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dgcybjwg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ehpvnouy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xedryhzz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3egezwpqu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ygsgguhp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ndvzjvrs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bdvaogkq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jhevjdns.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qkxsvtfk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jvlkqets.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ichnlzho.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ignxrmft.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3bsmoffws.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vsjgxkam.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qqngyrsn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3socfsixd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uvnuewrl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ryhhhjgd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nytpvwij.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3shopaiie.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ouitsbti.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ubyjpsvm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qdkrvcbs.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tamfredo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oozwcrxo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vkidcftt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3btnckbfm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ejptzanp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fhdfzumx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fwmykrhx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ajyjuznl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3druohqjk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eebuqnrm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xjqfricl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rxqtbbyz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nmclapap.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pndwtbqo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ifehfmis.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kuamrzgt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gsgxgwtg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zlzcknhd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvzfdvlt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3drlfdmjk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3juynnxnl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3pwkbwidi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jfnjrxok.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jggcydsh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ouvmznqt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sufsjzhx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fnytyqxp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lbtndfhm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbiaofos.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sstogiyj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dndicujn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bzzmmlzp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ruvdikcq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cvwplrwu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qcbzawda.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gbjhmcwq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3amnpassg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3buntsdqu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3edxjxury.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3clyvtlih.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tyhtelgh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hsnhzxik.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ryvlxeyd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hfqaawhb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nhfnieoj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3verfyrha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3swocoumy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bbzvwdxc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rsawlvvs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xiaaemxs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zjczmiyt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uydlydvw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3irzdrwyv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hzmjymas.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jxfpwaum.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bxwvdhpo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3iozxrnmm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gbvgxjst.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fhwngzvq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lqklpfeh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xazzntyf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jygokuaw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3csbwaxju.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3icjrlkre.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xgupnqbn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3frmvclgl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qdvvfzho.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mjyrrzay.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dtcczovm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3moaflrvr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dmbofoum.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wqixqrgh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jdalndox.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tvkbjhrt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pzrdjfii.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3oqioqtuy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lumdqgqv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3smqnkrwm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yxveugnf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3rjxhcczf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ywgqnsqb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xvyvntrc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ixuvhvkb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xprtbmhj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lensjhdo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3oxusrlad.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dmjtogfm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vptjphur.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jvprgbtk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yppmbrhj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3phpnnfgv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3apemtutj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hnvvcgal.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zitufeju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ubvgkaon.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3afqyzida.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pflmdeaa.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kckbfqmx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dnjuwyvg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mpszekuj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ifldwvte.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgewxhid.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jjqaujhn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kanzqnqi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dbikurzf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3npcepbed.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xvepjblc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ufywidqc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mjbqmtal.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xnwpwlyr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3aiyctyot.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yhsyfxdv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ixpvzgcw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xbtudmhg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rbpyyogn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kvvaxukd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nmdbubiz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vbyttgpw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqaagi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xittwlun.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qzhubexj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3icohvehc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nktutfcb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ochundmg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocnyjknm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jouimogz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pbnbwkml.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3akdvguts.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3txkybehu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gsccjsdp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3skkysqgh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kzypdhzv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3igdxkaua.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3edbntpnp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xwyzltgp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vpyfwpqn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fziuthwb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vciaxnlv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rnjxvdis.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xfjynkte.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3anxlaugq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqzxjxna.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pmpwkpui.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hltzwuwp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3arrnagsp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnpugjve.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sdoucpbq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtpbtiki.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3iatahhxm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xmdvegnu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nctuvryr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3koiranqt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3omlpynfs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uxjwsuah.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bfzsmgan.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cgbznhnq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wxbywjdh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3irohcjez.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itfzhzrf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ugtvcdbi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hxoowirx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uoepcugz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uyqcxsxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cctmjlgx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3isvcllqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbvmptis.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tuncjdeg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ygefpppg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nvxiqqvx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3amtqkmmk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vbqibkwk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxxithcb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3phgsdakv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrtxiwzx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3drzhcffp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mggvnrhn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjmerice.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3egcybnqq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lrhqgbhk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwnkyxfp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ajtpmyik.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ywitrcfd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fqensjvo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sitezfkh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ythgihks.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fxpmnwwn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qifgjfnn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jmssinoy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dvstsggh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3udiuapcs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mkfnbvhj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cjwbwgvt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ldygvmmg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkkupgjg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vugyodlb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxyxidcq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3upbpiwjo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ecphgwkw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hjhxhygz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xffegxbs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bcnczfuq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mbflwhfk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rryoqknk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vhennuar.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vavodabd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fuvllirr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gpmfnyka.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jeyshucx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gellhrxf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xtbildnm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ghxeyaba.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3alhwjwiz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zrvrdljo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tfyrejaq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bvcjzvos.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejgcqdar.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3sukrcylg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hwbxeyli.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tpfmwshh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ksniwpso.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vjpvmpdr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3irqvtdax.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wkdlmssu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jmsbkwfm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gepfvamj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rxmxrpea.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fpsaighw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zpzdubdd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3imtbhiex.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xcjdhwxz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zgrvfgkl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3apcmqtzb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kuytqetk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lfrsxugu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ekqvsdjh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3atvdtfgy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3iknzrqzf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iilmqmiu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3edfohuxq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wnrcreqs.html


<!-- 参考信息 -->