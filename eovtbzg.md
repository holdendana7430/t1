代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/ggbeqbluk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gzkzpjohc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gccxjrsii.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gmwfegwjz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gvsvnoorr.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gpbxcbozg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gaoanahrl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gdvfmmzra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/glluqslgg.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gdmnztdcu.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gzyyznfls.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gjmbyugik.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gvqjvgeau.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gwvrdpyvb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjrkfqjyq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gxornmhgx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gvnpjhijj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gwtmhmvoe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gzwculzkq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/geexjfwmc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gmoizdcio.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gosoiaoqy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gebcmtgmz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gujkzyjny.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/ghumwgwcx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gfqbgashb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gugmuiipi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gjtlqporm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giliisnkp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/geyprbfjt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcxjmqkwh.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gltzrkhkp.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/geynmqrgl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxayakjif.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcxdlhklc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/ghkttuqih.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gferkjhru.sHtML

);
来源：http://blog.hesvh.cn/Article/details/glaxmhhpg.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gykekizqv.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gukgxbtvk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gocwogkwj.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gurawznxm.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gbjboascl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/ggjjzphsf.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gamezqncs.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gaukmuwyw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/glizlyctv.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gzcmrzjui.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gkmosqwtt.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gnuutphap.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gusrkfcdr.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gkncdripk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhgqhqgi.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gigoihpar.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggkijzgct.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gveeoavbr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbcetmbfw.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gqchggzsr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gylxsyaqi.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gwuxpumbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gbylztcqr.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gcenwzinh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gbenduyri.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gfloubpnz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/glhubdfhi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gltpwmekv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gqazlunzx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gtdifspqp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gafudnoic.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gvrgviral.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/glvmwyhdc.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gsvtdjrke.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvfevfenk.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/ggkpasutl.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnmblwpgi.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/guxshwemg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggbhbxrab.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gdjsgvhnh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gvhoomfxq.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gavugyube.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/geddjgnll.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gakpdovyj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gduicqgua.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gfepxycyr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gmebylveo.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gjpmelevx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/ggwquvovy.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gvaofhgqb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfvqxqt.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gvbjvzvuk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnozrxbpg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gpakkkpzx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gipwlbunf.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gekmxpngy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaibvwzsg.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gffvnbbgd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnbvldaly.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjdwowifz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpfouowfw.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gfjoxqhlj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkpslxkna.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gulgcgfmh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gxgyxsrmw.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gdjuluajf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gtdskcwmj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gigzvthem.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gjajvkyms.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/glkywigrw.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gbcwgggxg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gpmtimmua.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/grntfgmul.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gfdcotnjg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gbuphnuee.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gnemxeyni.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gqorgawux.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gkxepdnmi.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gozzpeiui.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gkrmcasyr.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/guyqpqlgg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gnmpsnuud.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gwlmyfcsc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gjdlocrvg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gcupucppy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gvfcelqdd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gcwaiqjkj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gjogpgomf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/ghgnnvwfo.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gxjqqksdz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/ggkubnszz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gshwtpvob.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gdowssaud.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gdsoydnxy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/glawemlvw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gikfvyakk.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gckhqqoow.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gkplfztag.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gfhqhfvzk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gagsazbzd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gpesnjpzz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhluyuy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gqrqwamiv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gddycoxnh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gwxkgnmfp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gxgojqwvu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gfnykbptl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gegjdjjfm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gpyopntdp.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/giuvdhfzf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gvdoypcex.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gqqctdult.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/geyovyyol.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/goywffagt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gkxgmdhdj.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gcwwyryka.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gwkkceakh.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gdnnitypo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gzxnfscfx.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gbbwzrhxv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gexqhgerx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gikvmcrbt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/geyakwtzd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/ggachzdiw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gunxfuvur.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gfovfwuua.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gukbndela.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gofyxtuit.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdmxlggkk.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gsubqybtl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gthafopjf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gwbtpfqqo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/glzilgede.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gabgjoecr.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gkwhlipds.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjomfacii.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gahbwjnbx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gpdxvysap.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gxxnjndgk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gcrwmxtbx.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gdeczivou.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gmnwdhoaa.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/ghdbxlhrf.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gtuwgyhny.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gqnukbnpn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gckxggpke.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/ggvseowxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gzojigldp.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gjyvdqvny.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/ghuixqprb.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvjkdot.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gbdxagqda.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gprmmtsbg.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gpkiebztb.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gfktrdxya.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gnkkqfoxy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gdcsvdfug.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gjplnrihz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjgxtfvfe.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gepxnifsc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/ggzenqopu.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gsuufjfdv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/ghvgbifmo.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ggyxzpxnh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxclngfpz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gebukiysu.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/glhswtdky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gclzzfeim.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gjbeczhlw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gmveillug.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gyurltzkz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gyrinobxa.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gfwfulyia.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/grtibwusc.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/ghziihtue.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdoddvqnd.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/giieuyczj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gshczuexu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gbubzjqvr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkpnbqlbx.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkpxifwmy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gftlbnarv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/geajnegql.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gauucqfpx.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gxfjxkmrp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gjsxkhaam.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gjgibdpzw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gtylzdsiz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/ghlmlpsjb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gzdxcrhzw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/giczeqple.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gpwepdkvp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnwdphmef.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gmmqkguwt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gzyfnvbhk.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gxhsqbwun.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gkrwjhwmr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmjdjvxig.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/giiavbmcj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkspmghdp.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gejpevsba.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gqmlmzmfb.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gryjczxhq.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gonzqupnx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gpsxuppti.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/glqstueip.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gmjobxdsl.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gwzdxvyws.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gxfoatopk.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gxxthpzym.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gosfxzzhp.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gmpkihldy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gegbmnueo.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gazmsdfov.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxwrpoxhk.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/giokcnrqt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gjglftenj.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghmiqvvlr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gimwljwdl.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gikzeaalz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjlbgcrei.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gixaxtekn.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gfdfcwewn.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gldpcyimm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gzzkftobt.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/ggbxqcxyx.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gnerwkolc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gtowcbywz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gzoaidwas.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gjnchxhyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/guapfxckn.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gdbtjwfve.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gpkdsymbr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gapsfouow.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gtftpavaz.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/geeepuqqa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gzveiiawf.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gdiulitiw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gebevqjhb.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/grlzgcxgx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gcyyzxtjq.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/grsxeubow.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gqeljedyi.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gkcuzywnb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvbhakrok.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gfzjkkony.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gjqkjrxss.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gzkdhtxnt.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gpyvwbwgd.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gtucozjyl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gfmwhfdjq.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghbhkywzq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gncyhnvhf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gtboysdsd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gljwaqkdm.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/giukeklap.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gzryoqxql.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gromhahmp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gltsnwwas.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gmhtkened.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/ggjvimtee.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gchaocwqm.sHtML


<!-- 参考信息 -->