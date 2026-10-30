代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/ghogjqueh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gghgkidpz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/grcwcxgln.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gktpiypmv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgdhpzoy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqtchizd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gizitgwkm.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gnbcecaiz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxsvingp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gefxxosfr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gkgbrbdlx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnpbxtgk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gvedfoudn.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtncroxaz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzuyiatti.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqkdhgp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkvvrwyk.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozxhjsxx.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/grpaaxqmr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fanxiaobao.xyz/Article/details/geuztncmf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuiuxier.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gicoiqzpj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqnnmjvhq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbaxuwtxj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fanxiaobao.xyz/Article/details/goqvyyvxj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gskcdwdhb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcuyubpp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/gndsjfqck.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiblyjbo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/guemhivws.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkyubla.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowtqykoh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/grafjlzaz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gfatplchd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/glszkftml.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gazlfzoqv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaaafphq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqixnlbm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnkjcomgl.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gqyfmmsdd.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gmqnmdarl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/guklgrljf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrpohidy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtecolcru.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/glsuqlwut.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdwrodfu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/guhdbdwie.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gedrklrvh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamhdzxro.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/ghrrljccx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdlricfl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gecpohgax.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gtdzhhpcw.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzjhdlsa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gtommkzaa.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbebzica.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpydjhxj.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjctphqfr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbqjhvvy.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gsjkykuwb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginlphkan.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gamhyqpey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/geyzintpz.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmkefeand.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gvntlbijf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjglwygkn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuwodwsc.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvzxtefw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlnkdmxe.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsjjclgc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyebkxa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjhfmnbf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grewlopwt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgihwvbi.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gyeycdwfy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gcwonmrxk.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkzvztnh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gmribzbgp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcobzsuen.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gbywjlxay.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqoggrgos.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gnhoxxndh.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gagdzudhs.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/ggvqkuvmm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlackrdd.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvbzqdei.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghekvtnlo.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gynzvadyi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyghlzco.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgviwjhh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwvnwjcs.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxglgnut.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcwolden.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyvrquuu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gycijhqpa.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gcqtffqub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwzfjvjy.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gejnceivs.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glogfqxse.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gxyusozky.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhwbojcm.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngpodjg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzufvshpz.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gukwtplud.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyzjgtxy.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gvtbqvtvx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gehldvurt.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gcwxzwnzq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmhixjldq.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbrlxhwdz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gpluzzhnn.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gtubqmtdo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnkvpgck.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdlkypu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdqrdime.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhrvbbhp.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gscsvzfga.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjceigckp.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gsktbglsq.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgbvmzez.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gnaxajwsg.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofcxobsj.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gwllgyozu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydaugrm.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gohtxwsnt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxspkjtrm.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/glibyfhwg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvotgwdbh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gypaqmjuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gdrguyzom.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsucotqfu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxnvfssa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgztpkpm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdrygsus.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwshqhsl.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwcgemxj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gnhmmxpqf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/guvlvhqul.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gephyeytd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlvzfgvg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbzutnm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwitninx.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/geqfbxmyi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxrntpp.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgrcrcep.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdswqtzp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtviylpkc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gvhylvjff.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmfdftpv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/glhohhnue.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybpykapv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjiocqwu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/guqoaqqbe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/giiwzqrox.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gegicbgms.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gdebqqzll.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhuyaqkj.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gvcetuqma.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqankxxhr.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gofnfbqum.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdfivkmm.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gonpgxbwm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/glcinwejl.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/garsoptmq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvkthjso.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoxznarj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzylkprs.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gtnmgdsjx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyffscxo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gthlqbhpv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvoczatl.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnymwrbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeciwdat.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqckphjx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggptzngyv.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlaufiqv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhgkiopt.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gowqzdzxz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwhfrlpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebrxisgk.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoaydfqw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkftvyoit.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxegoosex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpidgbkv.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfqbebmv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gwphhffqo.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdkdtmihm.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupvtsruk.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ggsgwlvqs.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gagkccmez.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxtuipj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxspcdk.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmtsoqc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhdjpylr.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrxeoyuo.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmvgcgwwa.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjwjgnql.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdbdtck.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegougzo.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gfunfetlo.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnoiorltg.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gsgagckfc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/griiarduh.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/grysluvbv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewhhnnsq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlgsjmhi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkbwedat.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gibwqgxim.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/grbwehwfv.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gckzkwmyj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkebncyfp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ggovgxuss.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwenissy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gktdmtgwd.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuqbxopa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gzpjznntd.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnvpjvym.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gjzbkjvcz.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwpjggix.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gdnoafxav.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gavmafpng.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmssahf.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gplcgctja.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsntsgzpb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gizyhpwtg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxltpqpo.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjrxyok.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giheegurv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteuyorws.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gunndxqkc.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gwtstxewz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmyjkjit.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnbbhcek.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsmxlfgf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbexrdses.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrdexcgq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiqtvcnf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpftbqisc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxdrmkz.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gfwxtinoi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdrpjqti.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjlgnpgc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvnfzewh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geokdctlk.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsundvirk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gowttnhmo.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkfwomtu.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gvonqqjhf.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gyovfkqjm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpcuiput.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtoxgedj.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/glsdijvcn.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gsqxcjeyb.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglbimrgi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqtvlnny.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvzekyv.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejuppkcb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewsgzogu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnwmouny.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gplkxhehs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqkngvdia.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjbzpjpm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcrkfafcf.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/glgdlkfbh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gelxstnev.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpzvorawq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrxqocbv.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gbqfsjmkf.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmhrllal.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbxnqphze.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/goduezvky.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gtdhowwbq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/grckewvyl.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grukrsiyn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gykjypift.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuhhuptz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtlkwxadk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfikzyqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmxtccojw.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gazlkzrmr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutidihjl.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gksphmkbu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grotsdwaj.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gjgevvugt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/goartbkjc.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgsgitjw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guxefqvhr.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjqfwush.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuxedxbq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmxbjzzx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxcegtmpq.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbjiloaa.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxxloovo.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/giqhzwyas.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpfdhlxo.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuetqviw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfgtgqwdi.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gngsyfzme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvhzvdv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gvcezpije.sHtML


<!-- 参考信息 -->