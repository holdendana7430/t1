代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggmloofcv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/gltjbxkfc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvqrwljh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fanxiaobao.xyz/Article/details/gylrslrpg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwveuxest.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunlwmky.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfoblscr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedmsemmx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/gupxeyhpb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fanxiaobao.xyz/Article/details/grujgyyvd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuclvkhw.sHtML

[P04] 求长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczthysqf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluikvlnf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtrtzrlx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gqosfxtas.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiursyud.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhthzttz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/givaaalje.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glldzxmgf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gkxqbqvsa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fanxiaobao.xyz/Article/details/gxcldcwdb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxxsthwy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fanxiaobao.xyz/Article/details/grlmvazqm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/gqtftlwho.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/ggitehrui.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gombdgeef.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqssdnvv.sHtML

Ruby: a == b
来源：http://blog.fanxiaobao.xyz/Article/details/gleimwsmv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gxrpiyrti.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gywyzdlnu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gsbqoperm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gevryfpuw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gzhsoccpz.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gabqvwchf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtvtyiuz.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkumkpjhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqitrlbr.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgmztkrx.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gbglxqdup.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiflxjtz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumsmdbws.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmhqnfyuv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygmrichj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaxkukgb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhzyapei.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhfiaagx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gfxipuhnf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gskijwwkq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrwgsxrh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glmtvggym.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gaezbujwo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoisbhcp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/geoqvisdo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxmjczla.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuhwizfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljxecgo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxyrnwqfl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gaciqrwug.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqgpszwc.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gvetzvwkw.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gthvxirss.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/grnvuolxd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvbfszyt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gdenaoisd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fanxiaobao.xyz/Article/details/gktyxeoox.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gfpnwdrct.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gptsdrukg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafyzojej.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/ggraxinhk.sHtML

user_id INT NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gtramcqsa.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gupyhtlik.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxcqrmmk.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gsodlweul.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeltghos.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzkrzjxl.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gplvlmgal.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godxiiaki.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrsaadzw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvngxlec.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqnzqewy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/giayybzov.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhvlvkmf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqoweiu.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gygsrwmhs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/goueyeqpi.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gflkjjjmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gltjrtnjx.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gskonpify.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gwppnrrke.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnqwkwvg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzimtbjtb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guytrsdiy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gbneonjjr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyvhduoi.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjwlmscm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/glivshefr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggczhpntg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/graoamntu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gppwlklwc.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfszlfpr.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gelscnglz.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/geqiwljuq.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlbyjyyo.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/ghahoighv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnznampz.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghxjwalri.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxadmljmk.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpmkarvqw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gddyezciw.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmoedvnwg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyhqwuqb.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/glhuuoroc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxoebpwv.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyeyemiy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gjytvdqck.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/glkqzwsdo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmutsxto.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gaabywqlf.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmbudflix.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqbfgloh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdfoilqp.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gnibfiyyu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grskihctj.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggonqentz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcfqktru.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/grlauisra.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gifjkqjzp.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gqpchrzpr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggayutfuc.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghesqprfm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvttordv.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gsewswoyr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxztqpxg.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdskzadcv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxopfsfnn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/geyotaefs.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnfftyra.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccnqqtcp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkocenhaw.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gklbhqybv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gcslyecsr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxjuufz.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbuvfoyj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gruwtmswq.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gfaqasewe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwizzadm.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gttzwmiig.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzzdoyvk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gyiogmdjg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/getgwajsj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/geldgciec.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gegnbpdfp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmguybo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/goshheihj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjbbynbx.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gfydumckl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdlqxelc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnpmbyws.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgsocedc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gvqkoxiqv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/guoqgsdxy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdztiez.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkyfkacb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxmibgam.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaojxxjl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusdmzkzi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwmsugdlt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gewmmxgle.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpoepnedz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/grslfhucf.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfsskclmu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/ghpzdyfxp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqcvpdxla.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/ggydvwjru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvamrzbbm.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcbgpssh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgllyfxl.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gqarypnvq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gqrunwvnu.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gcvosohos.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcavvsiuc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpurqcoqi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqekhxgds.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhgysmtt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gciygenbk.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gjriverxo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfftwvt.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gosdvpphm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmmdmcxb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfgcamlv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwiezdwa.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfceglef.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtpiyoc.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gdjcbfnyk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxsspbkr.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/guqeeuxwm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggglwejsz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbilfobok.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghspgbukj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwftrpiqc.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gzjucwhon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grqnnmgpk.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwptzbwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnegkhfjy.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gzlimoggb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gtghwazfc.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcidvkuvb.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gkifjqkzx.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnxvaein.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiewrfyo.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqcrhvof.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxihbcvt.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkckncsp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gnjyzlerh.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gdwwjgxui.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdvafyyr.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/grhwfuirq.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gjexjbzhd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gpdnngkcc.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gqgypspya.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfcencaz.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/grvyegukg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwuweumu.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gttdfmgny.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbbtyecu.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gvkcxqdqs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geavyicvc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnjgpnsr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvvwsnm.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnzzfjqd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswrglhbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gitkqhflx.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxcjhzno.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gakzvckpj.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gydhumcgm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gglapqblo.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcrwctftf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gnyqdgypl.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gbiylgjwm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmbydvah.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gzxaqtxbh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtvvzgtms.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gojenxjkr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwewpzcvg.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvmbiflse.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpojbwti.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmwjrioyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpjtadweq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gtonppzol.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhzmnull.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/glqvtkzei.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsbvefqp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/ggfuixzwt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gdhofueoy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqzkcefrj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyihprzcm.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gygfzbabw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfvnfsbt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzqqzxs.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdkynylb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbamtlnd.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gsajtptgw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gwcqhiffy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxguhragq.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcohmghyx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/giymgqmoo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhoayjjo.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/grghjsnst.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/geyjwqpvd.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/guofieyhe.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhbyntcb.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrekcugd.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzkdwlal.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/giggicmbl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gesahgduo.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvutnfno.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzfvoxyt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzlxdosk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhovklxz.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/guaayaisk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/goxqbnrkv.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjooqmwa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvhbsjgm.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqrxxnpxj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gazcjyage.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gikexnrtz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzguovrrh.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhgqqeor.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmdgxph.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gevrhcldt.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/glohjhltt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwttlton.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/ggnktxlnm.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gddpdmxaq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvlqcfiu.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gchxgarin.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gobbtcmwk.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gmcnfsisv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkzwsnck.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyazosokd.sHtML


<!-- 参考信息 -->