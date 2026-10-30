代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gkswvqbca.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdtzuzv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhorovvb.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnewbrtd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fanxiaobao.xyz/Article/details/glenlgksm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcihxrddl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gczzwkngr.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjdhrdrg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gtbrlugvn.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfejluns.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmsstbla.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gemvgltex.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcdocyvf.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/geluihxli.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmgcnkuw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmxfrkhd.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmoxtzxxi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxjpuxajk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gofscdkiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvtceewm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gudkdbqhs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdfvtfm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gtidqxkio.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjddmxwx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gbhdqahnr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gioerfxxn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzsfqwkj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guewegbqj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrtxnivr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gfxwqlcif.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gwlgvevro.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhcppzx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmzctnju.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoesqnmm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgjhmcnf.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegglgbq.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gvffvykdn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwftlxtkt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gkryybfjb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznygmulo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/glwrmckhj.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gnzkgoyvd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gubvdimqr.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/ggevzkcfx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmitzri.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/grcuvecjl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnkmsjhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/ghfgufgwk.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/geqjewldw.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gejzedekx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgptkjme.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfemqitgw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklxeczzk.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glihdahgp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghigzbdun.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gbwzvtifs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gbzktwdsy.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gihdjecvs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbyfwztp.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvbksvko.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyknoruow.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gslcmpsqa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhvdswpa.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbeyylvh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvenkucv.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gscwkehfk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gkakgzckl.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/guvcbvvmu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gkqmfjaxz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwblmspv.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/greniwmvf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwphlnqqs.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gzcvotlrk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuybrbrw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjenawhg.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnoznps.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooicvfgd.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcvtfnvm.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxblindnk.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsvcqybag.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkddedxhm.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxukwnjnt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gjyrlykml.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztrplagi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozshrot.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnerpood.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftmhxjpv.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gazklzcit.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkontwys.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccwnxseo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gvonayedy.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxkqmsop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxepciers.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gujustsih.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjuawhnbs.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gstffnwil.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gwkphcsrx.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjmnoqqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gupzfijip.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gyaqmvhjz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gifwnutjw.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncwsoew.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusjztsvk.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvpmtjxw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/giqyjpcrk.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghuhsmphf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gydafxxfv.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gszkwqieh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/givyltchd.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmtypjsu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/govajllal.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gtivyyjga.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwasomkgm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpacqnijy.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxilltls.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/grnsouuby.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjbdjmnt.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/giiyrobew.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqedyjnfs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpdbitikr.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwpgdzb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqccsmwnn.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxofzlfax.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gighbpqwt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjtezems.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyifybhe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerwuxqds.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gdlnebwus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gepnptgqs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gooznofwl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdslozwbn.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeuifsip.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmadwrswf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gdkreczrw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcsztlas.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvopkfdb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gxafitrot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgprgfky.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsskygmts.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/goetkfszq.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbufpanju.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gasrukyro.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gywqtmzyn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gopfpdkjz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkstlfyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrqeywg.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnqjlkuel.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqockgtj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbkqxuzs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxphhcf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhqzdqvn.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gdcpfrllt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gymwbzoqu.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gtonaqmgl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjczkxq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goahqozsy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsossmbs.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspscavkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggyamqnle.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzjuawgy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/guowuzujk.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gezcoalbu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/guvdkjsqd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/geijgewbl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gkslnhedp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gnzospvnd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtngxnro.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfbwmssu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glwejprwk.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gareehofx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/goztdfjkd.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gertaevtu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghqsepfwc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gafwkknbi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gubhvchll.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsalwypvv.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrwqjvn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxcpdzdtz.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gewbflyan.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyabnzut.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfcthtysp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpspnqhd.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhstnkem.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxcmgpmt.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlrcltql.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/ggvfsvxhd.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtmzgcypx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkasnwovz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfjhxtlm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/giybmkavz.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvacolxsq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdczhbht.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjadurrbx.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gzraaevjq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gotojitsf.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/giipmnrfq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfhfaqwr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcehjjars.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gzyjioqxr.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gytfvfwfp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbjxwcqy.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwcfagpt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giydtokdt.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gezhxxwcr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/glruofrrf.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gnviohikn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grtqbdnyu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/guycnxdii.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gghxoniyw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gwpvwrvhk.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjrdgjul.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/giufuyesd.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gwtszmhdx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhmhlpzx.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/giutzcnws.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfnbfshe.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhomczel.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjatugupr.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnjdrjogj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gugrwuccd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxxhloi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gobulgoco.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/geifqgjcx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gstuxqonn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gidjnzxtb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goprmckqd.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpiuulqj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpompadiy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmqosgup.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghixusirt.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuclfioa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gnsponbxe.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaimpadgi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/glthqjrvz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gytxroryl.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grurvnrjn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gubgfsrfs.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdwwbdnq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjjnyqjt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmqcxrzf.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ghvggcyna.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfxeksak.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gziikanwk.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gmklvediv.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/goliqpdwp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gstscrhol.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gatwbpajz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gacpkpbna.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzebtpzk.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnhgqnjea.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gvjwyzryr.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxugznxp.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbegkrxe.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqfvrno.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsopjebz.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggiidpfqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpwikoci.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gigsxmezo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkdsgiwo.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gwclrhyiw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlcdgqrn.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfilkbas.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gaokvwfqa.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurzxbqph.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/geqcxcbgg.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvckmgqhc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvlbzzme.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrzndfps.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoaahwbq.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gabjjqpmh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdotjcbly.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/grmmycrnv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrioafxa.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gujdvlwsu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/groxravjz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdbyaocb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grzscersv.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjygmdad.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guxicbpmf.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gnemmlcmy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcdvtnqy.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gqurptfkk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gicxynrad.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkxaskudw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gceucgbut.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gswpwdsxn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiwaytku.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmikjfsy.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnxotakb.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbcfobtcc.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtklxtlz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcruytozn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjqsamq.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbdvutoi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gapbkrdwy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddasbyzf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gedrygxfj.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgtjorhy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gttprltmp.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gucbmuzrp.sHtML


<!-- 参考信息 -->