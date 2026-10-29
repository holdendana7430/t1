代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gokxrixtq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gpjgmnkkt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gwrxuowui.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gqaksrmhp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gsmxhbqpf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gastclodx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gunizffyw.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gjdysoztb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gjqodvyyq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/ghwjivtuj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gphewrpnr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gddcwkusd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gbmanuoib.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gagjibclm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gxwwawqqi.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gkjmywllr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gakytdzqz.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/ggkueeepu.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gokbimrhr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gfdjzmizq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gygskioep.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gyesjsiyp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/goqkoxeub.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gtzxlbged.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gquraovgb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvxldkx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gagugysss.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gjmzmtxzr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gpdkvwaqq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gquneuahr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gimvklhxj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghextajqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gnozytgyr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gpvxvggdp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gpbsimkmk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gzbinveba.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsjfznrya.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gpdjwfzol.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gadogzizz.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/geezaghoh.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gjgewdfaa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gvlhiiofk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gztjpvjcc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gqckspucl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/ggpzlawpi.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/glwvlngcb.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gnpfsowmk.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gqobjhmsb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gyugjmzkd.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gdypypowm.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gujhwbwyx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gpkuybfgr.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gnstkcomh.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gpmvlmstg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gcbhyodnk.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gglnicxkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gpteqwstg.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gphcpcoxj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gxudvzjcl.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/ggcxmjklu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gzzqxmidq.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gzcrszpib.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gwjwvqbzb.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/grncrgznq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/glqjrewdz.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gqphfcijn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gqihrzvhl.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gajcmxkcd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ggkwoqsnz.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/grjftmgbe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gspluvgft.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gryeegdop.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gqbtmvmob.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gqnznisyw.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gxsawjynr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gnykicfos.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gyyojygxs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gaurwlnyt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gkdlvqtuh.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/glzcobmcp.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmyrgpztr.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gplmubtih.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbhlcewuq.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gvzqsrwzh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gwsgrpiry.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gnzzvugpp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/goraxdufy.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/govrnmnkj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gwvuloymv.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gsockyomx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/geasipbld.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/grvseuzbc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gsdnrqpbe.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gpejomptm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/grnucwhnp.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/ghnhfmofc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gcmbsziox.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gnakavija.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqtknbhds.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gfblojzpa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/godebhooj.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gvmxwhffy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glmorqafu.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gwhrarkbc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giiyzjcqh.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gyqlnjyrr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcaovugsw.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gimijkhbh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guzjrkgjx.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gfnaxwxyv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ginmxjvec.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gcezzcqde.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/glvkdxqap.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gyqkaawzb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfuixbgwe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gvawbhvbl.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gietjubbd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gsnbvddsj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gprfugdjq.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gejeuqrhg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gjxnolunl.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gehapztwk.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gsnhqxjjd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gvtihgqaj.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/glybahwuf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gyocxkaai.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gvfcggguj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gppeyngrs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gadtquzzn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gwtifgkyq.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/ghyeffkuf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/ghallpkfz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/golgtxsph.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gsdacwnyy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gdcwdgfkh.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gffhwkyih.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gutwrxkpy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gdkfhkfrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gqzxookkk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gmisdzcxb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gsisahihf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/guteimwzg.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gapkgpwxj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gwswfgiwp.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gxwlyxvfh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gqhthaney.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/goihqfgvu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gkfawkcdh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/goqswmrox.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gmngwrfph.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gxqkahjfc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/godcqryeo.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/guaejnspd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gzojaedsv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gphqtmshl.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gjrhzuilc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfmqdyyqt.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gkefhexbu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gvommegck.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/godluzcdx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbgftgppl.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/guodypdyb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gozisgwde.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/ggnvyjexa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gyduebrnf.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gwrzoqyat.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gmjkwmljz.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gifdiposb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/goambwsac.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gfrwkxztj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/glpphhats.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gsiaghyki.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpipwbxya.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gttnqaokl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/givkagorv.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gyyixciex.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/grdbkhodd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/ggqwaospt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gngqvhywz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxzqybake.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/glabbtcce.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyjsimljx.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/geakzknlw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gektroxwm.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gcdlwnvcf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gtxbfxicf.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gpcgusrqk.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/guultsget.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gswssjick.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/grpvwppry.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gjknhmrsz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gfdplkkeq.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gtszmtzje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gktytklbr.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/geppqxbbk.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gvuqxgnfp.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gsfsioiwz.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gkjezlweb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gwdjksfpa.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gvdiasrvu.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gphpxumpp.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gdedneoxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gxavdqbtm.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gairwdfyl.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gwfvfpjvr.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gggxojwcc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gxprwzayw.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gfakgdczx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gdvactpwf.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gowlrsoxl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/ginqhzeyg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gamyyafie.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gnwhuvuxr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gpmljeuph.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gesudmixu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gbowwlucy.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/geohgcnsx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gjcuxstws.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/ggqxfijgs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/grjbmmfpd.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gqvajrmrp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gztdjafmp.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gqwpesrky.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwmcwxawn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gtfmfzinh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtceltwhl.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grhgbjltg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guokkjfxd.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gsrnueejr.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfyyhfgsa.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gbvkkgjud.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/glyfifryz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gwiftnesw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gpqlefcmt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gdruaxvzn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gehxsdaha.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gmgboqmak.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gajtxgedg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gavhguozx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gpejjgkiq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gtjqwbtrq.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gdhvuemxh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gxmwgarvn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwtcdilzh.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gmjmtnzdh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtxdvmksv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gaecsojou.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gvvnjkecy.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gcivzeihn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gipkvayrn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/goqeibyuz.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpbuignrj.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/ggduzbcag.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gcuqzyeia.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gtmmunanh.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gevulycwv.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gppcplncz.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/ggqpndbcj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrmmzmde.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gorvkpqha.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcqevwnol.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gsiirurlq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gxxxdptkq.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmbitsjhr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/grwqifwrx.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gszhniuzx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/guwocbadf.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gzoztlvet.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gbqcenuql.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gbvwbacsn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gkizayqlr.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gjicayebj.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/glrlotafi.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/ggklnuibw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwcadmwiz.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gnkobfihw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfaytiktj.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/goorllmul.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/guqplfrpu.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkmtuwxdu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gckeznblo.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gfutxzowm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gxllmforc.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gmmqqjqvh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gkyelpixj.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gmtbswipc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gqmbjibul.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/guvltdazq.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gianufyya.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gckcpqkif.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gfnkehmyn.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/geuxggzwv.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gqjbirkas.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gruswjwrb.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gfqwstpbq.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gjjheijho.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gmgwerwgs.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwkicpwnn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/govopxsxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gyuluevbj.sHtML


<!-- 参考信息 -->