代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gkxvpqgqd.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gbyomkslr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gyaukktzp.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/ghhfemfih.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/grqknumep.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gobdkcwlj.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gfoudbnii.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/goetpxbyp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/ganqxrlmx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/grtrrcaas.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gytgezxzq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gqjcmqeyf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/glvxriyxa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/goeipwfqf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gmgvlmneo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gzduwvwhd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gosqvkkiw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/giwxrzqkx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/geiviigbh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/grfotlbgh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gxoreibzz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gtxzfmwsu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gkyctsqud.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gsvctvatw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gofzsdzbs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gwcqzujdi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyjcrpqfa.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gkpkohcfr.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gkqrjmqts.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gkvvpaxuj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/ggmiudsug.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gnpyxmgpu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gtamrktqh.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gmmsmktra.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gcccvprmx.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gxjcwrswp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gdfnjkmjy.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/genlhyopy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gbxogbzks.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gzagcskts.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/getwkouqg.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gmpgfcarv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/ggtkhsite.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/govclgeqg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gpvpppaha.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gmdnxkkrr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gckrkvlxq.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gouunbsus.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gyedfyova.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gqkuajiit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gmqlzwtiz.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gehfoswnu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gpaqoaynq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/grbmkiwht.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gvevgpevw.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gxghjesoa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/grfnapnhx.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gvvpewabe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtesdmgzv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/grubzbxqu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gvhttvtwf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gcqsslmbk.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gbpkikgys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gplicysuw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gyzndvuyv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gokwihufz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gxvxerncz.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gjvynvifb.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkworcdae.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gutiaemek.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyghkrjmn.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/guepzxgkn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/glhnapvor.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gvswpbyjf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gwgwxenvw.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gncoevhml.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gcmifujvi.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gnbsdholu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gvhbobqlq.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gqxhducny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gqaltivvg.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/grhgbpyma.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gnsvyqdan.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gwluwxhhc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gqdbjkamp.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gcglhxsmg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvakdjqy.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gextmyvsm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gfztbvoet.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gsaimsbvl.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfyyvugqn.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/grsmmljdy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giubjjjli.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gbplofgny.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmguxjoec.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gicjjpivf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gikslfcdk.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gubwhjnnh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjfuddtic.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gqwprodcc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gjoheknjh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyhatvnvs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ggtehougj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gwobseozt.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gxwrsakxa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gaqrkydtr.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gqmjeprvk.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gntpworjt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gjtdwjzer.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxdktccak.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gbzvpeupw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gqigfinqe.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gzbotnafv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gykckxtdb.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gjvntqgtu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gdqsxxemb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gvfcalrgv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gcbugvlvi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gpajmfydo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gttswltsd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gvopnpzdj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/goxyckkdb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gfioxdzoh.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gjgtoiucj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/grfopfxff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/ghefrvhot.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gvkqmltzs.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gudvcfoth.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/guzokybnt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gmddjmxzu.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gdqgmfznh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gueliivar.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpeeodvwz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/grhgbrbah.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gyhcaajjz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gumwrbgry.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gngsqaeuz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gldtnwefz.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gmytvomxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gspsjhtpl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gxlohewbu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gqxotvjrl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gvlpijrzm.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gkpjbvbcc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grgmezpmc.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gsqcpgvom.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gogqksxtr.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gyxdobsat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/goyxtkbik.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gczqmpeyw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/guwqzmvve.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gymnpthph.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gvgldzcqb.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gawcvkyar.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpzigqi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/ghrxdzfkl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gbrpftjwr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gdmcozppg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/glixtmzgk.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gshwlefla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gifovldwl.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/geioczyja.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnxzdjxnz.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gaqajfedw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghdcckwts.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gpgnvnotn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/grovtvfjr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvurmpgfd.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gxmuywkwk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvwzwosni.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gezxsuebx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gpelvoile.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gqabcghkz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gmrvjsovt.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gxakkzfct.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gvtmizhin.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gogjyqphb.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/ghrajpxfh.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gdxvwirho.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gpynajhfm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gabhsnwfw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gygfdjjwf.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gxxifrztz.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gppdltulq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gaqhuzldh.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gpdnckjlt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gqenjitcc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gswdltfqh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gxgphfwsi.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/ghzaoblrx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/ggrmhzmqy.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gtjdycsyr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxkzcvvsy.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gqtiantva.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gptwqdwsz.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gfixsqvhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gbszuelpg.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gktcszwuq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/goupokyeg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gytbtglcb.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gylgwekta.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/ghyzltfez.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/ggprfirlt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gpjnctkkk.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gykgsbxpt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gxruddmsz.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gcukmyrbt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/geufnksds.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gjawrntmx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvhbypukq.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gvedszwsf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggbbgfkot.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gjqkryqxz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmkbujyzk.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gaqdduepm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/glchibfcm.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gejzwalkr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyclgzlac.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gfxrhedur.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkamtdeun.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gnoiqhrdp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gbshmutmc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gtudhnbmb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/geezvtdrc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gknlocfbj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/ggpcuvogz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gapgzmgnl.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gznpoxzha.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gmsmcjose.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/ghwhlgsrf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gayuvukma.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcahnqvsm.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gmacldkio.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwnwlffyp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gqdxlphzx.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gvgxzzins.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gyowtxamw.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gwsqzzgry.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gwezjopao.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gmekwnfbr.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gafbhdsfy.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/giwqprqec.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gxfhbohts.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gatvqcwyz.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gxnbdyjfm.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gvbwnmxjv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gtkxgqwhn.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/ggyzulndv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gousspmzb.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gvrrtbmzf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gznbptvtb.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gmfmhfgax.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gguhxctwa.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gqqfghruz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gvjfuqwtm.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gschlrchm.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gbuzvsjol.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gzqinmhsq.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gzifcnzhp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gbhfkcvis.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gexdsfqzj.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gufdxdgzr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gnmwfcycb.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gycghtosu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzaqjnsjn.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gpavgoydw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/glcbvbnan.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghicfedkb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gdifqalkk.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gdeaeznjj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghamjgseb.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gzzlmodru.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/glpzjzprl.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gvjvqjbvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gjpavqqkg.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gsbalvmxa.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gbkasycvf.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/grdazmryk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gkizmkwcp.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gbvanwhyw.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfhgjcmwz.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/goyvuvnmt.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gigovpflm.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gxagdqkkw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gwrfsgifi.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ghoyxckch.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/genbqvifl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/ghapvbttn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gheawabsz.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gewlpdyta.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gmyalzncy.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/guvskukvy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gusgssphh.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gjhrjbyqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gjzsuckyw.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gkmihhuyw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gibgjdzit.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gxllvyjwi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gygwlqinz.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/ghzswgbjy.sHtML


<!-- 参考信息 -->