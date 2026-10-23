代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3akqyfxdq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jzrhudvf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3emyagduu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fzvqadxn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ogooohkv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3sjgbticn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3epcsgppb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xvavsxav.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mjhefmpv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dxmrwujw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mbsprzgt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jekgngsz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mskgzfqc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qozoatqd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cronweba.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gfortnkt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tqudmfbz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hcudjpeg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3entsiexo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mykkcbnm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3onktlihu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dmiexdjw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3piwxyrfi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ogxyoyuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aijjcrkv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mtcrnhsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnfdqijj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jcbpjftv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hgplhhfp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3poyrpnwj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3heeqyqle.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3prmtkcur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3inktmnxa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ptuhovif.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dftuapmd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3krhfzikw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xcixweti.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qxbepzyk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3bdxbtcek.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3emowponv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zovbjlgn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gemqtkbo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ecpbtppz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fvsdjovh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3refcbgei.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3slglkqri.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nykadzkj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3umijwtsi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bnpwiwif.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qbimwjdq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ndcvtppx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rnkkmcoa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ssihpwvp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wubwvdak.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wqboeuki.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qwstsyfe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3thkrahqg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xejtqxeq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xuqgezbk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cpvdardu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3heqpoxnr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3czoxagii.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3gbpfrhyg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3phkvtczy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fxrhttoe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qcoybqor.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3azpmwrtg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mnkepeiv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3waudzski.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3glrllzbj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3voihveka.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bioojvsp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3nycvadxe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3joimrrbd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mfaadhrh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dpukqcqb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ijxqogfi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ymwvkrof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpaqlicq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fgjozdrm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vkdxokjv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bigwuqyb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3czmevqdq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zrqhisij.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ecaeevmq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nyysvcyg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fnejucxt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rrbtocpc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cbmsvamv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mlxjopul.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvhmalhc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ufiolblc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3skjkonde.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bqkuyher.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qancgcnk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3turvvsym.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ypfmxnzz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qgyrlhfk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tclbxlyx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mcvpzqro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bdjfzgtj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3evxyangx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rcycebxw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3crqbrjwu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3doxeitpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kumgjdif.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nlggemrp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3oxphjwwi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gqgzvccj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfbhjurs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ahooyeni.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xaigjlhs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3buhmpwqm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cducceoo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lhsmrdhy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3krphxkco.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nuzqugje.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zyzjjsqt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3uhkrlqls.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zieyuaaf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vhgttemo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qwsynjwd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3txsseigg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rrjeutyl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pwciqfcf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ikyavaya.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uqyhctcp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rsrigwvr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bzubuorn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ucoejuqi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gdqljkuh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ccradvjd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ubyqqwax.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ypplkoow.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pvkaqroo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wgodvyvf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wytzdcum.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fchyjihh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3tkwkvkym.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jjivmiyg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3phvpzdsg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mvwuzoem.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wbhacagl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nmahcmza.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ukdmunca.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ausshmxh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mlqgqqam.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pqvsprtc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cadjwigr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pkogtsdd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sjlhisju.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ginzbkqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tmxcqlsv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nvimkagp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hmtqvclc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vjqdrjvu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3edqrwwyq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3efunctgb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tzmhtvxb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3znncludp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uvsvnerz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3snsnpzzk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wstncsij.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ssqsjknk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uvseghkr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ljwrhqpf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jeyppgaq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bvvgtnlk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3iuziohix.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jntomwdl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jsvvptxi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bsptsrow.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jpqhcfcg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qvgmbzuh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vjbamdhk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3igntvkhj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pkfrbybq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bdvccvms.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3pnmdkxvu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3holyidkx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mfiwmvqi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lmszaquv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3lziyozhv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3uxgggciq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qqxuuvvu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3oohpsain.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nnecndch.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ckkthiln.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ismgmmjz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ohuvfyyi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nriiqhfl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gpmodpmo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrahvhzw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nisavbcr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xmvcgcmv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3doyvgslw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zwlrneyu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ssjqneve.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kezvjhyr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rhpfcgvi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dzikwuot.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xpjmcvtd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3neaxyqcb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3venlvbya.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dmhvfges.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3msivtcau.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mbhymmxo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nglomvgc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ecdwccfe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmbmcsof.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvnjohlb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqzrthol.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3glcfejhy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nluleghn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sgdvfdyk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yykeygfg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3auwshmep.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lluqykiq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ermqtzak.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cmdsdfvt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3eknuwcvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vytfqaii.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ujyzmbxw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wooejpov.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mzctzvrm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3oeamtvrj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivrnkiuh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tcwvxhat.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lqnfrmww.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xybthunj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3edoiirkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oinnggrh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dfufkagp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foguftja.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iorhdbzm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tnmmqmpz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xdtysdsi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tqlijezv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3amvljmix.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xdztgufl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qrredsvv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xzmsynjn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jlljxgmk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3txxomtyy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xhoqwmcy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pptbbvey.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzcbgpxe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fsfwihnb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3prfxhbbw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mkykqjgy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lpqdxawa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnjvoxfr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kerknxgw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pspfpizg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pzqomttu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qkrobrqz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3lgidgtsu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wsriinjx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kspzrofi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hjhafdog.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uaikyuek.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xsiwjvzt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ycardjfd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrjyezdn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3liiltwba.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3noairvxo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfbspios.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uuwgmzuj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3unblcluh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3meuwosdi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cpwdngfp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iicbdprx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3voltankf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lnzhveea.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dabwspyi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfemurkq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vlaimijp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gupuykhz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ziyksrlt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mxdzvyaz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylxhgaba.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ukhsywrx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vqmrphya.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wtcwbccf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uugeodgi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3snzputmq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3yfmncabu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mkssdrnj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cmriygmg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wdkvjybg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bcwevarj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jvwldhqv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3npqreqtw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3upygqhjt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cjzmfkos.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rfefqkfo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihfzqmya.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3flftmllk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ipogkiuo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zxqjonjw.html


<!-- 参考信息 -->