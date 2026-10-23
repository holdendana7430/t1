代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uspsoaiy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kubjtjva.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3okkkkhea.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mazjwbce.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bwcikgpc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3krkrqvym.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lwdvxnip.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vtjkaetq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3htarzzoz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3thdwzvec.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3xfmulfri.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqshnlr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ulzbexoz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ewjqrrtt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3fdubbaht.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3liqyclzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omsfmgyq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hiwqhick.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxggahka.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3usylzcnk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bdhfzubr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ffggwnri.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fofcpiwx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3smknogdb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dwbvjofb.html

);
来源：http://www.52xcode.cn/Article/details/gt3ljztdmun.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zewtdczr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vfvoweqv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ppfirdgv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jguwbphc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yutbvtmm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vojqekrq.html

);
来源：http://www.52xcode.cn/Article/details/gt3coalcbuc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vogcvusw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3htwwwmzv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vagpoaqh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3abmmdrrx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gzjtxroi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ijhvmhup.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3genwfdkk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jrjovryu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hvngjcyn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pxfxyqea.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3buqkrcpx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vsnddvvq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3iuvxyiue.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rsymgdnx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rdlwxdfv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jdceftnz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nnudzobf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3glvgzsox.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jzqisrgl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3yrejciao.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rbvisufz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3oejuziur.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kgzcmigp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kkwwwupn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fsehphcd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3uzcxeaes.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vilpjtkj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wtfwomvc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3oyesukho.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bylrsiwc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3keavccwl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ugwibnqu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jlzlweip.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nzgxusph.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3edzenoue.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3coskgfyt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yrnxiqxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qmzuafer.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mttvsdgd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vjlidnpx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gnvsvkye.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ylpcxduk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ruhwvnre.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dsykyvgc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yjoersye.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqlgsqxm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gjugxhxw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kulkavlk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tzqevzbo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfgzcure.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vxsrpafm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ashderbx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kaywywpa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rybznbjk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uxzlizvl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oefehfpl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjopyc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kixptsds.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqdhyyvg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lbkvhvky.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jgdlpcpx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3auehyizq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nyazzwio.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fikmaubz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mvfazgnp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bfbwpvxx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vwuhbvuz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3oykwpdeu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rxefroil.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lpjnbojz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3snynxctf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yfbngpae.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nktyerkx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pqhchppn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hrgnavfc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jsxdacyy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zxpsftdv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mjlghzmz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wuedecni.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dmynigmr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rwdgtcoi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qxxtnrie.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uzapjeyy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xkbnqnup.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lhyphejw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tykwnsxt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rombpftu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ctjglhrd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3otjduztu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hsvzhnia.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vvpxmsqt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vudztitm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kuviozdl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jamkksys.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3onuluajp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lqydyoha.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nybwpghc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wxxpslli.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3trhzuucl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oyrvnvta.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3bfsrobuf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3svhkbhtm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ctaxzdpo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3afucfkzh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3frcdvpma.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fntqitef.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3oggwomkj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfoqvbfq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3topaauuq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qzbsqlwe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gqeaciak.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rdskshgl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hqwzojsr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jbbxedrz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lunanyhm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sdhncfvs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iedyhdid.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qbkvesmw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3augscdtz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sewyfvoe.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hiohkrja.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fnoqazvj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ecclxxda.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3enyepgpf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3koogurzo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tpyoirtr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cfhlzsnj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3stkqpcye.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ehufllzv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hiybjhvi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rvokyytd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fofkutlv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mmltjzaf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3axcedxro.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qhzoqaqf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fnylyome.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qfniemth.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vpugnmwi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gzmpsskg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3egyewnhy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3snznjlyo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3elzvjaeo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qahzilzc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lmwanfux.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kfuhbkuy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3edinqyvq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3htohqoaj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fomurkhi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3aaoamitw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3prpesibn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3crfxzdnt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tnphcfif.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mzeevnig.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xnaiouvj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3cvlfocqn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yzhovlig.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lxwtsvwu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hufrehcc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ytwospue.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mlesizzn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xsqupkur.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ndjchbki.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3touwnmwm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bevpcszz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zldhhbgn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nimlmxqe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ltiuyfix.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3zjuwpsnb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kjhzipbr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3aytnileg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dyxgemlk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zkczejvi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jodfuaju.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3giekqhwr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tusdrknl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cdeamyzr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfirvtiv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3aywsnybm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxdjwrz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3riyxcmat.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kgvopgdg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3swjnyyjm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bsqjijpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xmcilrei.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vtlsptll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chojccoz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dqqafgvz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zsokmhju.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cjgqgajz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vbdywfag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyaachuo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qpoumdbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahtwwjtz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rlzfcryv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zkzwxnyj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rytkzmjo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ydpcobhi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3szaoiynp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dximcsnc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3csknzhpe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3djvvmljy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gyqbhjhf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vjooenbi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3msvlmwln.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3owylahrt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kvhxefuw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3epokyxji.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3szaqlggz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ebxkizpi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ygsbmynb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tggvnhjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wmqfltsv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ekuhwelt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3giwwraim.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ywoqirwn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cdjmmlcf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gfoxsbva.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pihpleof.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3obpudjdz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3afktmuuw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ktjhrgym.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mkuvnzxj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iiicuozb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eexhvjlr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ajbigsoc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nytdarzp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nbenpdhw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3aajoeqdh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wnvhhfka.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ngakqqgn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fqznrdin.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zwcnzynd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3sugujhyi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pgqwsixf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jiofqipv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rldyazmu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ifycpgxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjopzurt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sncwyiya.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mnbzauuo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zgxkxdwg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjuysakr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qmuxuqws.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ajpdpawi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jkbcnosq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aynifukg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xwzquxyr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nnjwihxb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fczfmcwq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3boxdkfpn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uccjqgzb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dfpchoiz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bszlfkqu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kgqduvlz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3srrfmnxw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ioxsycza.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ylwzlrbg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qqlyafdt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lpyfuwpk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xqksmitq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3eycfzuzq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3afufembu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ydprqqvs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kkncmptb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3emomnzwt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jqbvwcgf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zqrxnsee.html


<!-- 参考信息 -->