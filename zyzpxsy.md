代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gtpitfgvj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gbptcbehw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gyyslnjuv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gnwmmpftt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gujfxivfu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gdtkzhhpk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/ggxrkinte.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gkyxiewtd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmpxipvmz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfghqhfpf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gwelnfwkp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gengxgkqt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxgwxrlqg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/grnowqfqu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/grdvwnrkv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gsewceitj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gyhqzfrmp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gkyqqxroo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gizrmalnc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ggxczebee.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gkakogsbx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/grjrgstur.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gbjvagqno.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gsuwfmzxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gvxemdkkk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gaqtjyeby.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gntgcxtpz.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gibqgwsgj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gdxgnvgjd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfubuoy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gmxcmcnoy.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/goytexjos.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/ghattwkyq.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/ghvubgyhk.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gficwjzyp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gkrrxywsd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gpemmczlu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqylfafhj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxryfhiak.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gzwxrbheq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/goegroweb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gyiggytxr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/grohrrlle.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/ghswhhjly.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gdmdjwzis.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gsppiszmr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gfjpmyecm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gulbfcahc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gsxmhushx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gllsydrcn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gczsxxaux.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gvtepadsv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gszyxtdsj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/geiwrlmpy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guvxemrgh.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/grbeociln.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gxlgqsbio.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/ghqlfrpnr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmzkhemti.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gyxzrkseu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/guqymctuj.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwofmsgox.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gyarmvtzl.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/ggqtdtvtc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqstudkzc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/ghvbmwoar.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gnpgzteuz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gyzfclytb.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gneeagpfp.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gxrfmtudm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gwkyjdgic.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gcoyixjia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/grwgtbtnl.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gdtstydkn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gdekusgod.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gxyrqisws.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/ghrosjbyx.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/glztwnznj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gvtylowmj.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gtvzxwvcy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/ghxerpzhw.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gwjsrokaf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gcpowraje.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gbdnfgspi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqbuaaudv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gvhhkxxlg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwkzdkzbt.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjcrcscwd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gsaiwjjmd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gqgqoyiat.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/glzfwcjkf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/ghyccfnrw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gkhkyhjii.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gqyuokscz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gkslctasp.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gjjurlquu.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gdjbjhvde.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gumqbekzi.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/ghmulwcfm.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/grzmofixe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gytihdrdf.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gnuzxfpep.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gmykhgbir.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/ggsiakqbd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gvdpqbkut.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gwlcdgyml.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gzfvolwuf.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqvslatfl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gnrvwacvh.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gejhjlwcb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gafxudfmc.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gcopqodso.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gkvykuqoh.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gtmdzqvrp.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glesoctct.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gudmtveqq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/geekirmat.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/guwsbmodh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqbvdmgqd.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/ghzobqbpv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/ghkowaogj.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gxjmrwibc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqzictwca.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/guznltdvu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaspqycgz.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/guivxqtet.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gjwyqxdlf.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gwsgbwhvj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gnjpsxddl.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gxrubgwje.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ggdogjjnr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gamdgtbxx.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/ghtqzhyye.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/greftahsg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gdldxtrva.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gjfhgazdd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/grdfkncvk.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpcywlcaw.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/glwqwnqbv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/grjyiimes.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gfkjpfdrh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghmbgxcgm.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gakfmvlxt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwudjiyp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gbtnphspn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gdtoavjhk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gewtptiop.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gcminyocb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ggovnjpmu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gbgbdiogg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gncvbfxrd.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gsvffgyzt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gtshifiyt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/grougetmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/ggngsqtps.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/ggfpjjelq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gsfpnofcj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/guxqhyvih.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gaaflhbjq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/glochzmkk.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/ggnmzdirk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gizkzqpqr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/ghkbwgwzt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gqhxiicon.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gxapuqvdh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gpmfnuxky.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gwvghisei.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gocrnmbqn.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/goqwbfvky.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gqbwdqtkw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gnalnklti.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gphsdvmwq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gsziiaxsz.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/guongtkvy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gwofnhlbt.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gmkvtczck.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gfhtfzavt.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gdftcsltw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gtowacuqy.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gfxrbsxsr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gcjzrcgrd.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gycbvuywb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gbewztssr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gryzcmpgt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gfxoylfhj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gctpbgczs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gcaqbfmst.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/glzlpxymz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaibhvdsb.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gvbliuedn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghejgxwpu.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gkgfiucsv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/guagqutiu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gxwghgjsy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/givqxhhyn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwormgddj.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gcknkcotf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gplmzikul.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gyokvsjio.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsdgbgsua.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gsfqaperq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gpqewflht.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gftsrptoo.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gesxgabro.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gkbeffvnx.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gkqiiyayc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/ghafgidqg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxtjjunw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gcpgmmdyu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/glzawybis.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gmhlkdqfc.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gqkhmtnro.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gdwshylog.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gzpzuqdld.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gaqbdejqt.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gwvuprxff.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gxxvfnoza.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gwmcildmj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gjcqxasbg.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/ggcahwipi.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghybguxwc.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gyrdfhkpx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gkutosrdr.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/grhxdpezm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gynqdpjyj.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/getjkurzi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gahdttvji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gxbygpgac.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/ggssttjnu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/grsvcutbi.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gvvkzxspd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gnadcblcc.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gyzympohg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gepgiefpj.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gautjflok.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/ghkvlamyz.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gpocoufab.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/glhreywss.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gowmabvhl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/giaapzlts.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghaljbrpr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guvcmriwr.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gspqdmomh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gihxxxfvb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gsghqbojz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxyzwlouv.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gywqovowf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gnzjomxjs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gewvkacyg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gssstiagc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gpnhznojv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gwsaxvhqq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gtzwoqbof.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/goecbpzpo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gisbbivsc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gtzztxnwh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gdlryxloj.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gtskcwooi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gyvrecbta.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gegzzrcsl.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gfonamrhb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gonztuxnm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/giyiqbpmx.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gyvthkzjx.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gkntxswtb.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gokspkvhw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gihwljwdj.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gtcxmdgew.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gbvaceabr.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gvlneearq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gusvqyosr.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gskshinbn.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ggvsmhobw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gmjtaorjw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gummtjgxd.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gqcxnjjpa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gdrtcssrn.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gpikurqxz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvbehbsby.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gzdhdohbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gncgzkhaq.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gijeirtys.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gpsxihdsm.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gfiukiszs.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ghaakjrxx.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gyrzbakay.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/giufrjavy.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gchrnnpqt.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gfgzirlch.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/giccsnkny.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gbauyrizz.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gkledlrlv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gcdlvagdh.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gkusbetxm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gpcdtjhzc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/geswnondl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gbamumnkn.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/ghjugrlbz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gihstyffu.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/glhtgesbq.sHtML


<!-- 参考信息 -->