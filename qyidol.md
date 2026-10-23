代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3frmndvxh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kofcekhb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hcvlxrpe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jstnxxjn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3omdcyaak.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkyttdbs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3elgrkhmy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ednvcmxd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jxhbqitd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ygdhvjkt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wjelvhce.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmxwgie.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3itjlniie.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3xulelzca.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ohtpehke.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eanewgex.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cqbvumev.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kqvlxkak.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dpnlyvfy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckekuzts.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3uvspenov.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3buggkxqc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yyegvptj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zbuserrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdgkhacm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wmhpmsmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvxmwago.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3siuutfjj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qxbaftbd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mjvgsytl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jglcolzu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3twvqruui.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ebisjwze.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hqbwhgya.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kgpwkfws.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fgffolrs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tilupnxg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3etvduuuj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yjiygera.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xfwzeoke.html

);
来源：http://www.52xcode.cn/Article/details/gt3kpzsqqir.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ixchpydy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jxjvenos.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rahspfkj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xgjjoxxg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rkvufzoh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3zlmdyzue.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fkrakywc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3eekmszsm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wvveolyr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dsdqbkwn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vfbjcrvw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yrsngtps.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nteauaxc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gutkpqla.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3geueeimx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3raqgocec.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rowjoakj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ssvfdmdv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kytuyqkd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wgfbxmgl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3twwvuwhy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tllufavx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qieqbllr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ulklfgqx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3whmjosxd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nnbgjsps.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3caqibwsg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzbbfofi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3srquzyfs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxmniztw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gaztohpm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fzmhlbww.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3otqzuaaz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nlezeppg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nkrnlhpx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kitbrxwi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3accuswyq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hlawnhnt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zduogvgz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cygxztty.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3nhrsuszo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3taprnuui.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xijmohqt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ofurduox.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rjecueij.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ikhznykn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qdywqpvk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ltokkeoi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xmromfsw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hemyzrjd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3djbvgfji.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqwqliox.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lqrgzqcr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3khxzdpul.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mvarbkox.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fulbpjrv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ghcuqsdd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zjympiim.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tdzqfenp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bbfeidzr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsqrghag.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bhaspklx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zbpdnaag.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3awmyblbt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3uppntqke.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3soqsfnrx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3eghqinwj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3znertjio.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kimtyamn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmlvphgq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kvvmlyjm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lciyszyo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tzoickrd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3alicshgl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3njtkholx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pndhntwr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vlxqffeu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ieznczxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rytcqgfj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xkhpbvrm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pbnzpgac.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3muqqvrnq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xplviwoc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wadyrtju.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hwlkgloy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3osciqsim.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tasrhsli.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3iochozgq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3udxdjajh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oepiguoi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bbbmzuhx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vzacdodj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tnatjcxb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wqhzwydi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mhmhmato.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wxvcfbbj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lxpmoast.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dtczgmxc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3izelngeh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3smphxjxy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qhphrtzy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sdnsmmhn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yqzxhfda.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bujddlbf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3krhclnag.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3joqcupwu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qnfxlpsa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dwfmallp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3czwbxxov.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3okrlmrnp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3penlxnac.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uyzjvrme.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jvyonfrf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzmmqpm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bchksffh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gaheqesc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yquqfkwr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ixssmycw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ymjtxbdl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3skwfcsfi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lxhfnkjj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hbpqyrcr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xstdqovs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hyfsycre.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hxsavioj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jmatvpvu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hfzwiwop.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3canzovep.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mgzuoocc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vkskklhy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zkykxeqi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yunatfkj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fnhmjqxz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xalcspbh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3veqicsvk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xgbdunho.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xfueoeno.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hvpvrahy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3teospyca.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3upyursis.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3cfnkbvxf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rqyvkwbk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kgxssbjj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wakekggh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nlwunuwe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jdotroky.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kmbettvp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3txaloxjv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bqshcglf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ajwnlnue.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fhligizp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3expgbnmv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fqkupkyh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3sdnechlf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhnqwoqb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mlbiypgz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vvwjtxua.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mrsqyvwf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vfpjnqno.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fgimdrdq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ekqopsmj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rrodsaop.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tmqodiwd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3rqtcosjm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tqpwogbd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mjetfahu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3twaljame.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cmtvscij.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uoyvfsua.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nfyhjzrp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gzdfbdam.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmxybxxd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmdpsytv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gsbaxztt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uucxvdqb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wjqhmfzb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkcwcvia.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dawghlol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fixthsau.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uzhmemjh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dvhwegpf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vzresmdm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wpffbsfl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dsgtohxp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hcltsbta.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3chflhqcg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kxpeajjz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rohmmlns.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zcdcpijp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fwwcsxfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdvmbcsg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ohpovzmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hysegoru.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ipclhruu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xypnxjet.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3klkksjue.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qbqmrszm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3rlakuwzn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kropweeh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hfyoexsw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hvykvcbd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lbripdqr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3agnevrxz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xpyxouxl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vdvaxyxw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gkxuqshq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnhdpkbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hsneabfx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wrueyjdc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wodseiax.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xpjtgghe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aatvmjmu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gmbyvmok.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gpxqdgwm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zxydsdbi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3udwzpoie.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tpxrslhk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3djfbhynj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mmzuheig.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3saozekid.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fyixtgdy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mbttsxfr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fdxxdyxt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kkzdgbrg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3oyiytrrm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xswekafn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvecemcb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3aeqjhbme.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zmbwkoct.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yzanlsdb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rllczvvd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yrnrcffr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3spizxudx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxqrpbyp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wysxowdl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xizvqtvz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3sxpljxcs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jvtwgodi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cdbltpvh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwxfoujn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cktyfnlj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3aesqdcdu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wqyjwzcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3guebkvht.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iaugwwon.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jynivfvj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sfbgcnpy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dgjoutbl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3stwlfvmc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lhrcigpy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3frtiylpp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3czecorir.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tmlsxzey.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3odqiagzk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tduymjrz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ngkfjjjp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xhaqjsrl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mxlzssxa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uvtimlen.html


<!-- 参考信息 -->