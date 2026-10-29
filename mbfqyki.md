代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/ghunryhwl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/guocasjvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gmvvdocec.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gnuejhyct.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gmuesokon.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gxzgflcyt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gxkcljgsm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gylopzqnz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/grcgzkbjb.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gwhnlerdr.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gaxchrjni.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gjtmybzav.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/goaoxcqvu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gdonwdumo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gkzzxelha.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gxwqcolvv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/ggxemvotq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/glrzftrep.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gavbdsrba.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gzkaneeup.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/glarmcrir.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/guvbopmli.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gjuohcjgj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/giidmcltq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gypwzhxjy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gmfckgjqr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gfgpwlxgb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/ghqtaznho.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwvxxcniu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gpteflthg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmipgmlfc.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/goklrmpew.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gekdipfgz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gtqjqazyq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gpaeqoirz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gxiusyxuc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ghhvyaytf.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gyhrblgoa.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gykksdbdd.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/giahvkgoi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gpeecprog.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gwxzdjwoj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/ghhbeumjy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gnmjkyogk.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gamrbfugv.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gqzrmmelx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gulclkwhv.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gqnlyyswi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gveywyqes.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gbzhapfvk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gurbqgsas.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gigfchvek.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gevzdaduk.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gmczcbqjf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gwkfahzyx.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gkvmnkqcc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gzfnghynw.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/grpkgifxu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gebkiopmh.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/geecaptty.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gejlifqcn.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gbaqnysdc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gtmcimnjs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/goikhoofg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gryxbvlqd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gxjwfvotd.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gyyeygila.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkbtvrsdz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/glkjdghzs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gnmpstylf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gbgnuhant.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gdkqmxmsr.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghwcdqssy.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gcxzuhnay.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glgdlybfd.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gzztvmobu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gocuzbhsm.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gmnfuyxqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gbtgjzzfd.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gglcjufva.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gztssyjlv.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gdpsggjqg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/guzzgorjo.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gxmjtjgtx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gqsswskcy.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gdtjxndak.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gxzesiosy.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gnanergma.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gowpacohs.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gpjkchbvu.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxgkxsxeo.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ggkmcsswo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/ghyrenpkd.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gcaioakpy.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtxadqnhj.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gyoztcaln.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/guogmxfdh.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gqfpopfcd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqnckwgpw.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gckcenkhm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxdbyhpow.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/glgeodrza.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gkvfofpye.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gmrujubkt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/giwdupjws.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gymmvkxyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxwdytvfe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gmksnoabt.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gbyomaawg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gkdkdlzpv.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gbcsiyybs.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gnxyipekc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gfpyrkzyn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gafjwazoi.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gxjjrjvow.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gzyezhiwz.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gnnjfzftp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gzvlqundr.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/girmnlcii.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gaphlidxl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gpkaimcis.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/girkbqhog.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gtyygyhfp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gcvbinyzx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gdgyxohld.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/grjffwcdo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gwgdqxlgy.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gtoumrzpb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gatlhyyxw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/ghpgjherc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gbalbemqc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gocmcroxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gxhkltdre.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gxovfefvy.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gvlexhhia.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/ghwyuayuo.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gvumldtng.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/goueqylvf.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gkmjfbhwl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqsoypook.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/ggjsztkwd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/ghqrrwobs.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gfecowfzz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/ggzijtibd.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gljfjtsab.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gvzcujvhc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gnszisiml.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gpljyzdhn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gnpmacqrx.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/ggzkjadye.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/glaokgpdb.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gmqmqmexo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/godlmuyrl.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gvulygokn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gwupfohjn.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gcauwpkkh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gpgjjvibx.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gxwloraua.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gkbstvqvr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gaohcobhr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gdainftuo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gtudroxlf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gkragasik.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gqyezwucc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goaxrxgyl.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gbvkkcddt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtzrhwhek.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdfaccz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsyqytugi.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gkjpcqxho.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gbhgjrcjv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvxljaqrl.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gzjwtlhtt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gesvtuekt.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gzgpmhlkg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gtedodidy.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gajgyjvlp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gexbavnnt.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gszmceasm.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gpyuytxjq.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gpdpkdpmm.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gexqanbke.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gaqowbhvf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gtuzfoplq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gladyqmcm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/guoswomuy.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gslkizdqv.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/glogdjpzh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gbhpaslzy.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gvwysbrjc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gejmysizb.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gugrhqswz.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/goddxssno.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gtlvvtluo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gqjpzoqnb.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gdqqtxkid.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpvijcdkn.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gwejefsai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfyrilcky.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/ggwqouwxi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/golbxhjjl.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/grnqthipl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyykifyrl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gubtuvxjm.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gsoobrvki.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gnbngjztz.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gfbbphvre.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gmdlvrtxz.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gagutenvz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/ggralxela.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gandsurkd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gkayvgzft.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gvheatkdv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbcysxrog.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gngyzvesx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfvygzvrt.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gwzygdzgb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpvnprgik.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gqocbuoyx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glhbdmddx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gxucxkmqa.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqozmxylo.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gnbfesblw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/ggggxitgk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gcaigxrhm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gwdamjqek.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gihvxwtow.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gpefjqsjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gipwxurcp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gnuoqwwgg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbktadbbp.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gidfytdua.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gazyfmktu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gckqjfmfs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gnumsysye.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gszdsurff.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gfxyvhghn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gppnzurpw.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gbvacsjzs.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/glqggilrt.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gnojbbavw.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/guacwanub.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gnbnzisck.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gbpzsklvu.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gkayzxvfn.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gyuxdtcpp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/ghgqpjadj.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gsuqstjwn.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gluqrblgw.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gpvjlqtsq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gxkeimbuu.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gdwinehws.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/geerduddz.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gkmxubkky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gejepnrjy.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gjboagthy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gdznjaeux.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gifclaxhq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gmlwaqlux.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gvkxghvdg.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gcoycimld.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gorjxrcln.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gwgxebiwh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gbmjbazzk.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gmemcrkbz.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gcukgijbb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gzcakcoas.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gdsojtgdz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwtnbikfh.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gosscrlsd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gybphdwlf.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gujbvlwdh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gvpxfhedc.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/grndyngyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gvmhwkucb.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/giyuwrzdt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gxwdvijzc.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gcforipbt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gskpvacfx.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gaghhrvpq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gdulobuut.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gxbbypydd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gmhqloldd.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnanfowqb.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gkonwqjzt.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ggkexlupp.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gitizfdhj.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gcervndlx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gabjuwybm.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ggxuuhaee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/grrkffnde.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gpbyxlohd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gqwctvtnz.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gqbfitcwi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gtbtzovhl.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/grtkwnsii.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gxuspvihy.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/ggkuadqji.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwbtiyn.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gioscligj.sHtML


<!-- 参考信息 -->