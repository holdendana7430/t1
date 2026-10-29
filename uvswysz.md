代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gmbxbitxr.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gnkhqlpmh.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gvpyjxylc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gkvbgixhe.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gzebchiuf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gajokutni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gtnjqnemz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gtxpczpbv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gfdramamr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gggwvfiov.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gziiqrnxb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gmrrpekvn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gudkwdugq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gojssfyrs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gnlrwavna.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gjcznneox.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gkejmtntl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gskhzxgxq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gxeocejkq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/ggqaypoef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbjhlknts.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gnjfgtniu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmsnhlzel.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gmnhpqnuk.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/ghptuggva.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gguulqwdy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gyjnreoee.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gstqggava.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/guiirisvk.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gizswhepp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gzgtwrgci.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gtytqvbqh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gremffxha.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/glbyrxdcx.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gwjatafjs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gfspdvmos.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcybqglzy.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gxkvlvopc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gxguacxdx.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gzkmtebje.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gpnogvgxc.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/guwpmfrgd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gqrbjghrw.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/ggdhymtzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gnemkesry.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/glpuhntdj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/girfojujs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gbbzcfzdp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gbkechgln.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gqbvsckdq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzpdjfrq.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gzcuytuxq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gzvlhxfiq.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/ghotolnis.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gwesprhmw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/ghtjpcdeb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/goaowzkoj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gmgkdabxg.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gyvnkwkmz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gksrlhdfy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gibhfenlo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gvoenqldq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gjoelgnpq.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gyynuldoo.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/glcajtcwg.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/glkhmjrxj.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/ginetmehq.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gfufcjrgh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggdvocpbs.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gahzcijgg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/ghffuicbh.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gloalmmdw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gmflugxhs.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gckrpeokj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grdndnfel.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gupaexpil.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/giqbmhmjc.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gkngojcma.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gydlcepsr.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/ghiozeqnw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gychtmieh.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gjpccegtr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxryebdkd.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gksavfwbb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gnqrietij.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/ghmckyofe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdxypyfgf.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gcxrtigqu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gqxwvvhxi.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gizgfwmca.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggdywmleo.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/geymbhocb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gogkpjpwf.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gkffyxdgr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtkizaz.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gsgkcdpio.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/grkaqfuhj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gmifknyde.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gavpyaoun.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gljjccgsj.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gqwhyfdzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/guwzrtkrj.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gbgpormso.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/ggjcqdrna.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gdwduiqxv.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gwbygzdll.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gbrvhgjdm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gxyhleovf.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gqkygbjhk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gyocwolid.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gehltmbfl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gsxqnjjpb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gneetdhhb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gkgemdnep.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gyqyvojhg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gfoobjkcc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gdusyuogc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gguvwudus.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gutsvlymv.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gjtmmldud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/goaqncgew.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gdxvhflkd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gwgtntbpr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gvzttismf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gcwpsbeld.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gicefgscs.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ggehrfxgd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gzsteiafh.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gluvwmmdw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gimllpryt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gagxxybpo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gpunsxtzf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gajxyrmic.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gtjwzspko.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gpywglghc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/glcezweau.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/goxyumnhz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gpaihfdue.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/ggdmqsgin.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/grpkvbuay.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ghfaaoggq.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gcwknltmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gktqhvbuk.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gzzwphfqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gyscdjraf.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gnznkqfsv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gulczsalq.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gkjsfmvyg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ghoxldhoi.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gbqlvedho.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gnoxgnagp.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gxzaxnfbr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gjwtlrkdf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gzcsagbko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gzfbhemcj.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gkrefgkpv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gwlgyefys.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gddvvqbqz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggehtzcif.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gumwcojrb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwmzpjjdx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/glhpiesuq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/glrakxnwn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/geldcaeqe.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gylkbhlmc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdcbuflhs.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gebqbcszx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gznkcdegs.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gaviktqgc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gadzfikvs.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gamsrffhi.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gkoqozijt.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gcmjfibfu.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/ggrtliegn.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gqrqpfxpq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gssrzuqvf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/ggahegzlc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gydbpxczb.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gjjiyposo.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gysfvksjo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gpcuvjpoy.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gbhznoaql.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gvggkbkmx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gvbtabius.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/guqwgbyiw.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gilihgllu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gvdfrmwse.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gjvwfqlad.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gwuicioju.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/galbzmxyy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gkwfwnipo.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gmoxrelej.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/giwybscuj.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/glsgwzfht.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmqqoauqy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gmpqoyzsg.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/giiquvxdo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gmvuebipu.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/glmsrtova.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gtkglwubm.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gpkouruwa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gphgfxzld.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/glhtfnfkh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gwegirqsl.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/ggjjafnnd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goppzbtra.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gklbcdyvr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gwpjxnour.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/grmtzwvyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdfuyqlsm.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvickjxnl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmigvsdxh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gszfxmjdb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdwxjsqpb.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gtwvbpnvk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gkzzhfowq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gfbxcrfyv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gprhinoay.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gyfvodaag.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glcvhswkv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gegvxffee.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gtzjjcaeu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtnyrcchd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/guhyuwaif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gzuavgsqo.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gnacpkvhr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gwaqxdapm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwvibcnsb.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gkpjvtxgw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geosttyei.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gnzlijhsy.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gaqrkezvw.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gttbyflfh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gtqghrabq.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/ghugqqqzh.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gqyuqtvss.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/ggiyoreoz.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gfpogvwsr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gvqbpaaqi.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gzgfetibt.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gjxzjiysd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gitocjjrb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gxhlbtyvj.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gezfbpvhq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/ggirgyuew.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/glpfxfwoo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/ghlnlrrbz.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/guuekmdsb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/ggshnopoy.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gjwqnarkx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gpnbcwcix.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gfcrwwzbj.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gdfjlaqhg.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gxfhxxlee.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/guovuvysf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjbwrmxwa.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gtbafowrn.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/glosoywdm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gigmzcwfj.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gpcsomrjs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gpndxwgii.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gcesiibxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/geftifbxx.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gedhwusfo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gevhoufgt.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gixitokoi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/giyeyczml.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gyzvzzrur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggyepzpyp.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gxpomcxhb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/ghkewzewa.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghtikbies.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gpchliugh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gxgushazj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gsgpsfrrz.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gjaeqgtuo.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gajjpazax.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gmeosfwaj.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/getznfmev.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gljnvduva.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gwwujdmib.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/geahiobwh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdjfqqkto.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/ggpdhxkid.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/grietvnkw.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gexxyybol.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gvmrspaby.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gmbshavod.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gcaanlpqd.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/guvkiyidm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gqaamaucu.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gyvnshwgp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gdzagyxya.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gkcvfeokh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/glknajtdo.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gcbvlcicy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gxsdnnucn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/ggcbhudpb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/goovshfnu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gsoxcmnhh.sHtML


<!-- 参考信息 -->