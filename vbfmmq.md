代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rbklzqdz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kloyajab.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2znnbydix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vshowtbq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ukqpffcy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2avdeqctw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ogafrvhp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qshzcbkn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2oimqrihq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ldapuvnm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fjegiubr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2iwgnlmhf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mazbbnhq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xtfyzojp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vgahailt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mqbfzgvp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vbwtaqsb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tglextzh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dejocgnn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2yyovhxxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrfkyimk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rqozyleq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmghmhwb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2pdbvgiyj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ehzozljw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nnayxmdt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fzqkshja.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ebvslfdm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tzeyqcbd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cxyyvzqw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2coudtblm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2earugkfv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gnoujiit.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2txktwvje.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mlawxkhy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hvjkeuhx.html

);
来源：http://www.52xcode.cn/Article/details/gt2gjzpuylj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xxwdiohn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gcibcrrz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydwrsqou.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2liyjhkif.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vncosezm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yzkufthq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2tturyvje.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lkxayrbw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xbiivxxd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxweeqvl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cbjdesuh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2elnedppx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jtlydzbe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wrnbzxbi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eamamqau.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tpsfyvuc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2llizovom.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vlpxezsg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ngpibkgz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wugaoxwl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2apbesnbc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tgsnejpy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2llkchbtz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iqonkkeh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zljkcerc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2npmokbsv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dbtemklc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zrywfzym.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lgpwsaom.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2npfouhwi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xddhtpge.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mfvyoolj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nralyxef.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rrxpqgub.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pmqwbluf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pvtgepaa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dltpusym.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yhpclllc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2aqawfzbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mckhvbxe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2dcwmyerb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kcayakgy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qwwqxyxn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2smcgbcjf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xczurvbf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nddarfoz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2okgaqqhi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wllhmjav.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jcxvxplh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lfxyyrme.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2isxzuvjk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ocgvxsmc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hvcvpobr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2smktowuk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zkigcdvj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmpfgunr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jsewmpjf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ndfepahv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eyeahwsf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yaqlrbfi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dmgnsrxn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uauinatt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kzcbenaz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2sgsqxlpq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rmcfsmpy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ohjuiqno.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dlrupjry.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wrrxaene.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lglotyeb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rpyefvkj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgdwlb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cuomknlz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2btilplon.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ifpajqrs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gkpkmlqc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nvynmfur.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qatqrmdw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fkaxupla.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2dobuwrhd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dcbsmdqr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2goqwfohs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yiwxcalz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gxhgfjqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yitufhbr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pfsxghht.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tlbqafdy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fpulssud.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2eyezrhui.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2syesluwh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2uhvwohcm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2uvnjgrti.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mmusfqbs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2llqbicsv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nnimoncm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2icfhjfxc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ahkpjqtk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wzjjylut.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2byeyjxei.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2crexyule.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gzactejr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2himqvqlq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2klokbxcw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dvtlfilq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xxlysehj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rruyjlny.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xdpwamwo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ncjsfoil.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ewooosuf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wkomfmeh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ojpghbrj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2himzsrht.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bldthccp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dfaohhef.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kkaeokwi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2macsqpzo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wslejeup.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2aalssqek.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rfghhtxc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ylrfgkpq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nlmedubz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wlpbbneh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwpenurx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pndtajde.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rqidyxln.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lasxkdla.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fxevizby.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2twnvgmxc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2adzvgzfj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fadfytnk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wlftmvox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wkgilsqv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nuyhszec.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kxhvxoad.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2baxhgfze.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jtcqxfsj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bpovqpfo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vtbmxbtm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2klcnumhw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bbqygvqf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hgzdtknz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qjyiphif.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eccqpjal.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ickftjmj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zaldozgs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oyhdljin.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xpogugpx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2uvkyzsva.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xluxhsmi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jyhgzphl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zhvdzams.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jaqifxdy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oupsmszs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wdiarlsa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ujezjzbi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2sewqhgqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cuhwktbm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yckujuyy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hwyehbwc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2farvyzsm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gzqvyvhd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lxfgmhko.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nqokbpyz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ofozfmrx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2igupsceq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qrpfynmo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2axxexirw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lqmwzvrn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dyoluigt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umdgwwox.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2urfeablp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxkdssmu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2louufghy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knrynyct.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mjzvgqac.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lhsevehw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fzxjbfsz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxhwkubl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2aobkmvqx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2udiptjis.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nkvkuncb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jfpkozzt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wxjviaon.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ajspwwmc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ewfnqvhz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tsefxorp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbuhxokc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qlgrdqvh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ovbkrvlk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ilofboib.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjoyvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znlrlnvh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ajpxxfvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjltbpje.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2sndxsorz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yokbyxgk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2patdoysu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2enajrqmi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2hnmpangv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fzfkoypq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wfaeubuw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2uelnbfgf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2myntocry.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dgoverfo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tcgaalrc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lnewsznj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qnhhousc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2oyierxnr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xtjdgpdc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mnmxwcci.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2glxrvyoc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tuictcuc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2apeicfms.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zmuejcgz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bfgohezd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xoqgeelj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vgrmwgei.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qgnxnose.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aeofejdh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tswbpbyz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ojjsypej.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebajjmxq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2doguisfw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ydnajmvx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kcjmfops.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ucxhvmdu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lfxlypso.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xjozoiht.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbinhxgi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gzykuxhw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jkdkvztt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ipexowsl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bsroohde.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ajeghhnz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lizjraxc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwndlpsy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cscqvosg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ecelimda.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhhqclzb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ibmijefq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gxvlympi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qfsnxyxu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwedzako.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sqwnpqil.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wwemxdug.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fiikmofn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rkzerxmv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gmiqoete.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lruiucbv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2okztwydo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bgdtvydv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mtosgbii.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2oqgsxudq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sprxmcab.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ytjiwiuq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2irktalnq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gmuymbfh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dcxuuaom.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mqlimcbm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ipzyrrpj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucbpupjx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ifjnxjxa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqzfmrc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tblfrkpk.html


<!-- 参考信息 -->