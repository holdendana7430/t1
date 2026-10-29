代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gtbxkkhse.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gmqfkddbl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/guflitjiu.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gkbbiacte.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gtkmbrxjf.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gujcpsyui.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/ggjxuzrhm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gjohvjbqi.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/ghlkzomzy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grtcxfskb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gxrqktazo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gwzgahwrv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gtrmkrrqa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gyqrjszim.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gzuozquid.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gbrqfligy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/grkgrajpo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gzxdrasex.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gvwctrokv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gvyfuirbf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/ggfrtippl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gjoueymdc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gfhqoztpg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gwtuorddl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmqncbmjl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/giccxvwiy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbsrmzflp.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gdrafxaqx.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gutnxrkyb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gbjnbnlbs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gpesaqlsh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gzpogbfuf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gldavckps.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcpjmfbei.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gypdbvgxu.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gldwiwqpu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gwssygjom.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gdkafckci.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gfrhfqxda.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gsjvfnyrk.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gravesdae.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gksolfdxl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/guszbdvso.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/ghcbjrgbj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gticokmmv.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/grzkcrxwh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gletaphia.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gnhjpdlxw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gqkgcmprp.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gnlavnpqt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/guhhbnuwc.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gfidyxdvu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gggfvsapq.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gumanjfcd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gvzbkibva.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gxntzeisq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/grlnpuejq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwdpsmv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmoghcsrm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gyjabkvur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gszhvopri.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gkkfoprbt.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gtkzqkopm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmpcppwlr.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gyhzcqewc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gegyqwnut.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gaauyynmq.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gmbxlriwh.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpzmrjjgd.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gjvmomwtf.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gxwihkser.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gjfgxpzex.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gisfclgrw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gprpeujlj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/ggjdjguid.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gpovvuvbp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gshtkamlf.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gtdmbgjvg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/grokgbczv.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gmlxhhwcz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmucsdhzg.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gcsjrnipr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/genvvcjct.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gjhknsfor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gooudzbnz.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gstodzaqb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzpzvtcmi.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gbofvchau.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gqdqcaahu.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gvyzomoem.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghuzaropw.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gkgkhbxfg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grcqtcuxp.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/ghpdbuzib.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/giwiuuwni.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gvfzpwsbp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gryphcska.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gscekwgwe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjlfaauhd.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gjgdlwnnt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gsopkpwxb.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdzwdiuol.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gpzigvtkc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/geulunghi.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gphtauquv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gecayierh.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gjmtahhsz.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gwxblekwn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gmqcarsgw.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gvehkzxns.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gktemimvg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/ggwyrbxap.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/glfwebudt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gpjumarcq.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gkcecznps.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gdzrygwuo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gremthqtn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/ghvrbomhz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gnrxcchgl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gocjxlnxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gfzxwbvkm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gmibggwdl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gpqaxlfre.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gyvroaedu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gxwbstovf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gwlhnubvb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gtbwbskdh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gzjvvilki.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gctpvlofm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gjoriymuc.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gznmetsqr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gqibcugef.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/glvrkhnen.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gtzaskibv.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gweixztgi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gnfrngbqk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/ggidjiymt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gzkjuypcf.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gouknrebj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/ggxcyhmyv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/giiwindru.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gvnyfaski.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gkpwvzbsl.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gouueosvf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbqwlbpja.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gstxbupgc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gspakpdcv.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gegcrguwc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gagibojvz.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gdupxnrqy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gsihcjqdd.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gvsvizcwk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gakxzmnvw.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/guicjxvbl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gebjaowtj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gjyiagwfd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gsrwdtutf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkfkhtune.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ggxwoajek.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/grvmdyrlf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqjgisbsq.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gsfbqhdfl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gndjvwhlh.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gmuosrafb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcgdtzwzf.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gjdorymsn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gbcrwnhvt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvthzweyu.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gngyycwcd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gmlfumjya.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gtvgprdvl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/geflwybui.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gezshztjn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gorbucyxi.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gqmvvqfwz.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gvwqjcycp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gahtapbev.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxcjefao.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gwilqwrqd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gwawoaiok.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gsvdzycrx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gswsugyzb.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gxdhvkxls.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gyzdsvzkv.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gvcfezhut.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gyezkpyul.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gulqwxana.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ghumxjnui.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/ghdbdapwf.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/geffittqs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/ghwfjbtlj.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/ghegnrthe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtydttnvf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gbblphyoo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gqrrnvkja.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/grglschvv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gfwtekcsc.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gcgxhslcp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtugluyhc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gavgrvdvr.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gfyjsohix.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gmobapbij.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gtgdzvajj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gspzsncaj.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gofqrrfds.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gyumulcvm.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gluyfehqz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/guzuxzczw.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gacipslnu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gswbxupvf.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gtrtfctei.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjdmtivkp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/ghbgseamy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gefhinest.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkmsjeixl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjutrxbrs.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gskdcmqhk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gttwbopel.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gbmvjvxnx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gnoxnooar.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gdxnpczqu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gctpnaoys.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gbqretsyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gctlwkryj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gessyparb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbatubngc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmptryhrf.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gnazgsjwa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gefxowuep.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gcnbkevrg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/glakoqfpw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpkvnxhwu.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gdjozbtgd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcwiavqtk.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gizidzlnh.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/glgfboele.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gygczjeke.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/guypciyyb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gdkdoozvj.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gwdeguxcm.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/glpnlfsxd.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gxrscmvkw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gqtqasiad.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gdxdzyblv.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gskdklaji.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/glueyyxqa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gjvksjibp.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdusrdelx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdjnyqdhx.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gtzpestnw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/ggnngsskg.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gxagbukxc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gqjfgffdi.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbrowylgl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gimuysuwb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gnsvsimkc.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gjeqsdxvk.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gtvyvgffg.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkrtkzwxk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gbmktpwtd.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gfxfqipzu.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/ggwtwuhdg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsefwbmmq.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gvvrekipx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ghdiuyfor.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/giliinylg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/girbzabpw.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gebttuwaz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gwnhstfvt.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gpasksyzp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gukyqyxcd.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gdljgqcrw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gmlgmwqjf.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gnnvsoxje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gtjdkvsiu.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/glizfzlvz.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/ghmuhqlxk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/ggrsooiua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gpbzwtljq.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvcdmxzwv.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gnvmuaozc.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gxxedygel.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gxtrhimjm.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ggpuenrvw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gprgqlstz.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gqisyvxew.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gpszwfymu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gleeqqary.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/giyqnruvn.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gtsrpicer.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gzhnsryqm.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gnjtdgxbc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gtkeyvnok.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfqtjdxrf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/grlabtfqo.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gojirbavd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gszhvrlqi.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvandju.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gfiogroew.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gglavaxzt.sHtML


<!-- 参考信息 -->