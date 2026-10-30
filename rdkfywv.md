代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gakgjdlye.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gibjuytiq.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gnmoinbtq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxpuofp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsecoowqk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfcseka.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gtuztdawq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcdqmiwg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgpxwgti.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gacddopsw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gmrupkgnm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gyupdjmhc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygrwbwef.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfeyhbpt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhsuoeub.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsrompsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/grfxsrtyy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gthjkafly.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/ggbvxvive.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gqfbewerh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqwgqwiuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfcbwikb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwhyapxym.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gtnsjiebq.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gxjedohjf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwvnetld.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/ghggwkkux.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gocxouiav.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinwryyg.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidefvjfa.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddsfhsua.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gxiqwglsz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gblbxwkvc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvcpvffd.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gykykictd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhmbhkld.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyrtesut.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwjcnown.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutkbdoxk.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugqqxcy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gadbpzgyo.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/goxhcuqhd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gwizewfik.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzszkohb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnigyazvu.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gsdrykydy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdpmxvevp.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxnpjmrm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuwjfijj.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gfblxvzpz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxicydbpn.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gsgvrjraw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gbfmcobyn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldzkqcxe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabeswcgi.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gwkfjkoet.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjzuctkv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/glojykspa.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gbruyizfp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/grqosrgoo.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gknumyquv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/geglkhjeb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjxpvpnf.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gpgbkmylq.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goiwbhxub.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrssgpa.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcciikaui.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjqnobmf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtugcxso.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpbiamhr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gcsoowqkb.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gvvgfhfhk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guizyjyan.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcubyvy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ganfzcqli.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gjitsoaqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxamxydop.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsexyzzj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjafvjwwp.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/golchxbwo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gevcbxflh.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gauctjlvv.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gydpcegvi.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihiwcxpv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrvodbem.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gncvtonys.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvatbovxd.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gvjsuokir.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvkyemcox.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfubaiqdn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzisrycml.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvszyspc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbowopwtl.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklxpcqcd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsheabwmk.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpwxrzqy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvilyymi.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdklnlbyj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/guwxauhid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gaahjkaxq.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkzcdxow.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrqminvr.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbpnxdhd.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gonzzpovz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gytaicijc.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/givukhdyu.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gkbztqvai.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxdexlso.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwxjeyvd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/grzwqvjal.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkgnvvr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghtiucmwb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvsrlqk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlrfpyrb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjsmezyo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzvokszc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfjsupzr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzzjefuz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gadwujobv.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhhbhqst.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/ggjowmdmm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giitdyshj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgnylket.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnhnezxt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/grabsszix.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzvlyujg.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gltixbawj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gagvlrcrd.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmturlff.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbhfwstl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gucjjptzk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgfiiioi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/grtgsgxig.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gitnkeutl.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/giuowudps.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/goiyduxfq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjougpks.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkcqdtrz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gckecyhfe.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyjyyeir.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfqwgvyu.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gufsyxdxs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gbfkarqyd.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/guyjfpguv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnufbqbf.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gurezomby.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/glhpetrkq.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gipkkcdqs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gurdtltqn.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxugiwne.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gsgtobapf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqqdypif.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvpawrfuy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghycazryh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpdhydku.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gstymybsv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfxixijc.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcwqjtvk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwkshvvk.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gygqtrcmr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/giesfibyb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqynatyns.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gjptppxnt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzxnlwkyr.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgjusgyj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gczgramsx.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlnlqloo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqnohgpl.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcekqukfs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gwyfpbgty.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghvnpaede.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gvzpefwpo.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtntwlonr.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaxfqurl.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gepzyxcsq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gycmzymbg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gobmaepek.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftidibmj.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcampjbp.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmiflfric.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gguohtzpd.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gtocolanp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gveveuxjc.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gldmsqgxu.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlctmstp.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwmnzwmp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gndtqmtgr.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/guhnaviaj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbvfstdu.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiyeumgk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ggehtkyuo.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gvorqvyhn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyevbcdzo.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljuzzyea.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkfrpche.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgotendt.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gydkabhwy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gberzxfbv.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gobwaxvkn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfufxbez.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuceshqw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gatbvasae.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/ganjkfntn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gsmitermn.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdkhewbd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpjazzbo.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gifnjjecw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzoqqplld.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/glvwshysy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glcqruzpf.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxerswvak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/givhmoijv.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/govzyyybx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grfagrdwu.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gbuhhonmm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/goyksidhf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gtohfguur.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/guzahutzm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gatvdodiz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyetjgnsl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gfoietrkz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbxpwze.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkrqmxhx.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvpkkmc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvcarmjb.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyolxapz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gfcntbsuj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmhhczd.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwooivgjf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpmxmcjrx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gwijdfjwi.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gjvbuhkms.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gepekmkei.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gxonsqncg.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gctfcqbtz.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoeeyyvv.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtijqgpk.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwmjifnp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gevdqxhaj.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gimcmyyul.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdfnjrqq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnwzaxxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdbrgevo.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqemnlcis.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbyoaqutc.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqyuxbtmi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnsdpfdz.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegrswfsu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gegdtmvcs.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gymnbuqdh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeyuldaq.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gboyxtmuz.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gcojhxhjb.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdxjrvaw.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpakeckih.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gayxyfwln.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdydennst.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcirywhhg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkfxutrkz.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghkqfihan.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gquksrwsw.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gidmrizee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxrfpgza.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzajzauaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxdlfscpy.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrdafvof.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/guysrkiqb.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpfjfixf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqcmkofa.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmqdxbkr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplqsktip.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfuqjblb.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyglilpzc.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/goitjorbg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/geydcocvp.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcljliht.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcyhnvvjh.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobdqect.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gizjysvyx.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gydqsclvd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/grytfymss.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyijaxpsn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdrxkllmy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmgnkikz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gidgrxexy.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfkskzlq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpokvbfnq.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsldlgdt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqyqzqyn.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gitkavuer.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/glivyamxg.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgzgvclf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvznbrkyx.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbeaimpgt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gctdnzkja.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnikuoxzj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvojhmqy.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpczefgbr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggvxhieok.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtykjpzaw.sHtML


<!-- 参考信息 -->