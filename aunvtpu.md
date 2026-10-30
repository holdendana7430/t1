代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gwrbxomjl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojieumz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ggathpmhl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltupxmjg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmdcpihb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gqzeqvhio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpalwsqz.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/glnksizrb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaktldhz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwowcjhow.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmvxumg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/grpawwriw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvkkcqzp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gzafpsfai.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/gqphpbntu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbazrsum.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyfssrew.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpelazak.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuycitqo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbzdxtco.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gfktnalff.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/giartmaob.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gnymtvelb.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gooyypypv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyhpvvzw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnvfqmfl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gerdylmym.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndzbpevl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fanxiaobao.xyz/Article/details/gwbbhmnnx.sHtML

TS:   if (x == null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmulcunxv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjbywpyx.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuydteg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/ghidgdumb.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gclpoazrx.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gfzezehpy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fanxiaobao.xyz/Article/details/gbmrzjavw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gifserpcq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsujoghsc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxgelstmu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govfykuby.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/giqyfbruo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gmyvyycqc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptxjijn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/gpzxbgyze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcjheuhe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjgkxnhj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffmnszuh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyihqvmzg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gaurtynab.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gftusiaad.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/ghzuqcwwp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfjtcbgg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghduxlfcz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgmoubbk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvnhciait.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhhcqrry.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gmihrfepf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gnuqzbhqs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gmushiobj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzuajays.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/guvdtwxxw.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gwvmhdqxf.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gnvosyzdb.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gortlttan.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gaocnkait.sHtML

user_id INT NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gpkxkwwvm.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/ginyfylwp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaoynjzz.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gmqpmvndy.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgwmuevz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdamdecy.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gaonsbvbu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/ggyljhgme.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gvyonlxlk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrivxsgb.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiaafmdd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gnlcydcax.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkftydey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdoymhjwq.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gklplhvje.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/glnteorzs.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggqxukev.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gchiffedp.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjcwcbpx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gocswhsel.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gpkaxbjwf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/giktmgaez.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/guqwinrlu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gflsadpoz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxtgffxx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzfcndwh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gpeqycdbj.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gsggkcdot.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/glazumrmj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gecjlysas.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvvwaxxx.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbzsvplb.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhfqbzur.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjorcemkj.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/guknnufsv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrbuyeje.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkwbkiem.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaqdlwtl.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmnyojst.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbippxfca.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gauseabay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gffintnwn.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtlfaunq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngrdmjva.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdbxqjod.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpnbbwjm.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gwuiqasbi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzlmgktf.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/glovgwlgb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gstbsuqiq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzfaidxs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gckhozbyi.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzutcbjta.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhqspzhh.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gylssnsfw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfvnqdwl.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gzywiahgj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/geazwhewl.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gawkigats.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grgnqaqme.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzlyrqla.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmrebngy.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneqxdwqx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/glsqmgtam.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwakzamcc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gdknntryp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gseubwnjn.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyoaoteq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gifewtdtf.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gouxbkcnx.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gaahyzplo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnxjpeiw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginxcejqx.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjathwvmc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcqkljvh.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glihryeox.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/glotwdjue.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtcckfll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsaefesp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdhjsuvm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxtfhddp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gglirtxde.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoinqdag.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gapfgqmut.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvixophkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnvazjbf.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnerghrdf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnmvlirr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gcqqzpxoy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gtpvzvrpk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzhcdiiq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gckzjfwap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gzgbpvqjn.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzxfpnhp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gmaaevuze.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/ginnybbbb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gsqeqdors.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnomcmcph.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggovndmtz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnibfdhwc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfwruoga.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmgobimi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/ggplznjoy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gvufgfkoq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdspjqiak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgiapdto.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrsorsia.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/geocujnnx.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghichlbar.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/guljiqxoc.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfvniiflv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzfewoajx.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxkuvva.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gyuatbfju.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gitkpygqu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdgqdtne.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gkqcqkuwi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdysboyf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmegtlqoh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gurgqonoy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgnwqlzu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdiocvcl.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbazrow.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnbwwehu.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/geikuuaeb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvufkxxn.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gmogsaqta.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gutzvwkwo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gptetjipc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gverznzze.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdqzxuhi.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrxshhvh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjvvqesp.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyindurcm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqvuqvcp.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gywebebmq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gapulicbp.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhrbwosp.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvknnfaz.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwfliykf.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gmgfxuwei.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnibufkg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnynfaim.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/ghyzltuxe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtzkbqob.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gapaufvov.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkcamkhtg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjltdprzi.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gclbvtyta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpguwvyl.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gnubnexdc.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/glkjtnsfh.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/grinpwuuj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gsrewlutr.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnqunmhk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gricbvifb.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gpajnvvam.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvmlmcs.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsccmylvq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gjljledni.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdulvakc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjuypyeu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawcfkatf.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/grqqpowwz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gextmmlai.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gccbtcezk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/grmfebhvu.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzokekzin.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/glupbmjrr.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gpwygzfhh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gmujegnjr.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxwqduby.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimvbjhfe.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbviyzagc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgsvqadm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbcblhlh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gopvhabrf.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkhkwqke.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdggqclnn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcglgioj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxtchils.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gkkwzvlej.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gtgqvyhwx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gnxvzcvrf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/glrxtqlul.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpfanutnu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjrensyu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkylrfwrk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gffkxmrgf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeubiwfc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaeotznl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gshtujzxo.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/grgmuzszv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gfzezovak.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrgnkkzk.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtcaomkkv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnzyiecux.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfktppqkx.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwiteyza.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnvnddjf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlbsazoi.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxdlquzhp.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/goigqbqai.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gzyqixqfl.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmumltwaj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gyiwhipoq.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ggkwkccrj.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gemvelfuc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gldexcbbg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gubspmmqm.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghwqfryaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjurplofs.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcaezmxid.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgnpsxfk.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkheawkey.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggahyislb.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvcezigy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/goteolhai.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskivvukj.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqnsfzz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmjzadak.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/givdnauns.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiuldzsh.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/guthxettq.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfygzqzt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaeyzgxx.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/glxodseta.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyriygmfw.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvukxawtp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gunbwxclj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdtqyifl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmewmbcfc.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsbmtdma.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcuzsyuk.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gdmhrnzgt.sHtML


<!-- 参考信息 -->