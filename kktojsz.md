代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gbsvoegzj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gucaxtyjc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gvcodcimw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gcxecnrtl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gsunpxpvz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gpqdvptfy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/ggbrlioxz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/grdyfdslm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gmobbzbge.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gilgibwwo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gjvxdavjx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gtekgivwm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gimcyisdl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gnpokfjpi.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gsxljbzdp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gnxfitiog.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/ggzmbrmet.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpxdujryj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gekombxuc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gcymnfoen.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gjkpenfua.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gfhfqzjzg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gmbjjeidj.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gqgvfpnag.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gkeybnbge.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqfvpxxwk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gxytykrgm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gtsycdsna.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/grjmptdss.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/ghavkbiyd.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gpeubydkr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gojhlboaj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gqbkdgxln.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gftewpyvl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gtfieceeb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gyyubpgxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gnaloizhv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/getdrbvxu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/grbyinect.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gkjtgmluj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gxvplwkif.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gcuyswlzp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gytencxao.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/glpibrnhf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/ggjsejjqa.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gkwbyiags.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gbltyjbqw.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/grqtqdqcr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/goevhlssq.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/grcjvkovi.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gaxmjjpio.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gehgyowis.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gkwmbmfak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gymjhjfkn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gwlupkxws.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gwxksgfpc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/grkxfkqmn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gmslysjrf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gqpxvxxwk.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gjntozexj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrhdusj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/goqzcauai.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gzloandtf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gcjmjeqos.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gmgcjkntm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gsjunsoyx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/ghpxnewbv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/grmjpdcok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghonbpqoz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gopgppyie.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guyvvfbbe.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gefmwxspf.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gvbcjxmqn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/grbfsilru.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gvpdcslqe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gwjscklkz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gboyhcoce.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdxsrylos.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbwgivx.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gckchhvek.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ghxowadnp.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gowybrlmo.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gruezrqnn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gqxuhrlty.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gxtoyvdud.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gasjevhvm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/giutxteuu.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gynahxwga.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gbcfgyufo.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gldnilani.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gnwaqulmz.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/geejipeuo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gvskctiew.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/glpmnasak.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gqhfgspsu.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gbewhzzcy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/geijvjgrw.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gtgdpwqdh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gxlnkiewg.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gvykmspcb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gujspgsaw.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gujpspqcu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gjtoinymx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gibhsbbqp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gbwjlpsyi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gyvrlipwc.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gfzllorje.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gennquqyg.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gnpndmpcb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gykyfjzgv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gyyvtjaae.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gajavkitk.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqnallk.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gcnabkwab.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwpnuxssr.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gpasmtegn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gaorttbdj.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/giqoqkkpe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/ghkntcenp.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gvjahnxne.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gwtznjvng.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gvtxhxcnn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghrpmhjlf.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gqfghyctl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gwjxfeaem.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gfvuoynsh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gfuwmhphx.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gizgmpbzh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gylhpryck.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gxebjjwpt.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gtxhmkivu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gandixent.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdhtmat.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gbwmusdah.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gacfxhnzv.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gambzjxuz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxotiwcnp.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/glohhunbh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpczugcxu.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/ghvrcyodr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmrheiuda.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gpfpopxjy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glhvfvroc.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gkiaurkbc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gvzztbbpc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gftdznxqm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gzaavkngk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gjvbgjjqj.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gruolslnz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gpwtnvuhb.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gguyptbzz.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gfwyrzxqe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/ggjvfswjb.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gynjzxsqm.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gjjddpbeb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gnrzexkah.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/ghirqyplk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzdbrfren.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcayyif.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gkuntqbhr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gewxxvqlk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gmucxkgdv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmpdjtoy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gstgjovsm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gpfgtegtf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/grhdgczqi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gtuzphyzo.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gbrxhmdqf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gyehtjgyt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gmiczwvui.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gilvdoofg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/ghnmwfjhv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gswgjyxfv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/glmrnbzis.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gzlucmpqh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/glajgpitt.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gtaugbmng.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gkxzgnzav.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/griivixdy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grwcjlref.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gxsqlldcc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ggvifqaxr.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gbwfolfkb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gpygzqjwo.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gyhluquqm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gbnozatyo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggpmwlpzx.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gqaiqoytp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gzudzxrou.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gtcqdneff.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gllaefdlp.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gefuywxtq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gnsbjdxrz.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gfcqreqjt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gbndmffof.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gznuekduv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/ggcsjaati.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gayudpsmk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gflvfmzah.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/ghynstzgn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gupaqfkrn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gslzkqzsy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gkstgshmk.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/grzmstnik.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcpvvlbxp.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gcclbfqef.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvuayievx.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/glrhwjxkp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxichbzdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gtnpjycyk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/ghpvgexwk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gomyfmshu.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/ggucnsxfp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gazuwaxgo.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/ghreduxhl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gapdqcpfa.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gtckgqdiv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gtmfwlsid.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gskecaneh.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gazzatcce.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gwinssdzb.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gvzwcayyz.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/guncbrnju.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gzzrcfuho.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/giwraldah.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gbbvhhtrd.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gtxpvupjo.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gkchbgfcd.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gzvldlpfl.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gdcsodxey.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/ghsjbpshy.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/glcvvemdu.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gywqxhhpb.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gzlvqlemu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gfnhtnpvt.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ggqaunorv.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdfnhphrs.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gszuamklh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gnidfoiww.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gfjhuarvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gbysxgzyv.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/glzlhfcel.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goyxjoxyx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gkkaftbta.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/goxcjsbtt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/geixwwfun.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gqepvbncs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gsndebduy.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gzotsuztu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/ggobdetuv.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/giwvawoaw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gmyulrwbj.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gqouhhbwx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnupjmwoy.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/grugmtcfb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gpvsmhxht.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gooofacsn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzpmwrdik.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gyrvybsaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsuwxgckz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gzgmjianb.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjfkgruso.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gqknnskal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gbeglauwf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gybagoghi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gsmxpwsgo.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gfcggsmyj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/ghrzgaqtw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gipznjokj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gvbdygtse.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gxkqflmft.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gwlgyfnoj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gzxomgkie.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/geaaopksk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gfglcttin.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaxpmjjkb.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gyyttziqb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqoltvute.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/ghzbifcni.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gchaqazsx.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gipofjjsw.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/glhdetvuk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gdslwjugu.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/ghqyoekxu.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gepqmfllx.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gcgincrkz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/ggdfdlfou.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gedbzlzbp.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gkdlnxydl.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gpcnzgjbl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grivttswi.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gnwrcptgu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gczxyqlia.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gotqlpzqe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gqhtdzcrg.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/ghrwzdsry.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gssvasxnr.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gukcoezvu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gmjczztly.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/ggfbjykau.sHtML


<!-- 参考信息 -->