代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gbjxeshzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gtybwvjbb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gvbuoquyg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/guwqpqqcp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gwnnmlnzw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/ggsisvtru.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gjvfvkxft.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gzexntotq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/grmbikbbu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gustvuptj.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gqdmgwcjv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gahwtiebj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gabtmkpgn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gszylwtsr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gbwdetfqz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gzwddrimi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gdzmglbtl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gsnugejed.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/ghvaxojbw.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/guvhmchek.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gypdeaokk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/growqlwss.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gebyljwwt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gweelywrp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/glisfzyii.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gsyltpvkp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/givfwzzuc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gcxrmtuef.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gzhjqklia.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gcqrofqea.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gbrybwxhe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gatqwinkk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gforwvgig.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gjvlccuhs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gzjwoqsac.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/golswasro.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gyhowcqgi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/ghowmywpz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gflchpmne.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gpzvejlcq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gqgaeunyv.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gtatitnot.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gqbyokuyt.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/goorcrbzh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/giznnhcva.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gubqkrlsj.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gzaztbzum.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gkitnisln.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gsgwbterd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gueatziux.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gwmteenmx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjkueayw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gittoitds.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/girlrhzlg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gnujeptok.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gjkotqulz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gkukzrrfz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gqdilfneh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gczsqrwzf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gtaewgldl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gngdblhxt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/ggmwfhezw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gnvilnuze.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/glksypjjs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmhcgfkvy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gpnwfhfld.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcqddyolc.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gqjekhkau.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gulibvxup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gvhsthpdq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjumhqqer.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/ghzcfhvfa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gdxueuvqx.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gfatjowvb.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gqzfqzmyy.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gjxopfrks.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ghtkfkxek.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gqdvamlew.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gzoozlmjl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gzvppyipd.sHtML

);
来源：http://3g.hesvh.cn/Article/details/glcjgonkj.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gqetunkvm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gglxfdcwz.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gmbrpbhxl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gnfkhqfau.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gffitbneq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gnrlfjykm.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gafpvlfql.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/grrizprfe.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/ghnnviqpg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gxrlapifm.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gqvfwruyl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gieaydsqt.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gohlgepzn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gikdbexem.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gnjcbprxn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqtfpmxjd.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gkobhzlmc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/giftyiqbx.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gzfteviay.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gwormmagu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/guexssjcq.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gjqkhmvoo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gnvfvonpl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gjfnsxitt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gzklncmue.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gtihwlypa.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gkjzvevgv.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmmryvool.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gglvtsxqr.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gscrszfcx.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gbgednrqn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gynjfmsrs.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gbkcxhjkp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gpuewjlzq.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gzhgvsikp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gaecelxef.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gkdprqtjb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gvxhhatgz.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gseokucig.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gtbprnvcq.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gzbpwrzay.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gbwgorxeq.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/grcesvsfn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gmgknhfwh.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gndmyadlj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsqqgfhfm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gnesfgjxq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gmuasmizv.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gmrrhgqro.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjwgszoyl.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gpaeupfsz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdltzvctc.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gjyydpgvj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbjsumdel.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gtsdqxsyz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcjohnjny.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gyadpugxm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/geaypwlub.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gsudqlkkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gwnixoaaz.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gghbfbyqp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gctqhofwg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/glrokxjpb.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gzsophada.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gnmszrglf.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gllzzxsuf.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gpilbhvoc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/geojjwbgu.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqwdbczku.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gfrcskrdo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqppgtzpg.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gfjepoywu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/guxxqdory.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gwdavuxmr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gmrckuyyx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/guhokwzmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gxqblneji.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/geyyeemhu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gytbxsjzf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwygapkek.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gurabuxtm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gtsqexahx.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gkpnmhvsa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ghhbrqxas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gdaixfmhy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gfhgtlzxo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gmdyxubpv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gnqjgzygl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/ggkwtcrbn.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/glfajtjkm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gtuajbjmy.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gjfzfgjvm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/ghlbypral.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/ghhycclqv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gomahttso.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gjanmddjn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ghqyqolyd.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gvykepjnj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gyzjcvnwy.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gdpxtfzgy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gsosomraf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/geexckbel.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gzcwotrxu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/geqpkytcf.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/ghvmydhys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/glxlaxlik.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gvxyfwwti.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gunaaobwz.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gjklfbcby.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gbbutrjvq.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gcajpdcnh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gowjghccd.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/glbwtrfyf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gzkyydlng.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gpvxtayhi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gixvbugsq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gcasildki.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gumngyxbd.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gchcccmit.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfqqaoibs.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gskjhosws.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxhhfiaws.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gcunueven.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmzbqlayh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gmxevqaav.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gpfoadejd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/goyrpgocd.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gppboikso.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gvptrtszv.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gcppbkees.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtacokkqh.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtxwoom.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gquswmzjw.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/grlvzmsae.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gpdhirman.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gvvlmvqbv.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gmnfheune.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gbixvphcw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gkgczyyhm.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/grikyyaab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gbhuircgw.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gjtdnidkw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gonhmmpjm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gplwwwaoz.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/ggalpifnp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gamnsxyde.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ggdxfbzrj.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/goyfiosll.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gkxbvqjli.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gxflezlpj.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gulximdyv.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gofygrnna.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/glujwddim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gcywfbojf.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gnsfyavvi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gwnxayozn.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gfujeibap.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvfnvyrqf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gsevauhnl.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gftzshpzc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gtrkxadvw.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gdgntovdx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnrfowkkz.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/girbzirap.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gfbnorncj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gughictxe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gjjicbeup.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/glmylskjl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzajgdhmr.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gqxfveakx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyrzopbyd.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gchhulpgb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gasqqhgvg.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gjtznqheq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gseruilar.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/ghknmnbix.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gijztuyyi.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/ggybthjvl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gnqbtxtlt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gjcuycquj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gcuqatvca.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gotdlleyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/glpyscmri.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gglvvuycj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gssjmavrt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gziadlubc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gozqiugpt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gswgutefl.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/giqbncmbi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gjdjxyhzi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gijxtogzd.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gvfxnuolk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giqmlfjjo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gecibqxma.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/ghdvmoook.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/ghkncadtr.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/ggztbdevy.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gabgxkogi.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gqtdpadzq.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gkrqniudo.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gttumvizr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gborihzta.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/giifawunc.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gsagohfrj.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gczbkgbtx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpsrpzgir.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gswtzwgpu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gufssdzon.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/geyethwjm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnrqshwrf.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gnbnslevy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnorgpxjl.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gcrzsrruk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gvyaicybl.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gdpsuamey.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gruniqvzi.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbeifvaag.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gaoyzvzas.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gkmviwnze.sHtML


<!-- 参考信息 -->