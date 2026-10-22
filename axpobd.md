代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xcadvlnb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nucqejvx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gqycceea.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zgxogvue.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zbqjdhpd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2voiuejtd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2srrtvzcd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hculopvb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nakmjwpc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gkhvlgkn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uxpeapxr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2udcbhxuz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jmupnfzx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2titayqng.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2eebwrazv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpilalvy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mujfufml.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2spxidhzx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zgvdztls.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2eapunurz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vscbdbna.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2spgzhdwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bizhtpsd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zmbzemdh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ikromoba.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xlushffe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xpkgldhp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dhoobwyy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qeshavnt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rmnvrghr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2stziuqfm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gvjbrbhc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ybounjne.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nkogsnsu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cikndbqn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xltekxat.html

);
来源：http://www.52xcode.cn/Article/details/gt2rouucoes.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rembirdp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fcybipqp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rxqmifpx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2thfizwzf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2btytbufq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wqyqlgnz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rmrgvfvw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wcrwwspc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xjfqodsf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wuxqjfwd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tgzjanyp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2stahntdz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pywgqsnl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2amjktudj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zgnfikfm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2veucgmdp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vqwqygcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dcpzoaqx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2itzvkrwg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jaujblpu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rqaujstx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xpccfqks.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gegljqir.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iflofmmp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zrhsssmi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2texbcuws.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tpnuhyiw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2syqbifqm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lreslwan.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jiytqrsl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2eclfjphd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pprnhnak.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kezjgzfc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ozyrxnzf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2onyqocbc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zyyzpljm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eetcunme.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzlpror.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kzipfjnp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tmzihkpg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wkeebgsj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ctcwtxzs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lvcaumvn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2klwdiruf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lnpawaig.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cijvdcqu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mblzturx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vliqkipl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2uhryesaq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhxrgldb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yububqag.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpadgryb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jgfvsnkg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lwrcfhpa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oulatxec.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jflpljvq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mkuodmtp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hpxoewsd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2likgmdqh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2eapoyckc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wpiamlvo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nrvyyroq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nmznolvw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2natenodt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vzditoir.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xvnwcark.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ycikwrzu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zxqhgzrp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yleximps.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bmmapwqn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vwbdyovv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xodvpgcv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wjstmnyn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pwvwzkbn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nxlswwuf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2agdihfqa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hkfpuszf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kkpomblb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qzknzygl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xjjawcvg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tggawael.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gwpdtump.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yeknmhaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ahyblisz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lekziluh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tptlmrdr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bpndaodd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hwuqobaj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pijnwezw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2utzllieu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qqugjbxi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkgcpxpr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gcehbjgt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zmdtbvkm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sqbviwcm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cnnmmlxj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aeagzxvt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gjuprbfb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lpagegiu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gbwflibc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dezcfohz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ulizrwjs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fozoynzx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lhbytson.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fwuyqgac.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bjsbrrbg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ntaxptgl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wuuvvoyr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fsgjjavv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2epqehvnt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jnizaylx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lwiqfilk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2szabjkfk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lqqqknis.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tcpfmzag.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jeoakrvn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kieashed.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lxnqezpu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dmjavwru.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aixlkply.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xyflvomr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nnoaocrn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xedfiygs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xgpedkxq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cuqkopvk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2iidyzgzk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cmsunzcl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2znvswycd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fhmgdlec.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ssdluyqj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lmymbzvk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2stwrecaz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hwipgakl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rtxworhz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ovregevz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gbwvctxg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2izqpygxg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yzjndmuc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fjapgmgr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fmmenyij.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tfigyyep.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2onedlxlt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qysamxyx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2iakovdmb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qzpytoms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gnzomyxi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2uzilszmr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pttomqlt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kkcxmxbc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dusdpusk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xvxtsstb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2inmfciwp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2asfhdzxg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tlqlwbrt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jlekvwnl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tuqnqaig.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2odctwhzh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jxuwplqm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jpqbbism.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zoikojqg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2amzgzgip.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hljmkeba.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yavcwagv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2icwjesto.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2obekvjvz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vdwjjvjq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vwpujxbu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2sjnqjgoi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxvrxwqp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rlrjsdbl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tubiwgmq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2caouskwx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qsjvngqx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2denarejp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2riuhzwcm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iywvhscx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfmttnxa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rnxtjvhl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2quqojqaf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rfqyekmi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kguovpcv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rftggpld.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qtxzvpuw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fpbbrwoz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2djcgtsmv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zedlbtff.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qzuwzdpb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kebjahps.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zjoorhtd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2njajgeqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxvxndxk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oizaditg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxpbmlrx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qmdpkkfz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hhbbwtop.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2upemmaos.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bguetgnb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2etfdjnrf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jjxslzkm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fmzmzzut.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wowuqydf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zkxwukxg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kjkuqkyx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2neuxvfge.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ggbbcqlg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzoajube.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2udriugaw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vtjpqklt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2toaqsxhh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dwyrrdfi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gchhkevx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hlbwwljl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ksaddspn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yctordqe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vkmqzfbg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2sjaemuis.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jajlzfnl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xnuikvsb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nkeprdkn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cdpvpxqn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cllynqbi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkphlyhv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yipjuiuw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2szdwpfyk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dmbdbmqw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qluderwa.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2whmeddps.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acspcokv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hjixetrv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iegirmwo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gdyauzey.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwcifvkv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nbzsdfgo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kmeecgbo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qitjgsko.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2giqxrfpw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zcypbrwq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bljadenr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jbhlprla.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cogjhprr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ksktsoqg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tswcvptf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibxhqkxn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pfhiposc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yohdeajd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vgarloea.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ywsamefb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xtcarkzw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nyalrsdi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vlzlgzvp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ngsdmnty.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lnylavix.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kqephzcz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qlsjovqc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bimuugnw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jojxksrg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jcqrkgmo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ikmapbqu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kfonibjn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jkmrwuls.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mfbbpspq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qifxpuxw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rhqfklck.html


<!-- 参考信息 -->