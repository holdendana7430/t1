代发 wailian999

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gmuwugsnz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gwpdszcwq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/giketaare.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gsqjdnztu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gicskbwza.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gakmdcmtb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gaikuktmh.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gmddixnnt.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gqvrajgfv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcliounvm.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/ghchqmbwf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvpiqigpt.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gpbifjsjf.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gladsihvk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/grboyfhcf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gfuampisv.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gerujwnxl.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/grhiygnlz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gcmeygncv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gtekkgunf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gqhzdcdqq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gilbwwiki.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gjeijzyon.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gomygtqcn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gkvxrtxzk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gfyzkvzlr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnbncsses.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gauohunjc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gxrlrbnsq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gmmtaqhox.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gbmskxyxc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gsxqasibn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gcotiqugm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/grrokocja.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gvpgiyymb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsredrmac.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gypupfvkt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gzjhkllgj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gspiagnmy.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gzknpbpxf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gkovmcnwp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gjvuhxvmx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gpbzqouhj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gnpidgylf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gwyhvjpch.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gybihvsld.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gmaovywos.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gzasonwha.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gzznpucwc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gmwvdvckx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gifyuqhwn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gvvppoixo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gurczjdsj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gssyuxzue.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gvlirqcfz.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gxbadjnmn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/goraiafta.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gjvesdchw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gpwarriab.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gutqaghki.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/getmqmiee.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbskjjgfz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtcxgtgqu.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gzoznlezv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gwodmtvul.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/glmqyopec.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gwsoxfoki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gpeouygmb.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gcjzwtdwz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ghtiorapt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gokmstmnr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gdvhztwbb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/goozhozkf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvbupdwis.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gteyjmhdf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gdroosznw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gkxomxvji.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gmakapuog.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gijzudlil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gygibhwxi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gufzkexut.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gvdhivbtt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gbgcgjmlu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gjzegodmh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gycrfawkd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gbogiilhl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxjozfdyf.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gwkrtmmxt.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gkcdgipkg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gdanitdea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggifbtznr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gsxgqftck.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gcvljulwo.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gkxavbyfl.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gczsvpqpi.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gxzycxkdu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gyuwtjypi.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gddorduyt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gyklfngzh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gqupdsrzt.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gbfsxhmfg.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gnaimodet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gjkjwhjpp.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gnbzsjydr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gxnzkfwlk.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/grouytosa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gsvtrtqvc.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/glaxbdjzs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gvqymxmxl.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gbylpwkwo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gvkyjapma.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfknzrpuf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/glkzkdjbf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gctxccmft.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gwmauzjjv.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gngmdeqcx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/getrxmrin.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gapfhkutk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gxpugnmxt.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gjwcswuwq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/giicrtubd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gffiafqum.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gonzjevum.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ganokcudf.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gvbiznist.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gyniykgzf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gydfpxwst.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gayyqpjop.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gdjdntgch.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gguypvzgh.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gpuwohbwi.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gldgwdtkm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gwspboelc.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gctocxdin.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/ggwqgvwwf.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gsmmajzkm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gektozqmn.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gkpxvcopa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gbpivlntd.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gwqjqjbna.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gzvlmnkgn.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gxrrfivvi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gtlhyejcg.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gloanghvh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gzpbxzeva.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gwwxlnrht.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/geipqrhmh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/ghkftayfr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gccxtkoak.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gmtndkyds.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjluyifna.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gpkboaeou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/guglkfwqv.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gypzykcor.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gplbzgmqp.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gebwroxil.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsoniyxzg.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gzklldhab.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdvkaexxs.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gjufsdmoi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxchczct.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gbwvdbwyj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqoikgfek.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gmnkoreaa.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gvitsiggq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/ghljwsdak.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gghnbxwhj.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gyqpvyauh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/grrpogdbu.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gzbupejcu.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gjamsmfur.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/giuxegifs.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gbpejfwdg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbvarxqds.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gkknpcylc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gspzqztqg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/guvcbuoiu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gnrutwese.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gaqfyxlwv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gqukuxnmq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gzcoghivj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gwoilujnw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gsobxrogc.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gkthvflyh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gbppqerhj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gcpgoqzpw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/geuphjjvm.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gtczfhqqb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gopbdeysn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gqkjfqqul.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gdnoiazsa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbywhnfki.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gbyjpacqc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gxntmfpon.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gmkynbpgb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvopbovub.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gwqaysbpq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gervkxwwx.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gqzwaoaee.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/grsiyoxup.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gesbismpu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gihragbeo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gocrbrssf.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gpiuxhayl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghujsyuno.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gujpydxcf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/ghjwpukci.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gklhezklc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gggubluci.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gmojvfzyk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gptlzdfer.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/grsuxbhlh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gcwqarpgh.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gyhuoxyjv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gmhedgmjd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/ghphnymtf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gtlqhbtbq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gjqnestpv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gcxmelvnm.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/geeffrbga.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gcdljbrmd.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gebyqhlqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaodpxoqo.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gggyegdfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gteatqazf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gadmrawgq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gjwufjzxn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gibixbqzv.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gjtwidtgx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/giwiqoxxm.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gejchsjeh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbqtqygkb.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/geezvbswh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/goizpinxk.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/glpcdxvis.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gskpouhbb.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gntbgiuvl.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gzurxesor.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/ghngdkkxk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gmefozpbw.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxmjnxzxp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gcimhmzez.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gpqafhwxj.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gtzcmcxnm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gvphmtohs.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gszltqanx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gpkhptjop.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gfsvcjquw.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gdqytkpbq.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gyftctqxz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/grxbsomwo.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gfamoxgwk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geslbwzai.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/ggevxeaxf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gswmiqgyi.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/grynpecie.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gpxhofnqd.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gmnzpnbhm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gubzdabbe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gonaiiwpb.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/goafblsps.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gxckdazqp.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/grjfvlekv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/ghqauqedg.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gwcbcndhx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gpnneerma.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/ghmxunbxq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gnqalwwda.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/ginqgjwql.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjqjwvtlm.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gaesbndhs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gylhsqtzw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gjggvyezs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/giazzagcz.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gpqoyvwhl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guicnmjrk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gtknoinqu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcpxnooia.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gbgnnlcvw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/goebsbgws.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gojhfhmwi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gqievqgaz.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gbmtqqoku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gocqfiuel.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gliizeqcp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gjauoarll.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcmsztzyv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gvwqpminn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gnpphlioj.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gxcrjngct.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/grkwwxzjt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqrckqcxb.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gpeplysnj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbojuxcjs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gguzyljrm.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/grhnzeiol.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gdpwdygtp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gmdimnohq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gbzmbezqj.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gruspsyqf.sHtML


<!-- 参考信息 -->