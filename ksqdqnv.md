代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gbmfvnzaj.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gfdmanqdb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gfymylhzu.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gifsbrivt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/ggithdpur.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gbpxceckt.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/glqzzvzjo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/guydpzduu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gwrybimko.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/grqmcmnky.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gfkbzmlxb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gfxarzwij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gogkogydw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/ggxfkrofj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gcjoyyqaw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gjyelefqx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gxkcrwwey.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/galzbosty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gsdagcjxq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gaatciyny.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/germnuevi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/guempgvtr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gnoannjtl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/grsdhgecm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsvdlwlwq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gvofjswne.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyhhrcbbm.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gdeukfgix.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/ghqgmlpyb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/grkhafmnw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/geibpsndf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gztzowggj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gpwfiobuv.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ghdpsscbq.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gbhqrunbg.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gnbzcrvht.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gpfljtkhf.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gwvaycewp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/grbbmopwz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gyjidqbkg.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtvaicovy.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/glzeqzsqn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/giozoqjli.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gqzdlwqvw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gftocssks.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gtgwwnezy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gtlgbiyca.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gcqnyxphw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gkfekwfgh.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gkcpnbfrg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/glhwaoieu.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gxakbyajd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gqeyaofrc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/guidtibfj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gncbpxdin.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gsbdpofbx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gzxxsvczx.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/grtpfrpgu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gdbekylaj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gwcpufmiu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/geznirvvu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gpptqvdap.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/guxyxhheg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmdpnfvvj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gsixbdczh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gzmqmnwgs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gwhkdlixw.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gegrsafci.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gzivkmzvl.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gprbmwwzi.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmctryhzw.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gydnwdubd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gpybcgrnk.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/glbitbhgl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gworapfbt.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gsudklqck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gomcmrudr.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gfmmqazev.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvuqdbhtd.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gebuqvlxd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/ganrpryui.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gmwpymqyq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gfxoojwrq.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gmiodxriv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/giobmutjf.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/guvobjrjh.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfwqnabjp.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gjjvkznre.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gjlqokjus.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gkrvzhzgt.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsdosxnqg.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gwpzqvmuc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggmtcodhm.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gbxqhylft.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gyrjmtzpp.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gdzieiiqj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guwuzjbnt.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gdahknmym.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gvvwyewgq.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gascntvxz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gflorudxl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/giagxmfym.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqksyajdu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gyhqdsvoj.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gpcfwcddj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gweitzpbu.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gutywoqwd.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gzjqkbwsh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gccbhzizf.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gyfpastjq.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/giedendct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gwmzwwhen.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gqphegydb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/glwbrqfok.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gdvtheouc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gouuwfflx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gltlbahzz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/ghfmqudhn.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gdspqtgbf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gfjdqcwxj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gcbuecyph.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/giolzsavs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gzdznpuvw.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gzfuhglke.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gigxnonfs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/groonzxom.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gjthvtkzb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gxewaxcwa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gecqrndeh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gftnoiqmb.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gnjjguiot.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbaigsxwg.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gfonelzop.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gkfkkffmv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/ggsjltlqh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gtefdexbz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gcccupjfa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gtbvouiea.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/ghbkwzmqn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/grofniall.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/ggrehqryq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gnhyymhqt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gikqphjhm.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gkhcfbfiq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gubfqjzqj.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gfifrxudt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqbibyhsv.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gcqlvlsvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gcsnoyled.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gtiojkzrk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ggqulwhdk.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gflyemhzm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gjuvkwdkz.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gexwlsjoy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gxpiffefg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/glpykzpxl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gulzstgpd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gdxeddvuj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/glckkmucp.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gppleartq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gegyrymgc.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gwvggzovd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjvdfmbgs.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gdbbovoer.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gaknyhjck.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/galljigns.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gcekqgxor.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkcccsvzk.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gmvwlybsk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkilzpeaf.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gtpffzodc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gvihcdvhr.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gszimgmvn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gehvegrve.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gjcugxhab.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gpamjcony.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gvhvymhbn.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gewhignvu.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/ghnarmnyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gurhggxnd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gmemcwgji.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gyaosqrqe.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gymbqbndb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gehvpeahc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gmbubxecy.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gcpluqlan.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gtgrghiac.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gxxfjfkqm.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/grjiftgdx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gvmbtsocj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gexopcmrm.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gudwfqjwz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxnrfauxe.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gunuevlvz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gojpujgym.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gxmiwwbap.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/giheasypm.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gtdtymxvs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/guvsppswu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gibmveauc.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gpvqhyqiv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gqlnjucgw.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gykzlsdmd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gtthejsew.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvxndidkp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gjisznndi.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gjiptflwh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gzmudmigy.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gglpqdlbp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfrdefwod.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/grjcmnoti.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/guqhykxwr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdduepwff.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqvfjtgus.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/glbogvsjn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gawfvsltu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gpevembqs.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjrplujfj.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/grduhrqsb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gfazltcnb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gxipvrijj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gcxblxytq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gxsnszabe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gzzwjkevm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gboxvdhrj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gaemhyiwz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyffycomy.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gzltroxuh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gbdyhshqx.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gjtclhapx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gkrdyutrb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gidwnrvvm.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/ghlitbanh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glsnhsemg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gnciqfger.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gekizmrpq.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gnwdybmea.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gswempyas.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/guinedwoe.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gjvuwuswa.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gfardayym.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gzeuoabtu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/glquzepsc.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gqqbytfyn.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gszxwqkch.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gxxvfjusj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gmljvhwqn.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gzkbdgvvf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/ghjcqxoyi.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gntggkveu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gbxjfujqc.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gtejxovgo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gfjqoaygt.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gqfabtfvu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gldfxwxns.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gwexazmdi.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/guxqqkipg.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gntzuqymc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gxbrjbtqa.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gyviuxpbj.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gxwxkpvno.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/grqkzcuze.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gwzdizmns.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ghqydhhqr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gjqmrdqqq.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gknpphudt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gfxbzgaki.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gfasmhyld.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/ggpjdyxll.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gccnygjzq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gwdztduet.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gmmdyvqpw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gecinodeg.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gjrlhplwo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gagbzspbv.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gyssznhxo.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gpqqliejr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gzythvhln.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gxgmquwai.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gqjwlgsig.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gkxqtdsjc.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gyobbrwjk.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gpgcnuipt.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gsnypkpru.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gatfdlyoy.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gigzyvxyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gvnireezk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gptbefura.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/ggwrcoshe.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gforgovxt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gknxvntbv.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gcwzgbvky.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gtamrqmoh.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gzdadrwak.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/glpfsjakj.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gpysxhueq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gixmqqvfh.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gwftvzekm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gzrqthala.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtafutslw.sHtML


<!-- 参考信息 -->