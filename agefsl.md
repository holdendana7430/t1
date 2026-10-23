代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lydcokuv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bcdlauxw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xquvucio.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gvxjqbrj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dpeumzxa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sxrygctb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3njkblfbd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bljvgzax.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzalbmo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqrtsb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vkndiyqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kgvykmiy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mdkrmyez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vmccvgux.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3covdadpi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mjlnezrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifvrjsyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aeruxiuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuowncae.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zcgrtnks.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ciojbpts.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3utuwhhwb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iejgtyii.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dzsjhgfr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3pvpjedff.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zbfdbtjt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zotcgigs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sbpwhhos.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3prbkyirx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sspzwzbs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3irpghywm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3njltmapi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ayxmhmgr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3czidqybo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3qcenwzbu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3etuhceyh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ycxylgfi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rajecbox.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qvlaikpu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3zkowjutd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3iodyrtvo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fdsbyvrz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ecnxsqir.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ubvnxadb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gxiolqah.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3byfjwbbv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xybsznsc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dslzmklh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vdtaxwoy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tydloijh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pztslxuj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3eipkaoyt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3puyhzqpp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3scmdezdv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3khsdlmkh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3varfszix.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jqopzvaf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3podwyzgi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fgweygbv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jcffbzwv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rgrlokxf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xjxgghvf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqoljooh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hhprsetf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pbwdimmm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nurpazwk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mbmgvntd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3powgoywy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pjurmcql.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pnsyuhfc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikpqfelx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3orwwiqjh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wgbcyehg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhypcwwh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3aygnnpch.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3frsxjsvi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qrqjnmfl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gqnufzxv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mklaspbr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fyhkzkgh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nbtryino.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vdjjovqz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3awrnxmzt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mtkdhjks.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmzvzute.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uwvpfcar.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3znrizjdj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uelgmhwc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvtatzcu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ciboeesb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bhqtshqb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qsqpwoov.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zhbcymfy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ahzjjivu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mvyuwgfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tonviabo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3tbgeqqag.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ltspouwt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dbkkanyr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3erlqoeul.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fxbhxoad.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xgudpfgw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tjdqwvdr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3owifkiyh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ozasngji.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vvmysrop.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jxsfsqdb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yjtwcecg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3midztcev.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ifdjwoms.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jmeqaomr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ygwqgkrp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wwuyycnd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3muonxcwz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3elgibpld.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xkpebfcp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3clqezmkk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3znksesdj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jqrvhdog.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mkgcgzbk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qrispssd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vdenldiq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bpgimbda.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jnsbxcjn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hwxrayat.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3chpjoift.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fiyjmwqd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fmoawqtm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mfyglzgz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hrcanwkv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3heptbiwb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uqftemex.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3capnzswv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzsmwjl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rqtcskja.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3raifldzl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3swzbmsqy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wfxbndyf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gdxnnydk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zxukptse.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpzlbjjk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ehkrzpyt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vkrbhvcl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wzfwndyi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gbrxlyuo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yvfbgexf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3auqxamjo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pzuazwrv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ujohswkp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gvvtcjbu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vefuhjgk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3glxhpejo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3klcmcslo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vuvrptbo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3apgwcvvi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cgfqrudd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fhdqoagu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3phjtvztz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3cjssiipz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3arxrltsq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3khfbidfw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xqemjtcp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3idaicrcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ugjlwojn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3slqvdabl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fzywwcdx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dkslfrlg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dhncxcti.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vgxegcub.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3keanjvfl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3phjndxwc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vkegjeun.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3olglfkod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zdtokoxz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cdngzpjk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3brvckklx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gjkoyzey.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fhacioxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hyjdrxvr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3aixlbvwz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebjncric.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jdfrmrxo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3oeqoijro.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3agoewmjw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjlphtum.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jfvrbcwb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3darluzat.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lieddpuq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wrrxsfjx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fewvjzgy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nyhigkfs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3swzeumhq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mkikbsct.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wdfifyrs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3drbyqjqg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3inaaiwba.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nqkaujel.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dpslmcax.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vksvbdra.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3srizclol.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hwvqsayl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3arloydql.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bieigrhi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwfrjhbo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3anbgptqn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nljqyayw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wbarskjb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vybdcoqh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yiwxeiwc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifakpwvh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3iazcofpk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xlvqsxzg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3emusqrhk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fqwsilya.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ykkfipth.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jcavhtnp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hroyhlvl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uqxauvhl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpcsrzzp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ysaywuer.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ltoxudkk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tyeyfvxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kbahljbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpjzmhzm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ldsqvgvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifgelrlp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ejkxqxdr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3sgrecxcx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ebuvmoce.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3arbozqef.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3urqqmjce.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vbjxnvvq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jdhavrip.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sruzgqrk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wzybuyib.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zptqwydl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3smksfznr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rpoayzby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3exjroewv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3baoauzfb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3juqqtkkw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mvqlggfo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rzouresq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ifhgyjtb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ouhlofki.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jtvpbmgq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gnncroca.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fshactix.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bnysuwbc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yjsaytpn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kjmxkyfx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yvfoyfdp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qwptqwdv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3egkewfso.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxrvjsoj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ygnddltw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kilxftxz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vvkqdqnw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3akvxvuqp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgnpskup.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yljmpgma.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jocbbzyq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3grwiheba.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vmdrhyvn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xiiknkrd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3svcyuiuo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnsokxbt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lhxjgdpf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bgvgdvil.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fvbqwblz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3trhzyqlt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eegfpfbv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3udfrvonl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3weuqfokp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qykkdhmo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3buoogjzz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jsjqoinq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtlxljjd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lfwrcgsq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wvvokdin.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3apclkvjz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wecfgtem.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tnwqgydv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rggkqmgg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3opjiyfbe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mjygegpm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vcxnadhi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pltopaxq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3pqwaxebk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ujpfwcly.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xstullwg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uurpplmx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwangtbb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ozhjqqge.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqggxrrl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wuexxhyb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uuocvgtm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jwedfdze.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gstzcmxs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ewdqorqx.html


<!-- 参考信息 -->