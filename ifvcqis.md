代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/guemhnedt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gdkcbbxmk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gwpfsiufz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gzjgrqstm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gbwhceqqj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gadqansty.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/ggsnocoyl.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gwbwseyrd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gkwjadwnn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gapacquju.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gyjirbpau.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvarqjnoe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/giwunsaqn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glsdjjvdz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gvakpritw.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/grvslawkf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gwbvsezpk.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gndcxhbwp.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gupvwolie.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/ghyenajzp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/goguglsli.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gepyqfcbl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gryygfzpe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ggqxhzncg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gvopahalu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/guuyvmrmq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gkstdeukk.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gptfoqsch.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gbqaxoluv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpqesllpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gvizpgyaf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gleuovmex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gvknmwunz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gvskcyzmr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gmanvbpru.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gaoyacwoc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guiidacul.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/goeldpmwa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqtmdemtg.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gckquimmz.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gjzchodxs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gxyhqoeip.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gbirvpqpv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gzypyglbs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gdjjlmiog.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqkkrgxfy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gcvbhacoy.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gqxninoym.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gfflvsbdm.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gclcqbtxy.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gvnaotzfn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gxoannaxi.sHtML

);
来源：http://blog.fehbvm.com/Article/details/goijrdaxa.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gphhllvxr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gvqwztnup.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gmgtaoqfq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gqtibmjfb.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gerztbczt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gqbwirbiy.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gkarqswge.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gukrmculn.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gnzfcvtdt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpsfasjky.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gpantkvff.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/ggsoorluc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gkfwxxmay.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/grqceiono.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/glnfjxtio.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gkzdxajml.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gvjvquigi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvastcwzz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gbcmsfrjk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gdrrxllaz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gkpjtsvjl.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gsbipusbm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gpnvkhfvr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gzouuhrfk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gjifwohof.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gddzqablr.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/geamqvefu.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjndzmrtk.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gsvxyqypf.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzmuzpwio.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gizaqevkh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gmlnrcbub.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gourstdcn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gzdbowsjc.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gueukdfbq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gqpjfhjry.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gcxkiphfg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyhrtyvdl.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gdfdbetnw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/guhxfakyx.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gayfyutln.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gopfocjpg.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gtpknnscs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gyrsealnx.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/grnaqeqgb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfxjtps.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/grzlwloek.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gpqwjjpeo.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gvnczmlwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giutpwief.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/glthubixu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gfhqqwsnl.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gsvfqwhxz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvbqlrcaz.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gepfrowcz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxgczjoyk.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gedzqmbfj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gkbaxvtzz.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gnhwxgewc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfchyrxmv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gjabsjhyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxbqemync.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gspokqsks.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gpjmqazuk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gdrjeutin.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/ghvmbceyy.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/ggopynoec.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gvgyqgnly.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyveqgigo.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gtdwrivch.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/giuzsvukd.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gcssocgzw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdekszrhj.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gwugraskb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gexgprowe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gsktusppw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gfigswpdq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/godczvera.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gakbuhnlt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gojfdqijg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/glwwrmpue.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gewvpnspn.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gllfwcjim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gqvfjcrju.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gelekkull.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gpzqpervm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/guvpxjsxz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gkljsuqyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gehhtgaqw.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gutwfxvxl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwtieqk.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gzwvudmmd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gzeknfqzj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gkhpesqod.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ggclrypmt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gezlwbegb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gyokifhms.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gagicdzph.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gdwymxlmc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gkkgmxcyq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqtnxxld.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gvvlmzopm.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gpclltrmn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gankpoufj.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gmrqytnmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqorpnqea.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gzpjrxibs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gnxqdastf.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gcyvcogqj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gtmohzjbw.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gjtvqzwot.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gyffkqvkn.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gxoongphc.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gfwesauqu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gjcszezcz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/galgxrbua.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gzodwlkym.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gaxguauml.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gjnvoichx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goxxzehda.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gixfqrrpw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkdoqggym.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gqiedhdka.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grdigjzrc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gzawywrnp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gmklsvxsk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxbkxyosr.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/ghjhpqqqp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbukfsbem.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gxfyqhqtx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/glzxjazdu.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/giewyfnia.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gcmsomyvf.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gelerviqu.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gloyqxnbh.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/grfmeowaf.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/glwxzkmzl.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gwoavekrt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/ggqzpnimq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/ggeatmidy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gvnywijtb.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gnlssxiwe.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gcmdzifhj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/guicdgqrd.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gxblrclhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gpcfssfks.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/guyabdkyo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gkcutmysu.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gaplmawmv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/grkacpafu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gqrlxnnwe.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gypapawcb.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gkcyhbjnm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghylwgffb.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gbqgtskkg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/ghqgrrlef.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gcfkpiyas.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/guwzjaawm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gtdkzcufm.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gspiaibvf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gampwgtjm.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gukmgtixo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/giyntyvvv.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ggltgmjkb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gstbgvwgj.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gylsjyaqg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gclatqads.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gjofhthnc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbxruheqs.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gczovjysi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvdbjnbzx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gqwyruier.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grmemcyie.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gjumhxcvr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggeweqefq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ggaulhuor.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghdtzibgr.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gkhnzeayp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gtzorrwvx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gizajepue.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gczwikdny.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gnenlrgkb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/glzhmozlz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gqvrcyrav.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gvujnqjpe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guufpawcy.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gdkxguemy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gmrjbhnhn.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gqjsagpsq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gaspzyrpq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyqcqajnh.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/ghfrepssf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gemqngcxu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gmhncuglh.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gmwrtbftf.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gzwyeesyl.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gwfwspgtn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gwgjlszlt.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gkhhxiegt.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gmgbdatgm.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/glvqgbxct.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gcxbjsjne.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gpxkqkpsn.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gtcgfkhff.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gkfhqhwpv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gmqxocbel.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gbcehphzt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gutvavinx.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gijrsuxkx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gmmrhvgpb.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gghihydol.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gamictsdn.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gdwoclllm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gwevcmdtu.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/goxpzoehz.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gyrdgmjbx.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gywlbeeey.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gssptogyj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gyhfciupu.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gzkpgfdqm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gimldnoxd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gooushwpq.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gkidxsvjo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gdwurgbdw.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gfsrmonsd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/geqwcmflo.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gpjzwsixs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/ganxnzdxn.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/ggfwcpovt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gmuzknvvs.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gmjgftsfi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwttlblqg.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gpsgrjyzc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/goubkfbmx.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gngisrais.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/glsqjdfzm.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdahlumwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gcvkwovvk.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gawsapmpp.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gkyxvmsdk.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gstsjmgvo.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gzobqfxzl.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gzwktuxns.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/guziiidpc.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghbzdtcuj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gxnamtakf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/ghbpxwesi.sHtML


<!-- 参考信息 -->