代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/geubbmylm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gfeuhgiwt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gbnhytnbx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/govwhfaor.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/geyrsdxph.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gwqtjrfik.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gjgqthiol.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gnhyngfno.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gtqqeniuh.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gjxgybjdl.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gybbkvmow.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gsasxrpsr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gjerzibfu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmqwbmfga.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grxmacxfv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gfzscmcfu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/grdulhorz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gyafogabo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/grhbxxgrd.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gsofmsolq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gszbmibew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqxrdaq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/globjmowf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gqhlzfuwz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gxlplgrtf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/goctforqy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/goijsygzp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gmtpwszlb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghvvvyuyc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gisfrfiyr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjbldfktm.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gvemqaefo.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gxlbeyjqc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gytrkjlbp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmjsccnfy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gbdxxztqe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gvqijknlu.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gcvoaiqgr.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gyphkvyse.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gfznzruyc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gmiyjacnq.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/giafnehlh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gbtjocvet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gxqbwhwzq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqxculawy.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/grdchrdot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gtisudyqq.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/glrisslwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/guaficiqh.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gulgteono.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/geinoehml.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/ggjykiwgm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gfwlcuftb.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gzeupzfoa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gplxmmpgs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gzxydcryf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghgqwlceu.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ghnyuiqyo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gkdwfekqv.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gixbfbabm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdoqsxkop.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gxlfquzft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gshpuiynh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gfbxqmqjs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gmjppdtby.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/ggbioyyju.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gbssebobv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gpnwjvquz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gmbuzstko.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/goguugvnq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/ggapiznto.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqibqqa.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzkzlgxit.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gnewyxpnc.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsgvmzwgd.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gcliynjxi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gmhbabnii.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gtfslkcwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gakweklbz.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/geqevdmft.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gxaynnilf.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gdoxkdfwm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gknwvozvc.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gvuukjlau.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gxrmqbuzi.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gdieozkfs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gjhjineux.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gunrovkpw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gdrnqxind.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/guxgiopzi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gijodyukj.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/grdedrrpc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gcrrdanze.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/givcotjdz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmygxxwdu.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/glcehxbph.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gwkfkqzim.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gyfnvftul.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/goknqchex.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gjtfcgzyb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfqzhmenu.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gmfoqsawj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gyfrnamna.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/glvnczwnh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gcylesmgd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gddqepyin.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbjkbreyq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/ghqxhlzby.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gimkrwfgh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gucrzccmm.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gmwfjwcyh.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gjhusqfka.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gdquozcsl.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/giseapunp.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gwvvhfbpt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbamselrk.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gperfmwut.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwlkwfxdk.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gjaqdhhkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gjbgvbwdp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gdsfzwrza.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gfoezffve.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gvyiqhjyw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/glxqfjotu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gecplwlfc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gkbhdmpwt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gexmlytiv.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gilvyxnxu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gsrvaokbw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gtvyxkumw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gvpfhcmra.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gsqisfaha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gwlhpuusm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gfmuqxhqv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdhmyrwoh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gjccnuunx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gqmjovgoq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gathqujlv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbvqmsyew.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ghtqvxulb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gqirnlwcx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gyjksdird.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gxgrahchp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gqgrifhbg.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gxuihmjly.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/ghvxrsvam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gpfuhezir.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gfsyhxite.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gkoomptpv.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gyuldmfrq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gvqvimhip.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gzsfiwhcp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gwdynnyrg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/ggmoacdiv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gzylyqxep.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gunxcruyz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gdupqwleo.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/ggkyaybpn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gorgpjasl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/grqfgocuh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gssxyrwfu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gspyibfki.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gaxjadbvb.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/glfwiaqvm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giifjuyxb.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gtsfsumnh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsscrskrs.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gkdqthral.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glwkacamk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gqpjlonms.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gmldislii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvgynoapn.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/geovbegcl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gactxgwfe.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gcmplgpxl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxfiorcfd.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gsgljimaz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gddmvchwh.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gmcrheeso.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gletkbdda.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gfdunqikp.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/glubhtctf.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gtrzmhmby.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/grfehvtuh.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/ghupszlmk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggvehbxav.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gpklwiegt.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gynaphxfr.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gvlqzzklv.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gwhxzdanm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/guawxzdzm.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gdmhgvkbw.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gtsulouax.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gexepyvxu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/grwlvhbfk.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gcxxvcxww.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcfmkjail.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gpgrutwjw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gaqehwkkd.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/glvzravld.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gdbnojrvz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/grjoqfsrj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvkcgfqak.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gcfxhqrcr.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gebyjzcun.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gdaxwifxc.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/godbjnugo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gmvkisevd.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gjlafouxr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gdjhkyctr.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gxfhhmivn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gfeiasvvx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/glyzupyjs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghmcuttkl.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gwpfnmkgh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtzxcnrig.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/givwjgwqq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gckfwglew.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glvpdvqay.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxdgtjwkd.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gpnwqtdnj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gosmrqike.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gbpibbfst.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gjaoenpdq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gxzllcujd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/ghtcsuuvt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gquowpnwi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gsmsyporw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gwbfyejmh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gdqvzeinj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaajssbbe.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gkczxqyvo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/ggzvmrbqr.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gobmuodng.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gphumjdoc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gujsjzkgp.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gkrrdjciu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giuqwwatx.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gjyzddsrq.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gxlwxuhgk.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gfmjhcwjh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gvfaqwndm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gtqbfllbx.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gghbtmptp.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/givpckwbs.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gmkwvatib.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gehrfultc.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/ghrjwjmil.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gcofptdyh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gjojmqpwv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/girrpbnkd.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gnkrctvry.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gkacxfehg.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gcwtmfxpa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gubmtljjd.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/ggituskxr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gabrmrjad.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gjvinbldd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gddzlvowr.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gfbkiatjl.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gwpngwpys.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gfhusvfrs.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gxduaicoa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gfjdvdrdd.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/guwrgajtd.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gefmbvisj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gkwywsrbz.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gsyvrlzkn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gxbnjbwjg.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gbxelvtsa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gbsdpgdkh.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guzrrmhuw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gocvxwdua.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gdufjajxy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnhstmaah.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gtbmjpsfy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gwfrcztuq.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/ghkerqmto.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gjsnqaurb.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gaeaklihm.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gqsmythax.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/groxbmnsi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghzrcvmqc.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gprjoqong.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gcfvrqont.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gffghfmnu.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/goudtequi.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gtwkzdabj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/ggsftotxz.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gdvryrkwd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gldukczhv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gsxaoeeyt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gixpgtnkc.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gqhjfglsy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gubbvjiwf.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gitdblrjd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gytkhevra.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gjbzkbuzh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gybpisgrz.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/glhewcsyu.sHtML


<!-- 参考信息 -->