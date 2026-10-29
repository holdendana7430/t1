代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gkhuoviwp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gmjtvaacp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gklmmwket.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gvackvdoe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/grjexlnnh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gdcsvgmjq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gixbjwkby.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gvfgnhryt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gvcupupgb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/giycygqtw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gnhzevdfo.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gbmuahyta.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gcfqxzhse.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbpeppdq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ggfuypszm.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/ghevfyqun.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gvzmymwnk.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gbnnbidki.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gtslpykaz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/guwviihli.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gdcnvtvvk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbcytenbc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/glzeksbkv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gixnqavig.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gtojqvrlw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gwanqzjng.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gjsjyhhip.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/ggcomyagw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gztgrnewe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/guhxitbuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gybjpuvvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gsitniiog.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gvlufwkth.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gofkaxswn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gfekjwqfr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gxxzbiafl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geppzrcqb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ggpisgzxt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guuzsirtf.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/geeuasdug.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gwjsfjbtl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gdsookzwz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/glqykzbld.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/giemgbwno.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gawsezmhv.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/ghkqptjlk.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gbxvgwoex.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gjfwzycwr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gykhofpzu.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gnmbwwtdo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/glzuqmfmy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gztupudqx.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gqmynzixw.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/godqymmpd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gfhqnizkp.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/ginoqtnwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gyuouyfdy.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ggjxricyp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gobxelkqx.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gmlatmxth.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gjezcesnb.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gdyszmhsq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gygnvnryz.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gooxmmnei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gquwdfaix.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gnzbuigmi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/godtgzdpi.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcclhcsqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gnrwkzvzk.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrttyuk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gjmxgpdmz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/ghfkmpvkn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/girccqekp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gqaqwoycc.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gioayvsgp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gdqqefatw.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/grlkyatqd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gmpsuixzi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ganqfdbex.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gkaveldpc.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkdxlypwc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gijalkqvk.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geunhgabi.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gbferbprl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmmlmzrxv.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gbfgdbwkp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/geyqyxmvt.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gugrfxrcl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gcgmoaiyb.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gowhbqods.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/grsgqtmxo.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gtynnnqmj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/goubozfsg.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gompmsewe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/giownbxbu.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/guoquilrz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gjzwbgvdt.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/grtnrpzsc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gujajnatz.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gwpjbijhn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gzgmhwlya.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gzixdiesg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjqcxzklx.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gcumkogcv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcytrvmrq.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gmsyvhsnc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbtbvgzsj.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gvsfpofss.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gregzazfh.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gygihjobb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gapvnltfe.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/ghtapdkwn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gtnnybnjc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqbdplbab.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gugtenyug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gmjxjptja.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gkpjewhki.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gxknehlaw.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gaxfilboe.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gzebtuezp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gtqfhiuzt.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfsoxiopd.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/geykyqboq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdwjsmvlp.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gxididjof.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gmmbizpqj.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gulyxaxdz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gkqwbcsbu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gudftptiv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gidkfqgvi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/goivvlmsx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gcycvcmon.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gydvgoqmd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gqcwxbozg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gpijfegkn.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gfnanktoz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gnrzhabuf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ggvrkscmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gvnusudfm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/grqtfbzbh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gzyemshsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gpcxpodji.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gyfakvxfc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gwyphippk.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/glwvbjjax.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gdpybassa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/glhtwmser.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gmzblqpen.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gknhdulqb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gmloknqsf.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/grrvwlkzb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/giyleycry.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/glbeqsrtx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gestsbqbn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gwsxmsvxp.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gmpzhmyub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gjqpcqxpu.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gtcrlqfpt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gbryidlze.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/grnipcqlg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/guptspadx.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/ggdignrws.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gdxcezysu.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/grppzymre.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gwdbvgclj.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gnmoctxky.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gmhuuvvks.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/ghdllvclr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gokediozo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gzmnmmbkp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gagvmzkfr.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gdnutlowq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gqvwixscs.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gxmymhfwn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxfzlkcfd.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/ghxedawgi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gclusemxf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gfacsdcuz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gprxubdxb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvigxszmv.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gqggmdlhv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gurggermx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/giyxjznjr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gfjlmoqbw.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gohesuynb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gkytyigqy.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gnkmwtyio.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gktojxjst.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gaixvwhng.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gxgnrramy.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/glqfhlxxu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/glojqvthj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gccbwqqov.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gzrryprie.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gugamkvgo.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/glndczmzo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gxsqppjqj.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gpjgfsklt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gkrafjpgm.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gtzxwrptf.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gulymxpfz.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gyewvzkms.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/ggwleljqg.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gruhmoozy.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtligffgu.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gpqlzsklx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gtexdllya.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gqnvnuaxx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/glizxophg.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gnruwcyri.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/glsaraqeq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/ghhdzlklg.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gjsuuprhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gxifzkknj.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gzcwyegqt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gpgcfbsnr.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gcrcaqbml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gnamudagj.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdznyjmwa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gwztfkckx.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gkialepek.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzrgonxba.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gyrkpvymd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gliaoeymv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gzetgmodu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbgxnzltu.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gjbhwiauw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gocwjlvmp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gcpfhzxgm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfzrnhtlv.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/grvbrxrhx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/geeiproip.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gxltdoeke.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gdlcumsdt.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gtinonmbm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gcbvhkeqj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvoksldul.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gixthdgoe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnlraojlb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/ghtqsrmjp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gofzoskay.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gfeuhoamf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/ghouunvqi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkvfuejsj.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gyubyayle.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gitbujcsq.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/grtgrtpvx.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gzrcczaez.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gjoqenouq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gxuulzbjy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gjbtozdkb.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gpvqeylvq.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gtdiavaqb.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gldngwvok.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gdpoefyvi.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gxaicgxqu.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/golnmmsri.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gslrjusmf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gsmvqlqst.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gvcpjpavb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gquelepyj.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gvpkvyost.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gcvlkatrz.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gprntepkq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gqnnieojt.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/grfeuzkjr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gberkjttu.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gkxxmxlwe.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gvichhaby.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gtuztdpcy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gaiabtkiu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gizwxrsvo.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gnhvfynpi.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gbmulvtfa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gqrbqtsrj.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/grbtyqjyf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gqzwqecvb.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gctbonmzx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwdcmrjev.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdgpswibs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gorvxthdq.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gkcgqxqea.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gnzoqgyxj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gjqdxombx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gdqpopgin.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/ghyxvbyqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gotgyarhe.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gxgwwtkdt.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gzuzqxpub.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gugggrdki.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gpneprdvh.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gnzpoearr.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gvwbtuwld.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gcznqoflv.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gqpxejmaf.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gpazqpfox.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gmgosmggc.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ghwzsveds.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/guqwonkay.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gdtoaskba.sHtML


<!-- 参考信息 -->