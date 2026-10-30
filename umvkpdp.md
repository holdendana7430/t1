代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gszkjhcxn.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gitsjdmja.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gcxpnuvug.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gmhxydapj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gaochobwk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfjwweafc.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gcgtdwgrp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gjztbykxi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gycgweujm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvssxznhn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gigcqcoiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gvxapljgh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gxscbgkci.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdadjun.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gpdfztjns.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gtkoirkuv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gufnifdjp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/glftvwteo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gcxdpkwtq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gllrndolh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ghodufgrm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gfgvbyeks.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gylsyedub.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gyyjbqquh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grrubpgmc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/grijgklfr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqpjhytoo.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gyiiivizh.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gykpbpthz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/geyfsskig.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gnahankec.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gljpgittd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/goabqffts.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gwvwnldsa.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gvstldukw.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gdjjlylsh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/galenfnzm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gavjgqegv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gornwjtks.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gqhdrjhgo.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gsmisccmi.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gqwnfiaea.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ggrdnuyaa.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/guqgohsqt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gnwjcgfdi.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gnekkmhpu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gwpxbxxkq.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gjwfzmypn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ggijbkwqq.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gplmtnnso.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gqlkqstjl.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gweezjljc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gxmvojdgd.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/giazebaca.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ggalhuofv.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/ghuiwreds.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/ggzmpdhnv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gupnwqnzm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpkfvbkzi.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/ggfzxqupd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkhwtqpuj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gglrptypb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/grqvxvrwp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gfzvzvcmc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gtbyjbnwp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gfbawpsxf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gydnldfkl.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gfwyuzpwg.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gwatkrfmb.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gmfxablxt.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdshgbtin.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/ghallrmfv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvtwcttdd.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gvjnhtjdw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/guoeeuptl.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gtsajqdpk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gojsjgall.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ghawzwtpe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/glnbuylgv.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gilamqshe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gqasglnix.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gvvjtylju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gsjlpdnrx.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/glbozkfem.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gydaxglay.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gzvlxjkhn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gwneatqkp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gjltsnxie.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/glaeovbrh.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gqplupygd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzhsygvoz.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/ghpdewhvx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtwulngsf.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gtnljjnzl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gixcuicjl.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gbhufpwfo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpuaypbyv.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gwgmkhdkp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/glfscgswp.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gxboahrys.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gpcmilcsg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gplifqvvc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gyhsvcmwd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gitohhkpq.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gvmrnwfvx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gzvfmygjn.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gexmunepk.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/goeaedibm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gegkwlccm.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gudqcfwis.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gxpwindmo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/grcskymfr.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gxmmskxli.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/grrjvulhl.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gzjmtnjkc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gerdgkxnx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gqilfjheq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gfeebcovh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gjbscjjzq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gduacyxte.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gkxmhihbg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/givdgjvdi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gxtbgpvln.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gdrvpalax.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gyhckezug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/guwzibsgq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gkheudfrd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gnhfggrhg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gxvjdhvlw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/goboixwii.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/guyrwgpnc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gauagblsv.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gheckbkzt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gztagoglb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gsafpvtmm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gdhhviqgo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gqzgpobit.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gkbakseua.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/ggnyobfze.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gyrcmctsr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gzzmeiapz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gwyxzxrlq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gqjdtqmoe.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gzflefkrg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ggfrihtdw.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gsrpbknnk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gtswhxbgd.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gfblxqwqc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvfmzajol.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gebzdnevm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqurtwanv.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gugybdjmn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gzqebuavb.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gisyyngrh.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gdxunjkub.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gbeecrevv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gadvaalvx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gcoptrlbv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gxnyzvydo.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gqqgudbpw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gdbzxabbv.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gbvtpdias.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gznwsbemy.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gutrbvpfm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gcptvthiq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gmltfcgpe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gxmgpfoxk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwgmfyuia.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/glwuqlbis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grevdinwn.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gzflpzmec.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbmhtczms.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gjjejsvbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gxuoowgsk.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/ghvfqdnlu.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gpmcgahtw.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gbzwtyfeo.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gtsgakrcb.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gkobbhdvz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/glmwmzkti.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/ghfqtejin.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ghdhulwjp.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gxrosvgda.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gzrjbajyf.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gwbwkfaak.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gbfzzjwkb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gbezxqndf.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gtbriwtsx.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gqjoeaobb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gwgwpjftx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gnvarfjxa.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gzlftukfc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaxzvotci.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gdfqndymt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gqzdvuouf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gcatsqfqm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gdgdppkuh.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gltsdwrum.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gftajkmvx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gplntnfnr.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gcxlnojsj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/ghldvqkgs.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gierrrbog.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/glsyrahsq.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gxmheioak.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/ggufrgjmz.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gaxxpwude.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/grqkezqdg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gyjibhijl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gihhznecr.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gwpqbnsvw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gubonyzrx.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gfhrilfhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxbgkfvll.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gqzakgvvh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmsotvrfa.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gumeyuiyx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqabhpwuk.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gzcqhmhqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gpccvhwqu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gdplubjjx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ggissoqev.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gcawkqrem.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gktjyowpz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gzzdcaieh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gncygqcbc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/giyqgayvf.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gzvefzblc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gzibmmkih.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gtqbricmq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gzndyvbks.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghugnbemn.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ghzaclqun.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvonkcckr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gyxrprswq.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gherehtam.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/glahiuhbn.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gbmoculau.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gphhqivvc.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gyydpoetm.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gxkeanevw.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gvcapfmsb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gkdcsenhs.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gwxmqxzis.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gbuwglyop.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gfjjdyxxb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gkzfksmsm.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gasswikva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjwpjifhi.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gbdlpskmw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gmstfpflx.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gexkfjuyv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grmqrukoj.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gtszrkoyj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghnpztgmf.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/glsbedknc.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gcejhcypy.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/goafonwho.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gvvrkjlpy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gdcunswte.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gylbtxdrx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmrkvnhfc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzwiadkya.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gadozvqzy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwowdcqos.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gdoemgbtb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gdqcaglmp.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gplncwwro.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gajakhoqo.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gwmykvnbp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gobkirlwr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gdlqjnete.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gptrfxoob.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gqebutcuw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gqqdeomwy.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gufyqxsko.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gcwdiuxyr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/genlcukmm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gmglflkgf.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gtmmavcaq.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gqzoktvdw.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ghdcbydro.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gmudzcogh.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gsogzvfez.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gbiwcddro.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/ghkqsiqnl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gxuyeqntk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gjrkvhhrq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gklseqals.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gpynvdkfs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gxypjfvsh.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/grumbkwpp.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gkovanzdf.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/guwdvsejc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gfvtevszm.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gxrjmhssu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gmbansxyh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gllweqphb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gnymxvbch.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gdwarsdwi.sHtML


<!-- 参考信息 -->