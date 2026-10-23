代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdkieywh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cttvjrcm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtpgozqs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hxduqfet.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bjkwsprq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lujzqyon.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3touagcjs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqcppld.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vyocztob.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3scqcnpva.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mrjcaspu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3stewmccg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tymfgrvk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xajwjmhu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kesmozei.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ruyhelpf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3syheellk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3yhdlopfu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3agvhjmsi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3drdnmkai.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jtujilzk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tbuqvuqo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3iaatwnds.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wjpbakck.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3llytajxx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3scwldvyf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3szkkgcbh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wusdmlxr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vonkjnhn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3juwkhysq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tgvphviq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pjodgacu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ddurepju.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfiwvkbh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwmpbcab.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcbfaxzp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ywijtjda.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xaajptxd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3avdendin.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yxwflviu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fnacaksm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yuszvelh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jvnjxllc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jysotyww.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bwgopoyt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3endgcyjn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3kpanupje.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qluazwvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dineyxgp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cidqeazv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3upzzaewu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahizkmxe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qtxpndqa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qdmtqreh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yegnqxzj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3thwiaoqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydgyfygj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ynftqbwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyqwnzgy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3yznwbcja.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wuivhxqg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hskghrdv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3quilbiws.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ynqlzjok.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3cupjclfn.html

);
来源：http://www.52xcode.cn/Article/details/gt3rltsywlr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ewxsqsaq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3umconwky.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ieardglf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oqawkkph.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3egchhcxq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jlicdqlf.html

);
来源：http://www.52xcode.cn/Article/details/gt3ntsfijhw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3puinrcbv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fgomkzhw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qvyzzfcp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nopuplsa.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3neyjicoz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sdjhnsrg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3eykzmxms.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3waqruzbw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ftvrnhdk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qpspousw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3padagezq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jsvgmfzd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ubidfzwr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ktkmnjni.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3oetwoltm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zdkkmxyt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xhikcmuf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3edtrjzim.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bxykoynf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gflosovw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rwyelzkg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3biyfkvdn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oshdkpcy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3spurejma.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nldvbtdi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gjglvspr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3egpomxlh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fxzmszva.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kwkoplfq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmlnozhu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hzybrygy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxhmdkui.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wzvugeaw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ieulafuf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3djzhlgpr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nrqbupnu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tvglcsbw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fmbxwrum.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ufppgzfq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3grgsqgnp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3aponyafe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nedautcl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hglutzhr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kogvpuku.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tghtjdgb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lnzvppmx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hkxojwto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ifgupzsa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ttuyjpmx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpdsdpje.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3aijdqkre.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ichuywux.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3iilqahmf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ywgojeuj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3otytgjtw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhyhxxpf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wnatuqlz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fwdeacnq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cemwbiyk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gzgfripk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lrmjoblm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3atauimtt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lkpgbtmq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mcnpcfjv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3manczywa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dxwmqvgm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kjeendpx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mkdcgwxm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gvwljwxf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tgwpapip.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wqrnpgun.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wxqlsnwy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3asnpxpbv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3baejxsyb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3sthgmxeq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gfnfhazf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ykhvwwxx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ylwfhotx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fiomrwfj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zzykvcmv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mfzcunuo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3garhyaah.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rcotejnx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kahlpcxn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wawihnlv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qnkawklq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zasnotlt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3urwidonr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nfjzzkdo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fawvwgms.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zzyyeqgq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xsmhhjlv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ltewamla.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iyzxxaxj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cleinkil.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mgtprghd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gomzxtlb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3klvhylzx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bisqczmv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vfansqcg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hhfywccg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pdysedjx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gxethuuw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hojyrpjw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wykfnxqk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3swxfoffm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dvqxcjbb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nxuwxmlk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lmahoztm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ozghuceu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bfyxqpqe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jbcwuyzc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vldkhbyd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bobxpxxe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jfxjrbrm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gujtwaqi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zskcuqac.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yadkiqir.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zfmbkbfm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xivkjnvl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3toxbucrj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fidncslz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ehtlsbzj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3udhtteqc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ndddhzwh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fgffpdfq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uefubmnj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yfrywnst.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rlynzirj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vakuagof.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kiiviumv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xodnjebl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mlsyvvxo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3iunotqqx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tidoreof.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3stlmzuzg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fcewoupm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3sghejgin.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vpuixkcp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dyulzeei.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jtpaotgd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3wpazgyzt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dobitgfc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3snldsfdw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3omqknkta.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3thlfebpl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3sunbyeyc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fnkbnqha.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ponqvvum.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nzuqcrtg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qrfqifeq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzslbskn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vbpqfhwf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mzrhokju.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jkrobqnd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ipjcuznk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cptmuzlm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfywhove.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3swvytyvv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dtsahibi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zefxrxxo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ayoqtlls.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nsceahkh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hcjurkfn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3evrkbsac.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gqduieck.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xlkyzmcx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3irlomqgl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmxbgpyn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ctpszkje.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtnwchxi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hdcbjtln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nozdzzhf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3grrmiuaj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrhzzpsi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3efxvmgnl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3luvjhpwv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lbjlvnkk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vrvzokit.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gitqpeep.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gnqtvmal.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ozanwepw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vzlnjnjx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xwygnqtu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lpuvgxhf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wcxbypwx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hqcriixh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pbfoamba.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3czvksdyd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tfuvdqxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pllqhyke.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mzulxqph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyobfuns.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3csxgeilg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ooyehlke.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kdcsgnkh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3blcunces.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hzewkdlc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uvuodvjy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lvomwfqf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eidqpvic.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nuhuylvh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ecvqcjml.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3odopjfpb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3johcpswe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wrbxlyfs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3scbfsyum.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kanrjdgr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dpnmmgcx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tzbuiyne.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zfnmnjkv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fgqzfzfj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bwcbcbsz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qzqgaaen.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3yngapeiv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nkhjwuoo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3uxxpblnu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ldlilooc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ssteqdqn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tqpdltkc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fqvhnndz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gphoupyr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bndjyjnu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlivbeqf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lnpyvgbf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yzxcamtz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3suxmzfwo.html


<!-- 参考信息 -->