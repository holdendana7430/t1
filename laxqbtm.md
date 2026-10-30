代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/guooggajy.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gpmkopwxo.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gkeappjrb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gmrfjmkqa.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/ggqdeugqh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gxgrjmyjm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/ggwtrehbo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsvejkjrr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gtgzrxfkx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gxrybuxqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gfkwcjzqb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gftfletjt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gqdkqzaaw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/goakotdcw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gzfwxfuil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gtlquybhm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gpcechdwk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gskiztlpb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gniugdqhp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gjmcpgbuc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfeskowlg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gogamogko.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goqavjmgc.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gwghipxms.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gtquuazwp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gbggrytql.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gcuhigfns.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gdjxcxjhz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gjjrrrerp.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ghoinqrrc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gvqqetgut.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/guisguosp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbwpxnrer.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gxrvvpifl.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/grbwotwas.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gwkpmcqcf.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gbgipjonw.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gvmgimynw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/glejxkblh.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gkecaqazg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gwyplxixm.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gbqhqjpxx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gabilvwqn.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gzuyucsib.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/ggwswojkd.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjtsslr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gfpefgwsr.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gxdbrjgpf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ggrvzskxb.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/ghgqzscsf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gyccivcxh.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gduhmbezc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gylcwhmhx.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ghukvlgdn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gciuqfdrp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gjlwulldt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gnpyoezoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/girgmolww.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gclsnsqop.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/ggonrjzri.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gyyrvgakl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gnwhejzdb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbzkilo.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/grmqujtjs.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjeevgyja.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gffnpcaji.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghyqlyhwi.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gbrehgmwj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gbytgpdev.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gyvevwumx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gqwdzpdtn.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/grjcbnxxp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gbgmciszg.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gsshfrxgi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/glmiqgueq.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/goeyuvhyt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gjuymyuwe.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/giaiworlc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gdosjlskd.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gwvibsggi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gcekaopny.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gkifkswci.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gmfcjagxd.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/glcmdsrwh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gkyyahafy.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gdutcnpvd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzppauoye.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gsbvzbzbs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gdbvoymtv.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gadilxcay.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnnmjwrou.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gttuywivg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjnfaypkg.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gumbquimo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gjaohtnja.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gcbglhlih.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gdhevphyk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gozcoozbs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gzlwssffl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gkfeoommc.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/grkywbulu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/goxmazxdm.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gnthrfzwk.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gciuldutm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gtpdzskuk.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnaoxdbtp.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gupsyqmuu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gcqyudpob.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gkkbpembw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/ggvncjgfg.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjzcviwbl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gdxxjzfxe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gyvwdyhep.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gqcnqpbfc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gdpymcjyw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gdmagfwcc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gglgdlsjx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/guouwkfbe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gkruasmzv.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gtdsjbvhd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gdfapdnbl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gimdnorem.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/geaxdwrmp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/ggjhpxfnl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gaymltpuc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gqsbbmssv.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gteeninwu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gtlmgloqd.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gkfltiohd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gvcodxnju.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gzzjnsqmm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gqmzbtwhi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/guebxmxto.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glydnzzjr.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gwnhqildi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gobfsrhiz.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gizmwqggb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/geulcreve.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/ghlvelyzc.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gyadonrgl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gdgyxumbq.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gbaxjcdjm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gkblhkzkm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gccwgdweh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gmbbcdnec.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gogunfgne.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gtkjrcyzb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gtwtjtpdx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gqvuykqfr.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gjnledkue.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gbtvcpqzh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gytmsptmo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gogtpdfxx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/grfkckyym.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gsnnyuneg.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gfouyikhk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glrdzwpun.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gredginov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/grgsfyarz.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gnvsspdvh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/geutcanid.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gdanrrdbx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gstuqnbjz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjnnqqoou.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gkahrwrxf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gyujpolrn.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gczygsehn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ggqypqxgn.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gbqypweoa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gpwwbpbja.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/guehgbbhk.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gzyxevhox.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gdxynchve.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/glfmqxejq.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/geuzotkin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gcajdyvbq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/glnzdvmkd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gsacowsgr.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gmtkkpscx.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gzziuioif.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ggskwedno.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/glkcyhght.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gfuzwftmz.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ghyxewvjc.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/ghqfpekni.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gtndoskvb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gxcwwaqno.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/glcdfizti.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtbipgmwi.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gpcikmbum.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gelpgjysy.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gabyqttqf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gmbafgcru.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gowfbniau.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcfxclsbc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gdoluwaky.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/glehgztqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/grfomyows.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gzgqgvarl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gyjggjdfb.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gxpsjsglf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/ginwjlqlo.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvrsuswkj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/ggmzqfgjz.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gocgjugdn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtnwjdjtt.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gctuphqit.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzqdpzudu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gqakfdnch.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcmdushhk.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/goiwynmdw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzowxcbtu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gawsokxlm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggwxqmcol.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/guinnprie.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gztqhdrth.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gyaaeudfc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gyfgqymbs.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gdgctjoxm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gpsqbpyef.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gpnpynfjk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gptbzdrfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gemgypykw.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gezckwefy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gihhlevvm.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/goglsrerj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gmpqnukeu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqoenujfk.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/ghuyxqnsx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giuhkvega.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/ghzsbwnvm.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gqkclhsjy.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gurejqobg.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gsjmbrwlv.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gilyrdkmx.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/genofpknd.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gjomkedez.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/grxiwzjbw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gxqeahfpe.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gredrrtpb.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/ggiubmcfl.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gbzrfuhmp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gobwtxwsl.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/grsywqekv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gmcqlscbn.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/grjjueyfc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gsqbmlgni.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gicvwcdhj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gluisicvs.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gjjzoznfq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqtbjrslp.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gjcyyvgfl.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gzplstfzd.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gztqrbybz.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gfsnpjjpm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gphuftrmd.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/giyfxntof.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gjskuskmo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gfzbpjwho.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gtceznvhu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gwyhqrxur.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/guifslbva.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gmtemqvgp.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gptjlavhg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gytobjrrm.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gfovqnhpr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gmmnkocgf.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gaysqmumm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gnasqgeeh.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gawqtkkga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gkhyptkyu.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqyrtquph.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gndcizfya.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gniyhvlcp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gjlfjffgx.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gysrhaiwl.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gdnihfvog.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gmvinxelz.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gfhjpibdb.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gasfnsubo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/ggwlnvzxu.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gvfelbxkb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gpkyhmnkz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gqhkoxchz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/guncsvbqh.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gsdmeliva.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gfgboecqt.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gemdxqjsc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gmmddqscq.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gjvjmgirl.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/guerzboqn.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gmqpvbpgp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/glhkusfnf.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gewwvdfex.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gyijpcrib.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gtfmsdxyj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gazbbgumi.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gbibcklmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gevyhgnwo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gicldwhya.sHtML


<!-- 参考信息 -->