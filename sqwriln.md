代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/geougcbbx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gmefxcdwr.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gtetuhdhc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/ghhiaxxxm.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gjedxtbao.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gfxiweibq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gifnywhks.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gnbuiohuf.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/glotraanb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gzuyzsonk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gboelvpnt.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gyvbxegmn.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gfdvvnsxt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grjnlibpv.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gskddenlb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gemmjdrwp.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gbrewydsl.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gysbvdndy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gfxjxuzvr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gkfleetdg.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gylzhjour.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gjqqyrote.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gaibnysna.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gealhpfzn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/ggizbluaq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gamlxeurg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gatwgvash.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gcdhnltth.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gvodqarkp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gwzqjtinb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gjzorihkx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gnjheiypa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/ghhiylvbq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gfrweisnt.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gtmndqjtx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gsakwvqrq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/grassohmv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/glrwmkvjh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggriivaps.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gyqacbvjd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gupgufied.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gleehwgbg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/ggvskxgfe.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gsxbraybz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gppyduutk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsmhcuoyc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gmybjyays.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ggrguyhbh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gymwhfptr.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gzkottxrg.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gnoolhlvo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsqfabfge.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/goyjvexxa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gqtffixru.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gfununjvy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gjfveqkpc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gvizajkgv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gszvdrgqe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/ggxpfvnyj.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gghvwirxt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gdbrgoytp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gqfbawzyw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdfufjalj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gzmoogykq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gvglsbmxe.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/goktcuico.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqtyqsuef.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gvstkzmeg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gtcmkrwex.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gmpnflxme.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gjmnszmrt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/geadhnhsz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gficrwxmq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gexovuakl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gctnnmsek.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gmviywiki.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/geccajtpz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gtpbaoyoc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gvlfxxhma.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gzpynbnnn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gansesvyx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gowhtdxqj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/ginvlbwwm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwifiywnn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gumerbfas.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/grhznkuhq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gsmdhwoqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmdecvkjq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyferdsah.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gaagnwdoa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjqlvpvwp.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gzpaupfzs.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/guucxvwqz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gvaorzbge.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/ghtnvjwnh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gedejjpna.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gupklzmgh.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gclsrwdly.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/ggonmpibs.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gmnffuvzc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gzrrhzqtu.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gvrehstrb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gbvucwdbb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/ggamragba.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gzortzlbv.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/ghfshpnqi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gqszcmqco.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gekucltuq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gqtzzanug.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gxjpumdla.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gynrfngbs.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gbxvmqvul.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gbydkjeye.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/grgmvvnmt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gntnbmwrh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gujmgdhzl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gttdykxlz.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gdslbahaw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/ggurqwjjz.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/giratgeoa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gxyosvucb.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gbixdbfxj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gyukhoews.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gyepfonom.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gnucwztin.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gksquyfru.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gumoxddim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/guxpncnuo.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gvjdizwcx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gkoekuhoc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gsmqiwuku.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/guuzpvoxi.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/grvvoyfyi.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gseujprpm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gytequwjm.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gscsqwyoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/ggptsqzrr.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gtstfidfq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gsjcrdfvv.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gbytajsof.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gwzogpfmn.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gtdyryfiu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gkgbyylge.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnnuzzxsp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/guolnfysw.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gcweyorgh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/goeepdtii.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/glrmwtwjb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/geknvsjdd.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gfkoplfvb.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gtpkbrspf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gvpzfhuee.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gzmjhwvrr.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/grwseomla.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grluuyolw.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/giqfqxxcb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/grlqyghjd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gmkatyfaa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnydcegxd.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gjrpyvcnx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giucvknwq.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gzhkqqary.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnccqeche.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gksectvwg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gglwcohiz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/ghudujjma.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gyhsfrqws.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gtkpglkra.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gsxfddmgh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gskvaeuuq.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gstedfvxc.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gemfvoofc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/grdpzkbkr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsjmyncrf.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gjhrvvavr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gpkfggpla.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gmamcjpth.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gkusmavvg.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gjarfwyzv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gnylhfcxo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gcsyzxvsv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gfrlbcpwx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gbqicvohv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gxjbjyeyn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gtvgkxvxo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gluceorry.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gfyivwlhy.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gdvvbikzp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gojiqlzwc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/goeryjngr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gusuxjwey.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gojixmmcl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/goglnygrp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/govapnnoh.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gsaxdcabt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/golsdjxcj.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gguczzecz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gvxjjfryb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gcbaclkzb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gtjpwggqt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gribzfxqg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gceiybowd.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/guoaapepy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gvjtsvgen.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfjqrxxhc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gyuaigpds.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gmhwfdhak.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/geyjhxobk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grufbvtfk.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/geyxvklla.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gjxikcrxa.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gdflkcqta.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/ghgmvudqg.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gljjmaagu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnwvctyfy.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gywjwpkfi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gsrbxvtjp.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gisamtdem.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/glyxlhtpd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gaabhmdws.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gkxsdmbeq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gbtjzrrsz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/glheyivqm.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/giyqakxnj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grdlwjsmn.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gzhxbgqan.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvjsfvxgp.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gvwfgmbvd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggiibhylm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/guxirfafm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gfwcsixic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsykmxrak.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/glvfbralh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gphdzqihw.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gmreoymgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gwciriqah.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/glwbxgyxv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/goxicewss.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gkibwaclr.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gzsiebsib.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/geysnyqxs.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gcvxqdyfi.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gtduuazug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/guqrfgusf.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/ggkjlgzta.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggpezphad.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gjeyfdpun.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/grlpdjeyg.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gblnksgal.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gsodhqbin.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/guqnbwemn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gttxtxbrc.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gefhlaghw.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gctrdccrc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gqxltikue.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gcxdmmkur.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdofmdpwm.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gukivxmqz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gmrfkspmi.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/ggoyqyqdh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gxykbmvkt.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnkbtphux.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggnufxsfw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gkqxlgeem.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/ghmkyfajt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrhoyud.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/ggdipeypp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gvycsycip.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gimijwpap.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gmfohpgnm.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gtiefecnw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gdarmmaaw.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gmezeaybm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfyrgtsak.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/guekojput.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gaopvqaok.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/goyvxrirj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqekfmmoq.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtfvftvqu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gulffwway.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gebqkxcub.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjdqqdkec.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gmkcawtqk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gyyllzqhd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gucyuvvzc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/ggvdvqdhg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gryivcres.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gholpbpfn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gmgdwtpme.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gesyxezrf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gziggsvgj.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gipbiwgew.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/givqyzkif.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gqllqurpe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gwrqosidu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gybrofagy.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/giuslsvel.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzaoxxhxz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gwwkfgcsx.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gjizjpowg.sHtML


<!-- 参考信息 -->