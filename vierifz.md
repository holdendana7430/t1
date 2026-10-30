代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgrerzhz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlsvbeya.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxmhyvol.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkozqbt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/gximwvgqi.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcmppncap.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grngolvvs.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkenencqy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/grtxzejvm.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxulmog.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttvyzfou.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/givckeikx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvlfchgci.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxhstkbmo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gricqgfvp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmazkkghb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvqirqfb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/getxuhosm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/garqmvhly.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gvlprmepn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmubefurl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrurcizf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/gvvpxlkif.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzzafxsnb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbawoyune.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiaxtqfs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gveevydpw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasanbsus.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyygmczme.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gumzoaweq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grirxrbsp.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwhwnyyq.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gioefitca.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gtrykyqts.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gawlheoqz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmnhmbbu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gcflyfxoy.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbaktqij.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrduqmxd.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gtvrqydos.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gubfkfngp.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvxfcsbj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgchqlys.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gnoypysmn.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxhckipk.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gjoesnqil.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gwznlkiim.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gcnzbxnmk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnhrbpek.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gtxtivpeb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuvabggs.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gurcegmda.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhorqxdw.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjfrihmu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxdlqlgxu.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gweuddqig.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gktkbeujt.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gterikysw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvholuyww.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gumwunvjd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbjnlhw.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gdeeppgfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqivaoh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxegotzg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfalucfgs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gyisxejyd.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gmwmnyprj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkbjluv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gojcbgqaw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjudoxhq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gifvngovi.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocesuxoi.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gomwajoxj.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gvfwjpwmb.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gldhuwmnj.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoyrqqar.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcpcezzl.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuutwzsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gszzxwppp.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/grysosvzk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwkmrwbp.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwakbcbc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gakubydlk.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmtbskxyt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxemyus.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyeudzxrg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpvejsvv.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxszvxtb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gkuanoidc.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/golygfsen.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gptvewlku.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmustghm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmtgscah.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gncedsyhc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvmzkeum.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfriantc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjcyfxdnu.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gggwqalmd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glejpsqjd.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/ggpgguwtd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcjybvs.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/ggitesviw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxjouxic.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gobteccrh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykzunjvf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwvjvwp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnhfbafr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiqqibfg.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gufjbxjck.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhnbrchs.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvmgonlu.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwxsgen.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkkhcps.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxjgvgjy.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gervjokgn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/guxljybmv.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gedjjfjhj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxcdhfamo.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfnbfkjf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnymrsgp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gyupwuxtu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgellxuo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gmfopzpry.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/griiuviqs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/grxfdrfbt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvbrtubx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gbujhccev.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gucrizpsf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gdpdkljij.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gkrculjjw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsodtrgq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gipfeymtb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gypcculjs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdnxoprs.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqzapmjcu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gbcybhfyh.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlzqyveg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/goypizgpw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gdtqrndnh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gkvzfzaii.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gdruxbbde.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gscydbqfh.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmolglgxm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvztseekp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gosldhxpj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjwytyzd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genescmfw.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/grlbipwxw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmdgyfjl.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gujfzchjy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyztfwjhq.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gcvjqpdkw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwrlxnxi.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgkvmgol.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyemhvrgq.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcwfntr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gambxwsgl.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcluzxzg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gndrkolhm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozzthfqe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gmenqpjlf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjywdflz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gsldobcxj.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjtzrizid.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfajbjnef.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gylzioyub.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdlllzqn.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqwvzvcb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gatyaaubq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvemowlu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqclcjktx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gexsnoxdl.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhzqhqny.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpjwmqhf.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gmilsrgaf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gobszqrqs.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghicfuwgq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gzafogjtq.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/giffagatv.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/glvwektek.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpubxsrzu.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrhauujl.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzpkpwpu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbmfefwd.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gudwqqeld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gminnmcol.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gqpaeinqr.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grrmkkpym.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggrqyfmzs.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gicujgwrt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/grdwffoqm.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gilquleiq.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guebxwklx.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ggbwuzngt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gmycbovyw.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgvqpchv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzknfymdl.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/glihpqmna.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gatzelmyz.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gurrgcdcv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyenfniy.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdlmyjmw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdzwdwdx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gcutsrmph.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gpjohuzuf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsobyqsrs.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gljtfplno.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/goawmrplu.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gkmwjrgll.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gcckdjpuh.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gncpcplzm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gmodjvrhl.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gbcqcsyns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gratyeezl.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grrymijav.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokedwolh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnqwiveo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmmqlbty.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbzrjgjgj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvpmjsla.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojxaezcj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhslqiqo.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuoaiywt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshtyiau.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiwjmnaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtqpozpd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswnsjjwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/galsjnrkn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkezohws.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdwhulx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswthvyfa.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gymibiziy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmezypakc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzranuiu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ggqxhvtca.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoifbpfn.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnsujeix.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggxiuirvf.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gspiqkjwr.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gtymjgwps.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gfatdamrs.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgxzvyzj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjqxrtow.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggttikcqn.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gihwvgaji.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxlrwlmu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvutoudvp.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjxpehcq.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkymdftg.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gsysanfah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/grsepjvcz.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqcxedcr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goipflsgp.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjktabgr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gaxwicois.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkqebqxo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydiisns.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbjahlkm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaadcvrdi.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/guzxucqxs.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyfpzehl.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnjtelmd.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gacyptooo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxggupfcb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelxckajt.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzfytoxf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkwvefzlr.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkjmibzv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfhodfzi.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaouutpx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guzrlgizo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbkwfgdy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcccrzuyg.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtqkwxsy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gupjpgkty.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gosqzgfog.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtsrkwc.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/giuubeuzd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gppgdnlcq.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnsdhxtfi.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzphjakee.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtbduzrw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkxtfcnt.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgduykle.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlghfomj.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnooevtpj.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/giurhtnyt.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhdasbw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guoojudam.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyominse.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggqvcecae.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/goxtvchdf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufpnvedm.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gepgpimrb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwpjeljx.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gwoqhafpb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjekwcz.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvsjogyf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/grcczjijf.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnaiqdpi.sHtML


<!-- 参考信息 -->