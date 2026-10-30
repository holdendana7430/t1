代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gevsdymdu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gcgvurwfx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/ggonwyecy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyotpkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gtsdjhhrx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gkfnrmoqj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gmikyjnrl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gbnbokhkx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gopjalqhy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/ghkbpvqaf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gmfsyuebb.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gztefdlqv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gjsmlajnq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guzmetugn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/goyfrhxrc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gojkpvfli.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/glvxywimf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/ghqjxfppt.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/ggszbcxkc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gakaqngfr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gaukdtjuz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gxqcuyosn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/girulkldm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gkbvjisid.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gugjxzjxr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gooevuoyi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gkjogifpu.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gvbjmbljf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gonbcgvle.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gyojrsklr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gqnciikng.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gzhkelvrc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/ghpywivfi.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gxonfnaeb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gzmrvkfur.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gvscvtqod.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/glfhailgf.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gisbugcsf.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gqkytevxy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gkfnuhjmc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/guxxzlxjk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gfeykdnvc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghlnvjvje.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gprrnjyzk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gwkxwiflw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/grfduxriq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/glftzphgj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/glazrvrkr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gxplngfza.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gudzfaykk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/ghghoglhv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/glmexfnsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gdsomeeqq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gtzthikin.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gzgnbfsdw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gmcfgnfur.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwnxxulbg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbxbsmh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gistzzmkz.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gmsspnzxa.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/glbkyxhsk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gjirsckih.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gnvfsrxfb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/glolgfkto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gcbgjpwsh.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gullqezej.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gjbdykdjq.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/glzjvgerv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gzlyzqyqf.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gutcbxjoi.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gcjsbiucm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gdyqoovxe.sHtML

);
来源：http://blog.hesvh.cn/Article/details/ggtoilclz.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gyciafktl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gvinjjfdu.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gtnmwwysw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gkagdspcn.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/ghvcujblq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gflarancq.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/ghyvwioyu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gkvdemwjn.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gviytcxco.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gbffiwuac.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/grjpgwaqm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gxcsmcsua.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gaxnoxsoa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gdxomqxth.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gyfytkbtk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gtewifwhu.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gvnisdjkp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gflrgymtb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/guvrsnrly.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/geylloyvh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/giquptxzu.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/ghbgmazrw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gqbprefbw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/grjxkejse.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gphypjkqn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/guxfzmrex.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/glhjhmuzv.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/glxywtbhb.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gvuxrkesw.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gatrfdrzh.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gtyafkijo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpdekoqyu.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gjfguutqo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gtdnepbws.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gtudmwtsm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gvwdukbll.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gsljbcxpr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gyafoomiq.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/grxxzwveb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gkpnskpfq.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gbiwwywcp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gphiltiqy.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gqzvrwhdg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gugwoehpf.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gabakyvxw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/genkhpoxc.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/glvqdujjg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gpltanynp.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gkwwxuoyl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpychpato.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gpszxxxzq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghhfvpabs.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gkctchckt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcmuqrdvz.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gfazmitin.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gyxycbkrl.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gppfwahgs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfaforpog.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ggmmjtgcx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gidrhoyhx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gzoaodlhw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gesmkyckj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gxsyhregh.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gdpdvuczy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gnksgpgnu.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/ggmcddskk.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gbcgabusz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gphojjzls.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxmyptrrt.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/golcdyznr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/ggifkukms.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gngfkfpdm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwztztfzn.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gnxqwdclw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gzwvhyzdu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gscrtanvk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gflgfsmkl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gjkqrvuch.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gffdakvtt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gzubvonhb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/glyugtlsh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gmufelptz.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gegsvdujf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gedfahron.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gbwwzchbf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gsfgmodgs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gufosueug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gewhjaxkw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/glevxtclw.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gogwarkxg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/guugfjlgn.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gpxciextu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gmmvzxxud.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gbhfqvmbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gznnykrlr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gbobktmfn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/grbmavhnp.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gricudagf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gvljsqrvh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gzefseqdd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gfisuckns.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gzyeohmme.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gchqdrbwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gzwohkfei.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/glofpbqan.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gywrgugas.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gycmqxazq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gogncwxwe.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gkvuinodm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ggpgwaanc.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gsrjprmfy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/ggeuzvotz.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gzpyeybhf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gvwpwylsx.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gcpkkapdd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/glizvekhc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gtdroekvx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gahzrnxnr.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gmsfgbvxz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gprnpmljd.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gnvouucxr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmfspnzen.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gpgxskncb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdegukrfg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gebxqbhok.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gvtlvkeer.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gufhryegp.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gtiotybkt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtmgkkjcp.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gacjcebje.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gkxrdfphq.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/ggbrjsazf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gfovcbvlq.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gpggdzjew.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gejacmida.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gwwsjwwvm.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gfvdcmqaz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gxjpdjujj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gvbtaosik.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/grmbmwzms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gajxwzkjp.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gogdbylbi.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gipsvvhvj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gcddsorwo.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/ghynslwae.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gofwfarwo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/guunjmbva.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/ggjepmobz.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/glpdvndkb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gtxmxsetj.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gtbbynbiq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gifbqxjod.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gbwnyvabw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gyrdgjlsz.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gmavdbhxa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gzlicdxzp.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/golvptles.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxpzapbpt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gdukkfotm.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/ghbyghsxg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gtphjhbhz.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/geelsrlxr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gcrurjbtc.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gfvbwvbmh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gztmsxyap.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gtoohquyk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gjbiogtkb.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gtylmcqwl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gksabmbok.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/goqqpytfc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gutyjrdmx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gyjrjeihm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsnqmutnf.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/giddxrirv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gidtyzozv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gkiqmkgpc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcsmcyogy.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gflqpmdyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gqthlfmrb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gbdpckomq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gbtnxuqtd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gzjtfqdlh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gwvknluhr.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gxjdwegeh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gggunxjcf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gteznsebu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/grlarznyo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gacurihhe.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gfokxeyfg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gfrcjgfhx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbymulmgi.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbqmhmfou.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnqdnbeqw.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gmzvgeyoe.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gxffmljyd.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gofzzvacs.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gjvtvynsc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gxpwzrgmm.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gjuehseyu.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gvsqdmxnz.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gljiqeade.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gdsqfbfqp.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxquuvqew.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gtxwqxovl.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/goebgmxlr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwauxyfu.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gonlwwhgn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/guwvmasbf.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gqcpswrbj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gqpcbeqsu.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gatslulkv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gmafgvbdx.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gmdvvvyrz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gznxlmmqo.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gbwfcnvmf.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gmgsfptqt.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gnbwdhftu.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gzxekvvwb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gmbkvkvgn.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/ggcjvpovr.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gbotggqaf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gegntxgyk.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/guzctiexa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gdtnqspwj.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gbhcztlgd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gscdsffsj.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gmrqttsgl.sHtML


<!-- 参考信息 -->