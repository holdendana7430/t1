代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtihuuhf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gnfkpjlua.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnctqujh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxniqkmj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gltfgtgig.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwlxcrjc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbprcpdzb.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gigsxnmgf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwzruxhf.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gactgnnua.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gewbosffi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbuzimnb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuwatofa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdcrvyowj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsixuzme.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqfrqktn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhnixmvf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/grutrhcio.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrkavrtp.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gxlknlggu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqppytwl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlojlseu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/glaqbswib.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gesrycnwg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/gxfshpzzp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gvimzpzho.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuaawzak.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gamcdmroi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyquddyp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbqmnrel.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscsheoth.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gulkhuzeo.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/glwrksuni.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gqbbwghbo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxlgmcnt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflzsvlhq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/ghusolalg.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlcyymol.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gqxdccekq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtbsvxzi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gfgqqvhcv.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxldxlcl.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gykanwipi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gnxiyxhly.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gvszceuet.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqliwzngo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbthpgxw.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/ggmecgznu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfdgtpbb.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gqksomkdo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzgvbvne.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmdslazu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihdcmogu.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhnwseyb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvzwxmes.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/grihtsajq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gexckncus.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gxugnnuac.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwcdixuv.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gpghliliq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gtoqhbdbd.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzcnclvd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gupadvmef.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxnlqxhl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gbcfuyryy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gijwpsepq.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gefpkwvax.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gfvfuoerc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyssjdpjp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gcbcdtwhc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwbbqal.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbofaxp.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gchlosxwr.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghczdlsul.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gotcyksas.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdplklydq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gadbseccy.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glboyftsi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbzeaclj.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gtncsqlsf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvsrvvet.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzcpvkjp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdungjakl.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtjwvntkp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gybxhmaiw.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gebqkluhf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gyppwxast.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/geukadknk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjpliyp.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gxsmcnnsk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshhknnws.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjduswqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjimftlr.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gxznaofkm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifiaqvzs.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gmntkwuii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkwwixlge.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gbuakivck.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunlyiaqm.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcwvice.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvzbmrneh.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrryfkzc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbswhvgs.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkhlgllph.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmhrjkmo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnminkyij.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdclcncv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gejfyncsz.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtkdeyew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjsladoi.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/grpvzzfjr.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gapahoium.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthuamgyw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyojoogu.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gseuerqgg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqspnneay.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gcjowceez.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gctrhbxgm.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtjohcqc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gevkgblsn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyukeozu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gejnjydrw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjklkxtnb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvlinyfd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/goirpohqh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjhirsrh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/glrhlwzyq.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuloxxbb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gyrschgcu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gokhcbalp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjakjxxmo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgphlqpw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gtcnsbeqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggcsaipsp.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasskbal.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gllocspqe.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctmrgjf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqbyhpwb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoeivfpz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeoyeaps.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjmuocjv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoayzwbh.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfiggewuy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gqgapklgo.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/giliwdizq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjnnvmjb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gtaelqblg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswfnhjjo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjiytbeo.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqtaqwsa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/grwzdjrhw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdjhmzs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/goqyfxwoe.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/grgimloni.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdleaakkb.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmnacrij.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxvyxobs.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcujftzmu.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gugvynhng.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gonhafgcx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqchyoqf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufzcfhou.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcgzncwl.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhdrogaa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqaqslpr.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxoewaie.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwablosey.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaxbftbz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnkvuviu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzgdukjy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohgwpavl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlqyxpzz.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/glbqtfsxh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwbvccdo.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjangbly.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gdoirtjcs.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmmdizqio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gawwarcko.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyucduvp.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqylmgah.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gofhcqsol.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsijqmktr.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gyxqyqdof.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gqabwuuek.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwpkhdlr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gezdhefyg.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcmuxwau.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbskykyoc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqgrjpu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzhhxdov.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwtpzyqx.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpjbhjw.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdnqxjzck.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gnnonwokg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gegiucxmk.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbdmmlqj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesdchgir.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/giuxhriui.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gqwrgjawv.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbnnyjal.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gnmlawjaf.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwawefov.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjuumqstj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gmiwtlofa.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/guxarlopt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzoknjqh.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gcibdqquf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/geifrvpjo.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdyuubyvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrtbufu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gredsgecf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/geakkyyiw.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnhvozs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gezqfjrqz.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdveboaey.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgzptkln.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmhymlrdw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcdniqxyt.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/grppoukpa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjexceudp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjuokgbl.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhmsjgkb.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzfsevlf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gjbiwueuy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxgdrayj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzulenbjm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkkluhya.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyunbojv.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ghxbnwhvm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gnybawxgr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrcjeavz.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwpvkqjkt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuathcot.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpebvkclj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goraunvwt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziwzprkn.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gshbhisbf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyoxudxj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gtgwtltnz.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwqrfrrd.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gojrkehfy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/giejjqpba.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnkwuixo.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/givamewug.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/genzeoxtu.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/graligzyq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebemnkq.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gqfykpdcj.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzqkyhjz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goinlnqse.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqwewku.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfwugtqg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gtegfmxiy.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/guzxapoja.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnssmnbz.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqxlsajec.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjfbclckt.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtlkmgwe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwzccmpw.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gelsqgjuv.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gbliyxulf.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslkicjsm.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpueatbu.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjridzivp.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gloebobnl.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gejnfnhyu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzbbwrvw.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdasejtag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geiuojbna.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/giymfcaor.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttrhklze.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/garakhmqh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdclkgyau.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gobwrdeug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmrdhbzd.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/glqentwti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzgsxzyfw.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gntnlmhmh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfccfaozg.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjozadhhl.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkvdqitu.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gsrxasdwa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/girkddrzw.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfstoalr.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylnjvnra.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhsefuow.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzqybsjsp.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeeylbww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeqdmsmx.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gozrsuygp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gorbouokl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjjconib.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjppdmyzi.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvnondt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/glpohmzth.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlfortwx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gvzrodole.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwrrejb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrnmxjyi.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyomdamu.sHtML


<!-- 参考信息 -->