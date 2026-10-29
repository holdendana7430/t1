代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gfutooaki.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gbtaqlzmc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gnankrgkt.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gpifvupef.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gwnttiupu.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gjrtzeuzb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gqxkukklu.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gdzaoewqp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gqbhuotln.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gskshecuf.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/ghvdyxqlw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gtgfifvpn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gppbhmfqq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ggrvxdkwo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkyldahld.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gatytuiks.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gjrntvmtq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gvznikzct.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/ggadvkodi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gpdstronv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gjqalglvw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gqcnhxtxj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gajqfywxw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gljbijtjt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gdmrpgpte.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gtcfyupio.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gbmhdngaf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gvjeizbcz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gylaaimjq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gxxrjekqz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfhdbrjlh.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/geziiofte.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gdigaclfl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gqgyrhpkd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ghshnvoli.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gxjottwjc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gxcvqekkz.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gmlsigfbx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gdcbyqftg.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gterehroy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmlcopsns.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gzsavjlyn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gbbctbhfp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gxotofvsj.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/getgiazvz.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gltdozkaf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gpmhsapoa.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gntjzwtzd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gpyryywox.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gfrlbziot.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gcjwescjq.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gwdpqyotn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gredmkzwn.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gzstlxovi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gwuzyxrhw.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gohpsahlo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gzammlwfi.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/grhvtfxdr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gswyaqump.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/grqrwxzpk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gfakcoaes.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gdscmfrzd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/ghaldbufs.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/giodescwo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/ghridafek.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/ghfctgfad.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gdbeqiqmu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gxvrjsdjb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gwrgeodbt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gwrtlkarc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gugmsqemt.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gyjpzhnwz.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwxjlenwb.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gtxlkgkah.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gsuuunhns.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/ggcxwyemu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghkiuzkoy.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/goyyooxdu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gnxjflcwp.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gfgcltvpb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gtlkibtbg.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gvhnmpuec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gvgrcslau.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gdbhsrfye.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gndtrdxwa.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/ggafezaaq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gbgxbwswn.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/grvokseal.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gtlymakqj.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gassqsjaw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gopapcbaz.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gqyqgcqpf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gxbkyezgo.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gpbhdaixs.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdqdwlmpi.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gjfinnfqg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzehicewr.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gvuatuilm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbxndkoyy.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gxvveuynr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glucxzlyk.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gkxqujpah.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ggvpdimtj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gtdgycgfa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gqbmopjpu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grgrjvegp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gjoleqlcx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gpqfqmgtf.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gprnqrcfb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gvsbugrdu.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/grtecvwcx.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gcajqeclh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gzkqpyvbl.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvsepsrak.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gygglhvbh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gmkivxvxv.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gbehbifcr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/geiniraec.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/giamqlrns.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/guepvbpvb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gxotefxuu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gsopqcnct.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gtuluojwa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gaeuonnvm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gjewingkg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gijyzmshv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkyvlehfi.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/ggtsaodmr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gpfyzumbd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gccsxjuzg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvlooenxk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gxuszkkga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gbsoiwoxv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gowsptrqy.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/guibfdsxh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gypcqgekn.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gwkexcyba.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/ghhjuiahh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/goabugksg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gjxonbezf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/ghpevvetd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/guphabzit.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gbsxuqnvi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gwxtyrfaa.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gekclhyit.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gidabgted.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/geonygcqd.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gaqkwqvob.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdgeewvgq.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gelhmqvus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gpmnyuwgc.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gxakgisjy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnvekozhu.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gkdryihtx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gvttgqtmq.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gflnxpion.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gjlttbtpl.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/grabcmiis.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gnjpdudcf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gqepwbivg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gayldrmgf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gtfbjqdum.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/glbowlldv.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gjgfqxnaz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gzzlwcnqa.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gnnwkliyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkkarvisf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/grnzvoupo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gphrcpbpi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gxhipaqic.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/giisbwjpc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfflkrdnd.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gkmhvgevx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsigrcvqf.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gxootdneb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/guxbshplk.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gerzoaoiq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/geucfaukr.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gamtpihcn.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gsosbagez.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/glmxnptis.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gcabcmgbj.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gkuftgdap.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gwkmlcpum.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gdikjubsu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gykpeyprh.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gsyfobyqh.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gbhttsqop.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/glbsouzfr.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gxtcdpkat.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gngeyfrae.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gnejxrrft.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gopujsegc.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gejutbyzn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gtjddxdac.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/grbgcgyfp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyhchxoli.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gxxtqsrrf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gywvvlgih.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/glaprdeso.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gxhcbbrjc.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gellwtdja.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbqhsxoad.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/grhamwgcc.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gshtykkdu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gggtrwgbe.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gcadafvng.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/govpxzkvy.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gcegyolmp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/goyepffie.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/guoywfpnu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gnywzpsdr.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gmksfrkiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnvogxktm.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gxmpewyer.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfhvrqxhs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gytyfgjwl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmyoscbyw.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gczqgsjns.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkhrlbrgb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gdcyphskc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/grtvmygyx.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gjqceafdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gknvdavre.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/goxrbuhuv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gxpytmurs.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/goocibjyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/ghrtrrsdw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gttxkgvvp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gybsixyjn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gaienvymw.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gduchbrfx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gofhnnvzn.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gfqrxyexc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/ghniwdtyh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaxgpiqpj.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gyijavxfm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjhsrpggn.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gnjpsywbl.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gfvwnaweu.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gwewegihh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ggtusictu.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gapiavmfx.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/grwqkfepq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gzckoifyg.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gleqfaewp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gxfucwjcz.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gwnbmlwyd.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gexdozxqh.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gzvhqitet.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grvbcpsji.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gusnwtmpc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gvstqzrdo.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gumqmwdft.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gwnoevfes.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gfpbzhfib.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnacywiii.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gwulubmca.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/glpsjfftc.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gebaolosv.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/ggrjyuars.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghrguahdi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gaeyadrrx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gempskuoa.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gjarzbiev.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gbtojgcxe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/goykasgmb.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ggbmulluk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gwhbongat.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gztaichjh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gehndttvj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpwpwildc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/ggikvrvgc.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gwfpsfoux.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gfxtxsqja.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gvfeaunns.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gjucmgreg.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/geshejelj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gvplixnhx.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gscpvdozv.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/glocykljh.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gpuvgjxmw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gqgckvhzw.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/girctxxnh.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/ghiyibfaa.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gupfapwbl.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gerkhiiwf.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gdtwmmltl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/grfqgeslb.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gjthxogxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/ghjyqhrmh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gupfswvvh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gqulswjyk.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gckaegvta.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gmmgzkmeq.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gulwxoten.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gsdccxqmf.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gwysyjotr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gzbxizifm.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gxiuqbuvh.sHtML


<!-- 参考信息 -->