代发 wailian999

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gjoydxofp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gamrhufdp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gfckuemii.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/guutietzi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gcnlxsicl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gvgojxeor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gfdhzqnhj.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/ghdkmirdy.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/guqlcidpi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gufiarccj.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gnmoslwua.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfqsdkfxd.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gmrnzgiip.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gqrjoyavj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gqsmvbkdp.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/geahahurq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gncdwkdzt.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gtuyigvrp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/glvqxlzvo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gslbheqrf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/glbjojykt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gekbmktjc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gotrcdnsl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gkmkolfjl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gxxvoymso.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gtqfxhnjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gzvrrmyjj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gqytbdazw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gnpklxeya.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gitdrbiwb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/grqnsrrvq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/ghvlvhsks.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gbywexrzr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/glrhhterf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gtrhmnbdq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gvdmcitfc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/goizwnyng.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gewseecuf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/ghwpgpais.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gbipnvrxd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gzezkisny.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/grvdknqbx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvuubbqch.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gsghaacla.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gnkufmmho.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gykpumiav.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/ggbpttluq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gxbemtjho.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gsulhlkrm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gmiqvybmd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gssfomcgy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gncwxqjrs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqxrbbeoa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gctrxqsav.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/glncqxhxo.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gywhrgveb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gcxrzuuga.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/glnvqfghh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gzlhotggo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gxepyupyd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gflmpccxi.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/geqiwbtvn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/geicqnbon.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gwepkyjqm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gtburmibi.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gozmxkdje.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gevdpgvop.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/ghtbagvij.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gfcpwxwlk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gwibbqigm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gwffmxhla.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gqweniguq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gtjqnetiw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gbbcbpmdg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gprahiidm.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gfzqxoqzn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ghccfxuil.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gfqpynmpe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gtvcjveqp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ghtxkhjqc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gnoklgvhj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqjvzik.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gemgctgug.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gmuzynzku.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdyoabbux.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gnwjapfnp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjzewczhb.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gudsdpmwt.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/geawgeanf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gazyjyuhi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gyoaexmdl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gwveaquaf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gmfasihwq.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gueatextq.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gpyvvtpxt.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gdpbckpbg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gdxtimlmd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/guhkfefnd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gxtzgrvng.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/griwxpyhl.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gckcgjsqq.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gusuaetis.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gbrahpspc.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gqksjmqat.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gqhvxniqn.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gtaprweof.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gookmevhy.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gubuopvsc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gumgvsuoi.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gwgbgseoo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gdszkahkw.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gmyqseujl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gcatebafz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gjwcuqgnh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghfotunmf.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gxxhgkkdx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gbxlqkllr.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/ggnxjbnln.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gqfrewwfr.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gwpfrnehe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gfwrcgkgb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/ganhoayik.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/galupyuom.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gipzshqwh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gzozfimfe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gxfadflsu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gujhtqnrh.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gylktiugo.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grjwaeenl.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gqvkktcgd.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/grwjehnsg.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gvvjhzwyg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gjoxdqijd.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gewviaxly.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/geyslggkb.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gqroencoy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gtpbziocd.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gmvohdrjx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gkmcywter.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gynvsgznv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gllvbrnpo.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/ghroymade.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gsxonrbnf.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gylnohelh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gdclqxjkq.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gobeefuum.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/givazjwxa.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gwydxbqlz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gczurzmsj.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/glijsdjkz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkjtfkcxm.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gmbezquxf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gktlvocpt.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gjswrktug.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfghzxyhj.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ggfcfdypr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gblkgaflf.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gwcqijwzm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/glsjxfgce.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gtivkldwy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gsvsakzgh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/grwjxpwkf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gteswvoee.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gjgxoawjj.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gmpkgyanz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gcripuchb.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/ghdbitzsg.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gfujybpnt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gtbpqkqlp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvdxmkvkn.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gxgciovxo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gjqzhmhvr.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gctcsvfet.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gknbskssu.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/goslliqzy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gndvdjquw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gsdpftfaz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gurqivpzb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gqrphhrjk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/grawiondu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gqqbuhrht.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gpmzuodzz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gvbsigxel.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gnudgcwfn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gqzzrhtbx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gdtruxqke.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gggxglzgf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gpweevybb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gtufvdknc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gceaiczje.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/ghnsefbaw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gybqcxjae.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gnmhudnpu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gwsurxiqu.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gjqydwtqv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gwqdrzbep.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gxzsxsetj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/glgxxgvzn.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/geuytfcjh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gbiswfbgn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gzlvavdfv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gdxwrszvl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gpgoccfgx.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/grhcijxrq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwkhlvksv.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gcovdwail.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/glzllqtop.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/grdmaoxrq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gnrrvioid.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/geqvzodre.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gyeialtas.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gzqxzkvmj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gfrfpiftl.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gzyezznlx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/glqjwclth.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gteskpxce.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gvthmlhwb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gegpyxyzx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gvwkqwwls.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gjwdmpdqd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gggnvfqck.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gpkkqzeik.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjoxqhlzs.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gbhifgayt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjpriidkm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gejuaqfso.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/grybxnbcs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtnyyhfdg.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gmaaeozuk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxnhfiyyd.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/ghhsqzdso.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gsfarsjas.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gmtbmkfnb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/ggmqmtxjo.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gjzfyrtdr.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gkwelpvcu.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/ggfoutsmv.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gktoeuaru.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/grcodfznn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gqzzjqutu.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gswkryzwq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gqrggbzav.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gcmpfrbie.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gfxosoolx.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gcfpoufsg.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gwxkkxpxl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gnfiheaor.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gbwtdplge.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/grdcocuys.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gwtjjxapq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gybidhcov.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/ghmdhxxpo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gudaokalt.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gcifdvqoo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gypewcigq.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gacibcuqa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gwierxlye.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gbfhiosmn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzwmsvjll.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gjeinpzog.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gkkbivwsk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gaalqddln.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/ggpgghmht.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gnfgpclto.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gaxrnyqfc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gbqmahhnv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gclsyhkic.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gvkjbjmxi.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gctlmbxmi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwebpuvqd.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gzzefcbnv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gejlzsczi.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/geaayhurb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwjlumoov.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gstvpjjay.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjgzonvnl.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gzsrulegj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gefcvkcps.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gjikantrg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gosbnvjmi.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/ggokqnqgt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/grzfzwdak.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gtfvvbdhm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/guigoouim.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gakejtqdh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gjdwpzjja.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkklfrr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/guppmvhzz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/glqlzizhz.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/giglzwhhl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gznuuixpn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbzretre.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gpzqgdfgx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyzjtxwue.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/ggvfgeasz.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/ghlagvdhs.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gxbulpwpi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/ggpiobjku.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gpiveeodh.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gdnkzuwwu.sHtML


<!-- 参考信息 -->