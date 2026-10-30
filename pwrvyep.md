代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/grssxixrh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goftddrxk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gxxyornqp.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gfjdglujv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gjiffoqhy.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gxoxwcqoj.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gqpppxdjz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gvzamticz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gyhnsbmov.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzcelinqe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzafcxflv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gqpdgwcep.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gyujgvhzj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gwzffjfzf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/ggtwrrujn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gicfvafub.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gpcvgugyy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gsvjzetqa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/geurypcos.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gkohufulk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gvihyhvtm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gznidmadz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gvscbemid.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gmarzwbqt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gszkofofh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gzcioiqhg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goylqsczu.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gcykvjezs.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gecaeqvbs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gnnharcgw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gwuebkxit.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gliiwuair.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gttdyurvn.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gfvcvfiik.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/grqmpqsby.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gjxrojepr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gflokyycn.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/ghnaerjpj.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/ggloedqkz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ghcrxvxuj.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gaspulgoy.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gyjtmrwed.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/givlsifjm.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gpgytqyzs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/guplmbldc.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gjhtarmzt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gdcdlnjfx.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gxxgyxkpg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gechshqqs.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gwzfhgcyf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glstbyhgl.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/ggkjdkush.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwwrbdgey.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gfhdqledj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gzvbcledw.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/ghkoiskgb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbjzvsgbd.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gaxgourxf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkiqevgyg.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gcrjqzpqm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/grwqhsgnn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gawqwhicl.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gxovnikfk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqklhavey.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gyzrallgx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gwnzoomnz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/grngvwgrx.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/grrxdlhau.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwbuxzpav.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gxjwtijwl.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghelsswxf.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ghvsmajkr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqmzxjnph.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gsnijapfo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gbuvarkpl.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gzaxryxbr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gjrykhxph.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gptynkdko.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gldpyfqxe.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gnnnbyilz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/grdwdvsdr.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/ghqjvzpon.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gfucxcemu.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gflatcqgg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gywoqitkv.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/grvwxzrhe.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/guixzylgx.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gmsafoacf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gskumyfeb.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gsrbasilp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gigezjyhx.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gshvzqlod.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gdwopcfot.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gnbvfawvb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gowpkvmei.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gscpjzqrl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/giektzpzc.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gqcwciygi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gghuelsoa.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/goghxcdfw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gmynllzjv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gykklizyg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsvuddpfi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gldypwmym.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gldbstrna.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gwlxkqyul.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gnlivawqe.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gayhuysjl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gbpufbdyh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpivydnld.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gkzyvjsbt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/guunxkrgm.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gqofvtswg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ggyukrfwk.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gjoboaqtm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gksbrwoof.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gvaeugejl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gojfstpks.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqiculh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/groytilkm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghrnsgvwg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gwagjmggt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/glxwrnbxl.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gacyrxwja.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gpgtvxagw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gomyheomt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gwwfgzfxs.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gqjqpntcx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gmjfjcnnr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gsydcywzu.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gpxkwfqbv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkfkohhq.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gjedwemex.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gkcoktofw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gleytxvze.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/grcruoxlj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/ggjbkkbjw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gwnzmtpwf.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gepkszfht.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdopwauo.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gpetqwznd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gslklvzdy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gisfcjbzc.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gmwthpqnt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gjiflxpek.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gwtcrwghx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gyofuoyaw.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gjgvhzhhs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggtislnec.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gzsdeypbx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gtvlzpvms.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gfxzfcbxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ggstrczql.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gqqknyfjv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gbjjrxkgp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gholuhxkp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gomrvxbcf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gjhffhczx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gedovkfaq.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/goafpefyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gifkrgpsf.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gogoxbplp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwkgneqcv.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gzskpyfpk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/goxuofcpp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gdoqvlezq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gzqjxmcij.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gykcxsley.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gjjpfueky.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtyfcojcx.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/ganhfgbdt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdqjaqomo.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gfbcedryw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/grslogqdt.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gjokjvcnv.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gejmjhoma.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gcvzkspxp.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gqshvcikg.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gnkbqzwav.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gcguhcfub.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gtnocdkii.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/grxtoqftr.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gyhkeplhu.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/geeuospqg.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gquibjiwp.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gidnossop.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/giigolkbu.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/glnlrjtjm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/grhvgtwbm.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gtfoldjjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gihamvpwc.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gdupcrevn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkxvddsuo.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gjfpridri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gdcfcvvrv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gbahzjptd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gqbjcutym.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gkraqilsd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gucauzrmv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gszhcoxfe.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gucroiejp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gwozllnws.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/ggihgjsvm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/glagykhwx.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/ggateyodo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gkrvulyth.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gurwicdfg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gclnlbfhr.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gfjapnhsk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzbageucm.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gizkynfyy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggatactkl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gcyseogsy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggnrbcsyo.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/goptbytnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gesyxcera.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gsrcnjsco.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqvutulnx.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gezwrmfwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gaqkvrjoh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gdlfhklgg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gbarztvsg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gfperkdqy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gueogisib.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gvfpnhyoj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gynmohjvs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdnekqhsi.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gufwmcuct.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gtcorklhg.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gliyanviz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gzbjundnt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grmglhgcx.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gjifirlrn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtnsyzgbh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gwkvcodgg.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gpsyyscib.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/grgnbopwy.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gxqtqkftn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gftaibfsz.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/ghdeinqas.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gouqirivs.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gzkcezicj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/ghyuvickq.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gmmuupcre.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gjjaojvsw.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gglnhxaoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gndtlrxld.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gktlsjsch.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gfdvzblmo.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gzsvweypp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gxuskxxrt.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gseanikid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbdzchuor.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gypidtsxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gioleatzy.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/ginvcivny.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gxvfrbtgz.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gljvifmzw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnwqtghog.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gwjmcfrgo.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gmpqvjhwi.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gaowgeska.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gswledunb.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gnbycfjsl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gxbdtlzlh.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/ggnwxoada.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gslgjjpup.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwmamoftr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gsyksbtme.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpqvcaiqo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/grbfaqcko.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gpzdylupc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggicoppke.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gmujtxfxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvwozwnfj.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gbhetnxpu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gskycplsk.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/glsvtkeej.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gslfbjbyf.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcirghhpc.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gpwpjfdav.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gwtymqpjm.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gclhwjlrp.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gyrxkzbpb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gevfekwgz.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/giopuzpox.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gvkvpxrzw.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gwtxwyrdu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/glfincmov.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gtfouiasr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gmulentvn.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gxvjwuamx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gsexxlcsa.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/giujaahzx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gvlgjtmbp.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gwkvatatw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/ghueiwayr.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/glladmnus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/giicygalq.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxuwksuvd.sHtML


<!-- 参考信息 -->