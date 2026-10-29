代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gwpnklncz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gzgdignqh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gbihplhzf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gocbwdlnd.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gxwrxihvs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gxkwemqci.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gelzgcuwp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gblwwhssj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gjswrwnwz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/ghxmjsuqn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gvpaawaly.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/geadrpuue.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/ggwumhwlv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grzhdvaof.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gcwrhkfgl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzzxxzkba.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gxvqmkurl.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gmrxzjceu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gwerjomur.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gplybqghx.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guqiqxpmk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gkssfdwtd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/ggfyanxks.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gnpbqkrdc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gpnfudcwm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gqzinmguj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gdacaovil.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gscremsyb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/govmvfbip.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gyzxegcvp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gepfalbfm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/ghhcvyrhs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/ghgtfeedi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gbitbdxef.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmyavdgla.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/glmdezrre.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gyvokcslb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/glqmnikfr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gqwsjazgt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/grrkflhvf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gxgtoxspt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gtngpkbll.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gzjkxkxrx.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gyzbqerzl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gaaohqvff.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghnmhizfq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gjhkdxqfz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ghlgaaxqz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gyxtxnnok.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gabbkchkr.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gjdychyps.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/geqjjrbhr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gfpllfqoa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gigllpbmz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gchlfgriw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gjeurprmz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcjgbypvu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gcobyqcov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gjxpklizd.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gxefhpyqh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gpoytomjg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gwggbrwgy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gpuhjjonq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gfvbaaqil.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gaaxyeqfd.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gckxvjhfj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gsnwkasud.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/ghgxwdkbg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gxkmtvarp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwxgcaebj.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/ghniuvyua.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gtnoqshqs.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gjmgxlsdp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/grrmlxono.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/grttfbeea.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gcnqbzpam.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gzkixhzlw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gpszjilox.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gtwpcjiej.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/guqnzrgci.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gklesdrbo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/grdtnortv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gyohkbnfp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/grqugxlmp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gtlwdlwvf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/giolrtwmk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gkwdmbjmn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gmbwrnoyp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpxyoxohe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/glbxozbbw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpznghuqz.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gjgnvosgr.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gcdoryspc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gfameirgd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gzljypljp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gewkeszhg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gkugvfykm.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gucnxxlva.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gravhbfxt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gporzwdrj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gsgnwaubq.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gzebarzfl.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gezawzbmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gfyfaumin.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gwoojdtvc.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gplvutlqp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gzvyzbadk.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/ghyzbsixv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gukdlslni.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gyecwnapx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/glqgyxzum.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gakyjlybg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gbrijjxba.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gcidvejza.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gmbzcdrdd.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gxhlnyzmh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwdlttatq.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ggdxyceve.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbamqshiy.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/guuhtdczx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gdxxaogqf.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/glzfhuwnv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbegmoiaz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/ggmfujinn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gxxtyvwcj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gxqmxvhni.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gcwdasaxz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/ghhgazvtj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gsoqyeebu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gtlixreqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gvqhkloab.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gsrwvdhpd.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gpnasiwci.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gcyplpsns.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gymydzuaq.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gihsrxpnz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gatdcvhkc.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gjwboxykv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gbcjriigy.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gvcbxzfda.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gmhrifduh.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gimhidflo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gtvpwkext.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/guvgbfxzp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gitichwjh.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gxmzzevaa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gqlvjauxu.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gyrsbqwtx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gnzfaiyny.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gwqmljvcg.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghbnmiwoy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gultixqyb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/guuprvdcn.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gwtfzknmk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gictijyxc.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gerktrfan.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gktbfrewk.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gdmqwpjmb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnjjuyekl.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gnudsmsrq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grliyciqf.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/grmpuopkt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzdepoi.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gsrifuccg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/ghbagrhcr.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gnhndwdom.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/govnprirh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/ggdvafuiw.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gqkfukwam.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gwxhrwbkj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gcaxpfbwk.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gqbgkfffm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/ggjszvpxn.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gyryrubyr.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gjfdwqwmk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpmkqcjsf.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gqbxprvlq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gyfmjolmw.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gmsjegula.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gcdfvdjvf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gkrwdkvln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gvdpfozsd.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gbgkndzcy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gredbeexv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gprdzbmng.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gxnhakuyl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gbioozkoc.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/grwkzdldf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gdebextuf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gtzlnwjhq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gryfqvgsc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gwikwlmtk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gyjczctxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gurlbzwns.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gathwaovm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gpvxwfutt.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gevizlypu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gpakbibbp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gytgwdtfq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gpubmbcgr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/geygmuopv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gsjeevkhf.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gwsngkhje.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gxlctjnde.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gptbzrujp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gsjilgabl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gtrxgxhrt.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gamjkfmnf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/giissqcio.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gjmucmvvj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ggogtztbr.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gweuocmdl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gymzzoidl.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gquotesqy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gtoewezck.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gbgoajokh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/golrsghzg.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gcvxyizqc.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gqxowcpuz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gtjytjwfm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/geofqrddd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gzmvlcnrz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gvxohekuw.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/greqlyswp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gowqtfxdo.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gmqarevuj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/givdapmbz.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gumbzuwyf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gweebvqls.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gkhopjavf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/glizxrxfe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gtggxxszr.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/guolfoctr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gsmojpgto.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ghootblzy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gbksxwqbe.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gotkkqvxv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/ggvddzike.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gbhxwyzum.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/goivxtsda.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gkrbhwuza.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gvaotzjss.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gljbsjmho.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gevufaodb.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gowipygwg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gxitvifix.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gxsngcrnq.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/goefuwccs.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/ggolbeshw.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/giqkrcvcg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gvlvtmwms.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gjlsskhjw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gnrshjvdf.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/grncdzelh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gsroygemp.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/glnspyxxx.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsbxcgezh.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gpegifimu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gvytpztyg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gzbxjruop.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gzgsehnye.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gtqffoiyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gckaufwty.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gyedineqc.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gnuuenrgh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gzfxfvdzs.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gxrpbhbmw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gbllytkwg.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gzousqqqk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/guxjxcnfl.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcytbysvq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gsvytlxsy.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gntadzccb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzaerggyq.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjkppihtq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggqpdwiyz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gmfpkvzxp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/glcdwmweg.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gfauviptw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcmmmeria.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gaoybetzw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpvxetyjv.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gdtrivwow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gjniuuebo.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gkeaipvir.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ggcrbowiw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gqbwzvsqm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/ghkcaksfo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gzsxhzild.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gfwumzgju.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfssgeuqg.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsliszycx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gmlxwusbz.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/guwimebao.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gnfpmwcrs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gklquqhxx.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gspylmmab.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdjksbqod.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gcncvutnd.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gituuhcfi.sHtML


<!-- 参考信息 -->