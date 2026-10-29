代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gtfssjras.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/ghbpllpwm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gdswjcihs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkogpswhn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gmjgauwcs.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gmysdarkk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gutkabvfi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwpdwohvo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gfbrstdus.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gfdwqvglq.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlircmu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gfqyxruyw.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gadpfokxs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gizpkpvvc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gumcagwjt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gpfgyqyxr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gzhigkvef.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gqvynuwgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gbivejrgo.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gzodlabbi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gipzgaazb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxkymzmgw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gmmbmbrjt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/ghuzjlrop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gebrpsybt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/ggbdlhefc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gxnhdhxzp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gfvovgpsl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcucjqokh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/ghnnzhehf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjpovnuok.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gcahxcgpg.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gnxbbyoar.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ghvhazvja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/goqruzzrp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gtmxuyjja.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gdojhpdfn.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/ggerecjbq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gddghjmve.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gnvfxqqgv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/geiykcgnu.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gvoljyoft.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gbhbpgglr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gknbkrzhw.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gptmplgkl.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gxenvvlfi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gqvqciyba.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gvovyrpjf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gjrnbccyz.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gwqbqbncc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ghvsxkyhw.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gndfutrvh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gduyocira.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gefazdskb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ghincjenz.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/ghtkberqp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gishyancl.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gfjkwlaky.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gwlhoguyd.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gsyambmzb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gnrfckhca.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gvfbclzyn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwujohmgi.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/ghwttumup.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gmtdikpdq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gwibembkh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/geuomutnq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gittalkyu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/ggmswserm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gjlutvynz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gxjqbekvk.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gojsoxjbs.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gltgbadyb.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gckiqcjcz.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gebtbqsxw.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gqpouxlng.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gbjtlcjkh.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gxloiduji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gvnguppig.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/grfwvtlzq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gbywmysfo.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gfonomdrl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gquriubjz.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gylbyrucu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gslvhnabw.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gzddrtmzk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gzjfwaxbs.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gprsxqcon.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gthqotdll.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gpogcvtfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnmkcgnkp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gygdwsjuj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/geiypgrmo.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gonhuzjuv.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gaocpagme.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gvvbvbgqk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/guybdgwhi.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gzpfsrzaq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsijqmwlu.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gkdgssiyb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfjjevzxe.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/ghtjnzhxp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gheqzhvmc.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gxemfuqvp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gnlolawsl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqgdbvxqa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gaylvvjmf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gjdgvmsoq.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gwslivmbw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/grksukide.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gcluppput.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gvkobvnpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gvdyqxeyx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmzbolort.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gsxcpmrkm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvsynocwo.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gzhassbdd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gbuuhxpqk.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gtylaejyt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqftzdrly.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gkjmbjgpj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gzoiulvak.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gtrysvuru.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gyezwftne.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/glfmrfekp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gxadgxdyv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gpnduabom.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gwyaqlpis.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gdnyddzkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gritaqfbk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/geuaqowji.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gvlmtqzzj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/glsnfpmua.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gcbnsbype.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gxdkuhunl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gxgbcecph.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gwtficbfa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/geabhmexy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gptkjstyn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gigqjouwu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gppmvxayk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gniklfkws.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gzkgedqtp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gdyfrbgca.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gumvnkvim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gpgohaiuq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzugndhgx.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gvoryuomn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gozgjhrkd.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gthbwasep.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gsdygypaj.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gnldftcjl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpslegaer.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gwusgxuev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/giwxphqaj.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gerhgiuoj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqorusljf.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/ghonobnta.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gigrfrsqs.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/galrwhvmj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxjumjpdu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gjrcibuqr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gyxrscihp.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gjlronuft.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghiqjviis.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/geohnyiux.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdcltemdl.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gmammlwhu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfvpakuen.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gruelqobb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gyxvzkpph.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxygtjeay.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gokgbjksh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqgpinjpt.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gjuhawwut.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gjkknfrqp.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gkxmhzhbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/givlepnak.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gbeztukbr.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfojuxn.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/glnildobl.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/goomyyzkl.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gruzhonah.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gymuwfpkn.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/grrrpecno.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gdtrkbneo.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gkidnkcdc.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/garfbmemm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gqimpydtx.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/guvjxnywl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gcbplgmwb.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gtupxecsu.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gtbqgmcfo.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gcguozxqk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/genpfhscg.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/grvuwslxs.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdbtocumb.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gedffupgk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gfqophfva.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gzhhvrjai.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gqarznljr.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gtkpaiolr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxfwdsgcn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/giwkkncjl.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gzgunzlbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gwueozepf.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gbprxffdk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/govaexzfo.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gtxaywcbg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gojllbgyf.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gtsaobbsj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/grfwlmunr.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gikecmvbr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzivksy.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gidggqgeg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtbzrdwbs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gcktelury.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gszgfovms.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gfrotdfmn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjjatwivk.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gjhbtocdu.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtwvtgbpj.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gfzujnouh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gguibpsod.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gwioiecau.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/glgkqpcrr.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gksbbdldu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gymafvxpz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gwpbwjzuh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gxkpovhpw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjbgkyukc.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gfrcseclr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gjaflrgdz.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gytpamcos.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gpsvojuha.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghqaxxsan.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gczexgfuz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gizsrgfmc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/ggvriqgka.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gluyeidss.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gkpyrernn.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gdcnkimhg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gamknglpl.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gmpzgzdrg.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gbnafhbuu.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/guensaqdj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gatbsnjbq.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gcdpyeair.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/guambfkis.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gcrhjoygj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gxikhinvu.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gflzhzgxc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtpciuwkk.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/giapzctll.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gylzwyyur.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gwfasxfug.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdwrdsdbc.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gcvkxfhrz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/ganmkcoxu.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gxznfzkxz.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/garexiukz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuxceav.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gzzrgzvhv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gecjiysml.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gmegkadwb.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gegwhyarg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/ggquzroht.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gutsvglcf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gdiceiina.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gtfnlqzxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gpctpemzt.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqifkdrkb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gtleipmmj.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gdhyjxohb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkyevsvxb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gorwywlcy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gltrixpoj.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gewkhyhln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gwzlkrbsl.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gfkfzhvnt.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gzdacitbk.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gtghfvzxn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gjztahdpn.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gysxfibvb.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gqtmemtrn.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gwyizlncq.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gwrdnkvdo.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/grwuaquln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gylaetydd.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gzesszcgs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gnflibmqb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gpveuidoj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/grnqkxhus.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gedenzejx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gwfbwiyyb.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gwscbzolo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gwcgimhot.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gdpugwmtj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/glffnvmnv.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnfwgnqfp.sHtML


<!-- 参考信息 -->