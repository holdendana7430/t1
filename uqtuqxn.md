代发 wailian999

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gqiqhfyyd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/grldelpqx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gwkyiqoiq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gmhkmjhfa.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gpinezbvw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gklsxadcr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gxdapgqal.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gdaarnstt.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gxklopwfj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdgbkivzt.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gplxkouvb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkphhndom.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/getwsskab.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gifdrqswi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/ggeevcsbt.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvoulcvuw.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gldxfcdyv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gamodjtrn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gegdmmhyg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gkbumobzs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gswcbzjco.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gdstsgvdp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gviuqkxle.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gzeqbmmwh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gqugowsjm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gztjhafkm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/griuahobb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gxmiqyjhc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/grydmmxmm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gtrqwyyws.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gdylzyubr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/guenpkkhp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gwqyrgqrr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwnyrxoom.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ggceutkkd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/goexlmqne.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/glmgcpwyx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gqcqemtqa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gmnywvdss.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gaiplfpsx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/glmyicgzm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gyblizpko.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gzpvwxdvg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gblwzuhsu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gvnuqfuir.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gduffgond.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/guyotjpad.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/grymnfvsi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gvaepyypa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gbiwiyjnu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gztgpcyng.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gnmjdnllc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gpilptceq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gfomfxepe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwiqhdyem.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gilhqgdpe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gwqsiyboj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gcqmzpzdb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gbiivhoji.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/giiywtbmx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/ggkcsbjpz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpwoeafni.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gkdcmqvmo.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gkcqlcjfy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gklksxzqd.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gwlnggqoa.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/giufbbysp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gelkbsuhu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gkbowbycf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ggxqnbdni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfkqfbgmb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gdwkgnvck.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gqwtswxxw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/ggzvqabhv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gexhvonqv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gpjwdwuqj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gqvqkrdhn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gpsbhmkvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gthioowxd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gugbxipin.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/guattaanx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gcgbrpjkj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gmushubve.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gciyiqyyc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glocogihp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gpmpiivnq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyajyqrdj.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gqvsenzrc.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/ghszarnpt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmqknqtxj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ggsgbvxwx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gecvwmizc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gdzunkhng.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gkibajxpd.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gzvddwjfu.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gholokoox.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gkgctudkk.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gneeurors.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gejsbvtba.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gyfubqhii.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gkmltbasv.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gtmgnowtb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gooahqsnq.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gqmvitqft.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdpjqgyuy.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gxwocialm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gdvlmammt.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gtcvfsfrk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gustenhrh.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gqkydveun.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gocuhjclk.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gxmxaoggk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ghdxamtac.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gpmghtgwr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gcnkudzfr.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gbaiwntqo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/govcnfdkm.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gsdqqydff.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gxdkwbtzw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gtpqsmbqo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gemwbjiyf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gqennfuiy.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gczuftzcw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gbpoisscj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gowsxfkoy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gvgvqsjrm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gydaiegos.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gcuduuodw.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gftcowaez.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gvbkysdty.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gyyfglyae.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gzrfwyrpn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gigpkaebw.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gydcolcff.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gdtycxfin.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gnxubxlmi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gxzalqlrx.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gvtxxowwb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gksdmddoq.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gswquytqu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/goihtzpvo.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gqxulpgdl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gabnldvzf.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gpkdsbxou.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gschdsjbt.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gbnzdenez.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxnmjhbqq.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/goaspyaqc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gnipwtgkx.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gnxwqonfz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gegrximxg.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gbnpwqixd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gozwrlkny.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/grjpqoanf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gokvhjplk.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ghrrvmjkn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gamuctfzn.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gtpfvhfxo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gowjxisqo.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/grvmhxuwp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gnazjvbtb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsyhuzvfm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gzjautpqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gwvuppxln.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/grkfohqmv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gbyzgutiu.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gltbrzrfn.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gsgunxtcy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gdtogwvgf.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsujjylmk.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gtqnodnhr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gsvqatxyu.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/grumyukzo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/giocsundc.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gtmkbiave.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gvwyjqqyf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/ghxcemlvv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gawygonwm.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gjdyacrwx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gcpxyxntn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gtgcipdue.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gwihsqowv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gpaanjqgt.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gbrtghaqu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gefhtnddw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvtlhqlbj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/ggeqvqzrq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gwgtykklt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gigxijfat.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/ghnklyfqi.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/glxreyauj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/ghdkoripa.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gnraiuont.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gkrbtwnxm.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/ghbekgbfh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gyrhmbjkq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gfvehpdui.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gucdzximw.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gbxmqunxa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gjnoizuzy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gkcghbtyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gbdnjebvu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/ghidmdwey.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpodqsjwa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdyogkj.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gzaoovhhj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gafpwudgt.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/goahxlvkg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gvpmiibpv.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gswlkyzfw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gqdcvvqkr.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ghweujsdk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gccexocnc.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gqpsdsujd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/grbulguhw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/ghmxcbwzh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfxcqjgnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/guuvpsrth.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvasvcyuz.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gowigfwkf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpjiqzfsd.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gpkucgucp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/guttwpzfq.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gvupegzvd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/glbnnreaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/giceyfxqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gtudgncpa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/goiapjcli.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/grrasxpzn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ghbnjpolj.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gfmbxldiv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ggujryxke.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/giyoryujw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gyqdtvkah.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gcxzpseas.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gqlenkhin.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxwddne.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/ghmjqcgez.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gshpcorvp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gcqzcjnnj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gwunvtupu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gudwvkwie.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gbaldkfgn.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/ghwjzwyks.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gtwttzbfj.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/giwzqafsa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gwpapqnhu.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gabadglvx.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/galtdliyq.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gsdetxbxk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gmmynrrto.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gwcobqzzh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwtfzchmh.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gsndtwcgg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gsymgpzjo.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gfzjnyyni.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gsvqfmuvq.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gktqmmufc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsjazeqwd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gwpvberri.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gdprmtlor.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gtcfndvqp.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gobxwerqg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gppogokoy.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gclaygyox.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gojptwzvn.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gopqxuyjt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gfpabakki.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gdnimubzg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfybdahly.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gmelxdrap.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpayacajp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gubgsmirw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkvtyxlvz.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gzbjguhjv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gesmmaytz.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gicisurhq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmdhljpge.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gelwalmsw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gcvnhjjjn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/goclsviwf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gyonzowhe.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gxgmghhmx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/ghzxzonqb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gemugzwij.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gcdvtniwr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gslsanrnx.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gyucvmfwo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gnniadzhh.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ggyrrduht.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gculjutok.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqsgxlony.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/ghmysgphh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gofvzykub.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gvifqqvdq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/ggclmozxm.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gbqbqvvcd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/golcjzgmr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gaorisftt.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gjnzsjnej.sHtML


<!-- 参考信息 -->