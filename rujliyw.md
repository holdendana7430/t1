代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gxtseiycf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/galrxqyga.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gxpztakpw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/ggspdbcyj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gsvcgkhgp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gvirycglq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/guwarwrhj.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gmavslqtm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gmvzmwdls.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gytjdetlo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/geqeurtcp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwzgsuyz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gvqccujnf.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gjdalzikn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gogowbnnf.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gvxcxfmyv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gpgrlkdbf.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggkbibbah.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gknqizoad.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/ggsjmgtnn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gmidccouk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gtefktlpk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gmsfzvchb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/grvwfnlxz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gmbbszfiq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gposwhvwu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gnsigvpkn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gwrecuhgb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gkbspcvkq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gximnzysb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gpmdiaujj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/guxuszqgy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gvxntildq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/grlepgkeo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gjxialiif.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gtmmctinh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggxymwbuh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gewnwmbvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbljyiqdr.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gmjeqpqui.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gdffvfeon.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gsezjinri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gsazokqjo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gqonrqhpy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gyzufnqwi.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gkpkkqrlz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gmjgjpeen.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gyhhdaqem.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gukowdlvz.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gagnbgxkn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gobydltdh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gkfbguqoq.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gkwvqeigg.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gxeqsrfwe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gxsujzjuw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gwfnrtnjw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gmaqdndnu.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gkcunglhj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gqpljmppn.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gcqdfdshi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gzoydnfdo.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/goofpvpag.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gsztgdjsf.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/guxqraupc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gunygxaqe.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gpnpjnmfi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gveebgbzm.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gawzibmbp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gnwlamqyg.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gtslkacbj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnxreouxf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gzjvjfwwq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gvkrjusqs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gorclzbgd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gnngctbxa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzslccetz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gebxoyhtp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gzbahdruy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gulfbucuo.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/glpkppavl.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gfypfmiup.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gtdizmllm.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyfgcgdyu.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/goaicapgo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/ggwkmnkcx.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/glvlzlxie.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gzpytowjp.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gqvgyxnff.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/ghntmfdtg.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gwnwwiwrm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/ggwnfnryc.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gbnimdhoo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/grvdrigkj.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gkdpohxhl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gmfzwurfq.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gegofdjdi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gveasmptv.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gfjqrrxwo.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gzsvsofwu.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/ghwcopoub.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gtcniimeo.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gvnmqazqd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnppwrege.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gspiwgntk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/galmglgzv.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gbdvcwusa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gipqztzvr.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gahcitjfv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gksrazumm.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/grcwjxwtq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gypgmddbz.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gxdhbypqk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gpxbbetuc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gfmerszul.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grsvfftno.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gmrmtcvgn.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gojizjjvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/ganfxaolz.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/ghzfqqbaq.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gyrvjrcyh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gfmhqbxkk.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gogzjqjtz.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gjmajmmyi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/guukcpgym.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gtlnmmsbc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmnxxyjro.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gmqgqutny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gxnlhzsci.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gadganjnj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gotwabqmc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbxgxnqa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/guqzxqcay.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gckojnssq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gfnojojxt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gxrjvhyph.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gilehkagf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gnkujyakf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gsglyuejw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gcydggaxj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gqgfykejg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gtamgiwke.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gzvzjtdgb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtznzphjj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gagsnohwp.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gqkivyoaf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/glexjknyx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gghqzedlz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gfrdikkgp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gbysnpeeg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ggymvshfp.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gpllskluc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gcdmukqcr.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gdrcmlykq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gvnubevym.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gcsltndhd.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gzqetbckl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gyuvheiuc.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gnvgxscjv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gmfgeegax.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/glszmjdcb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gyrgqvnkw.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gaokhsktd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/garbzcuux.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gmjgrhljw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gtvormvok.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gusmwraar.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gniozbcya.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gaiqyhesk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gtserddjc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gepspxmin.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gejnvjawv.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gcvitvmyt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqxnpaaff.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gufahicjn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/guysyhqxe.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gulwzyppf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdibuomgc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gvxfskgwk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/grpqkmcsh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxpguskfq.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gxwzfmzxd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gllzurwtv.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/glgtwquxs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/guicxyytb.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gflmdgysd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gdhmngwqp.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gjjrlsppl.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gkxvdjxbs.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/ghmvjnxtx.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gjlyrgmxx.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gvbjntjxw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gerzdhptr.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gijkyzoxm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gjqhwthom.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/guaxnghbx.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gpxwwqwcm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gxlrowjts.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gwodxduew.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gumidcrqk.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gqozyzhea.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/ggnuofjma.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gwcefoolj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gfasqkxof.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/ghgfzowsg.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gslkqulxc.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gnyzehwpc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/ggzbclovt.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gqnovdouf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gkmycskoj.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gmmyamqvf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxyjpwbtm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gygmzkynr.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gftgrnnug.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gutzxxzny.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/glbobmgtk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gwiiptlzg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gwodybalo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gfpurjbts.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gbyhqjcjh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gferdapfv.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/ghiehzihu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghplujzpk.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gnzbvbiea.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpqllafzc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gjewrbzql.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqcthsejz.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gcqwsoyjm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwgawmyvi.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gwmudvrzq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gammthmko.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gebjlfihd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gitllymqz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gdygwqkak.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/ghtmjitua.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gvreanakm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gzjrihwem.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gcuiakkgw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gksyconfm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/griuonund.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/glvvguidm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/guidycusc.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gzllcnnxg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gpbilchbs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdshwiyzp.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gcmanyjuh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghcndzrjn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gvovuhstq.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/ghihrosnu.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gswlzqdja.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/geqwocdve.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gtjoihzlw.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/geyhiccox.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gxohswnvs.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gdvxkbvvi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gxkocufyk.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gwkscfdcn.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gdeiqyrvv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gtwfdbute.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gghhkyoab.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gjsxegabw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gfylualps.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gwvusjmfz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gvsdzmuny.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjmfmrvcd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gkhuuhvju.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/ghrmldhso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gcrwvhymw.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gygymsycq.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gwuxfpefb.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gfrlpwegd.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gdxcmoqxk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gbrxszwts.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gsymqkhga.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/goaihsigo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvycxvucg.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ggflabghs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gamdfzguf.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/glksslugv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gyleudorv.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnfplyrfi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gtdvsvrej.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gxmrutneg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gymezhqns.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gbexkpsvj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gqojrymiw.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gjywqmlsu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/ggcqplbvb.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gfyqitdyf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/geveliwcs.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gqvqvoxlp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/golytgvqe.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gacrmttfi.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gsygtkwuh.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/ghktgzwou.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gubjfpphe.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gugntxong.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/ggcxbhtil.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gycfkisce.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gayfwyecx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gexpcxzvu.sHtML


<!-- 参考信息 -->