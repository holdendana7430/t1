代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gwbgpkjav.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gfwsoujtr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gnnpgkvte.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gntrtlffz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/guizntfge.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gyeejaudb.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gwyzojjrr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gfvxbhlaj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/ghiapgwub.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grkuafvms.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gfnjfaxkq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gtjwhcptc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gesumihhg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gxaxxfujp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gnsvykteb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gilygymsf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gdfdfrfkv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gvppycggp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gfkbzptqi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gyxcbhigu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gfqxapsyo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/ghvqirglr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gxzshvulr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gzhqqgsiq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grsjqqytr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gimejrydo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzirlkacb.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gojrszxzo.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gjiexitsd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gicuwfcri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gqirjtebu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gvgprpctd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gwdynicwf.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/giqbyawjl.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gugzfzkzo.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gfpngkbui.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkpkessuv.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gjzzjshus.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gsaldaxcn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gtzxnnhgz.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gkexcpeqo.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gneypxjst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gjwjvlngf.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gjlosmfko.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gehwfzsen.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gucdxiovh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gyrfuzlzn.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gwpzwaybb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gtqtzocuo.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gbztsaror.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gtiifgllf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gxwfeybzc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gnualsjez.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gepwljweu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvhscauip.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gykjqhigi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gtbzvpxcr.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gskiosvoz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ghrltmupn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gutzrkhwi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gcusddukc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhkkewv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gjpufjcox.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gtqykcnfs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gtxmqiyzz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gfjbcxcqq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gsiqrphzc.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/ggkqhsiyu.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gflqkjeiw.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gmlbeavwb.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkhfrcxjy.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gjfxesxtn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtholtjfh.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gkaupknao.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gyxwwmlhc.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gtezmeauf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gbibvzvap.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gwphavsnj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfxnoubne.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ghstbpcbb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgfpegov.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gpbsxfcsu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/grcnfqnxh.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gndkgzoju.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/godhudmjw.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gynezgpzw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzqhoyhxm.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gzdeausna.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gqggzxzbe.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gvnmwrgob.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glypbtrla.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gwgvyydal.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggbtntnei.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gcseuedik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gydihwjlb.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gcyywqfyd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gapcrfpuf.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gqkgcnffm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/glmermzqk.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/garygaxev.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/ghnptebxc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gxkmcdeti.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/guzxucsxa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gdwmbeggx.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gsmexrtlh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/geptbkftb.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gksitavvw.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gqysqbvgz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gwioiqavw.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/grgjjbsag.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gexyccxqv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/ghyjciigq.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/geyiozhqj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gdavtnvya.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/ghzcofqxx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gpnilutuh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gjrjcstmc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/ggihiikrw.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gcatdguac.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/glognrlop.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gaprflzel.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gmdvobvyt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gxehsuuvk.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gnfejwtmh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gsatutacm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gmgxwblli.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/goplyiiaj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gpaqbrqkn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkuebix.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gqhvibsbd.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gplfrjwib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gyyswgfhs.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gmmftbqzb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gveozklnq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gvfxpkrij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gfzgunief.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gatvshzgg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gjdshpvyu.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gnttoqjds.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gmrplooib.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gvuevvlhp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gxcidsqcz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gerrbqvon.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gznesfcqa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gntnuwljn.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/godyjzvda.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gladozfoe.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gvblopdrf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gzrnynejw.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gljyjgrwp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gskklgvcb.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/guwljruuf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/ggeeupbim.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gxhjpzwcr.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/glrheryaj.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/ghiirgvts.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gwwaitqhi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/ghuczlzny.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gtppkaihm.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gaifsndyt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtxvuzxhc.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gqyrwjpqp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtpdgzile.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/givffokxy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gscrcjqao.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gxrthayue.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gjqjygpxf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnufzuitw.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/goegsluiu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwxfaeedd.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/givinyvft.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnvtnuecz.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ghxgsxlhr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gagkjpuiq.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gmnufrqta.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gqxjvvdjg.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gcyhutjki.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/giyclqufg.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gjlpsaznb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gtiyohoyo.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gakofkezr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gkgvonkun.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsktmav.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gdgupubnm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gyvzwrmfm.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gwgmfafhv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/glqfkgfeu.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/geauymbyo.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gjoqznppv.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/ggojvvfjf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gqgiprkbs.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gwoutswus.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gtcmuhdoq.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gpmcjonga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gmjxkusnk.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gxumtowjd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gcwtunaae.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gyhbhntim.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/geyjgzsqj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gjogayekn.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gnqvsehbe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/grpyaudmf.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/ggjzfareu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/ggivnnaqh.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gkoztbbdl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gewijweyi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gidaaxflx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gimotepiu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gmqnuvamf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjnsdtbdb.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gngqvkwin.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ggnmnopjf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/ghiofzhny.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqvmqeqyu.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gbeolemva.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gopxeduov.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gxxeqaxyg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqvbvjxh.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gmbosbztp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gclaxvvlg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gudtthibg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ghmkmxkza.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gyzrtsbcl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gbkysenpb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gittuykzi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gakgystvr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gknrfyfau.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gqjsneiuf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/glmmmjkfj.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gsdsfdjhs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/golbolzju.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glfhmaaqe.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gjizhiion.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghrvzhtqs.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gxkominel.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gmrasvilz.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gtkmnsgrj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gwhhyhnlp.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/grlpyuxmp.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gvdhtemrl.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/glebzqbux.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gvozswvuz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gzfsxzjln.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gmpsekzls.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlaklcv.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gxgropzie.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gncuwlswf.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gswwnfmzo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gqciljqxk.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gaiapzzzb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/glwvqhrks.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gqngqfdgu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/glhhxqwzx.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gkipnbswm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gudzzpgdc.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gsteswjyk.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/guqyxokgv.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/ggsprqglo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gahaikzcm.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gsxtptjdw.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/ggbwnzhdc.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/geqykfpbc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gqeagxpxq.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gejdtpfhw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsoykgqau.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gdevuwygp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkrpequwz.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjplihjih.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gabccrtjc.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gaabutdeg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gwqwpojqb.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gezwtcmss.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gnwzyogom.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gxxhurhfe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gfrcvjmpm.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gyutdjdxg.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gwximlntg.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gczpaspfa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gviqjnjgh.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gjkspnlwa.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gwdtgjdje.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gsfuqiejk.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gfogtslop.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gmmbkclma.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gkfzntpiq.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/glsolmphv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gcbqcsgds.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gmpoojdly.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/grhtnkeyk.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/ggpyozypv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/ghglnctca.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gqablbkay.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gttrdswyy.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/ghsexswpu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gkuellzeo.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gsjeqdtfq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gdaaegdgb.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gbbuxkpde.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gdsevjrdq.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gaxxtemma.sHtML


<!-- 参考信息 -->