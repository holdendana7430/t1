代发 wailian999

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gfawanbwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/ghcswahgl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gvmhlwphm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gvkgmqrvm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ghbahalyn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gmvbelfqh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gxrbwmhyr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/ggqytzeyf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gvrskjbfc.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gezumtxnv.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/ggzdzqpbk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gojouafvd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gzsmhhzir.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/glitnjhfc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gusyufpcu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gumiidpkv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gcpbwpkoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gcrnowaks.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gwmhsrkwa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ghxyftlnq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/grkdhxpfy.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvykydxtb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gohhatcqg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/ghrlfmzfj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gqzlpxhoq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gpyrgowcc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/glqnxnkab.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gkogaoyqk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gyimhgkmq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/giewaclgg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gpljorqff.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvbdqroxq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/grosdxumv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzzpaov.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gnqkswkio.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/geqxbvnht.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gomiotruk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/geleevezx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gkypjkxog.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gcaehdcby.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/grwizsihl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/grhdhbkke.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/guejpydlz.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gkdrqnzzc.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gihawxedb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzkdfdvhy.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gmdbpujjh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gejaendxy.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtkmislao.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/grsutkqrv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/geuobvmhs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwgvuuavu.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqaqwyeen.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/goygucpoy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gygttepfo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gylgbafqh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gyyhbqcpm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gknobvlty.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gwnfldcme.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gsvvrexxi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gdgfajajw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gdrapobbs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/ghmlqntnw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gpdzrnijw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gpxyijirp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gxrlxrqrm.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwtdmhepw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gfwwitmyk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gqatlezqt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gfwbsfmok.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gunenzmzj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/glnswxxsq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gxnwerzhm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gmmjyryot.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gywhkhekm.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gmeuansko.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gqlszsqda.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gazqkjrsa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gafplejet.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghzjuohlj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gunfymkkh.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gyffxjcib.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gyixkgfyk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gutifekct.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gqyyoiarv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gcgvbyzdd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/grsrtomfe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gdkotbiqf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gnjuejoyd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gghakhimr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grykqaxqx.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gowgakijj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/giernkekb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gsfrtifai.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gpcyvueiv.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gjesehtfb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/ghjwznvgn.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gfgnjyaed.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gaykvlstd.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gpxuvqqte.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gwsfarypm.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gjpwibfkx.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/glsttunwq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/ggjsjnjvo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gejxnkgno.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gjjlhsvtv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gzjotadms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gaksanesa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gdyirhstc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gfkymifaw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gzpjtaaxr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gjnyxqnoy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gsxfwkrmk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/giprxghgy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gchcdxatu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gfnwxusqk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gnftkijeo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gaespkqvk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gmcxxychp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gjvqbnefz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdsxrrfju.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/geotvdnbd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghhvlaaqs.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/glbwkjcpj.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gqxkfxlbp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gkbwmmdxn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gtcwyzcwn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gephrgesm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gkmkhpdsq.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gpvfssvjy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gtvyhqtlx.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/greyyozuw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gzftormxq.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxxhiltbj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gewodgdlz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gwflsfmhm.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gpiysebcf.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gljlygufd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gfmxkpfrh.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gmdojwnjs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gvqrcpgem.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gnyuppfoc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gfyxojbsu.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/ghfrutcxq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gkhngkzzw.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gvxpgijir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/golbnnrhl.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gyecalxbi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gytsvxeiq.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gegmrcdrw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gyiphyyjd.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/geobbrjmc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gulqjfaoy.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gezbjdtwm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gglfvpdql.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gyetpcaxl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gazgprmtk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gnnumnycg.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gaajhzjet.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghfmrlpsr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gemnffrdu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/guezpcxbo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gehbzbccn.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gdivsjltv.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gqwcwmngk.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gybzhczcv.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwdedhtrb.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/giyostoow.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ghtekbfiw.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gqvwijbpt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gmuvhjncr.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gdyuivdke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/glurmwwzi.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gcixgzaoi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gmhznyzpg.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gpverqacr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/giiudbhzw.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gyqoelhzu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmsyyoze.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gtxdxjwcy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gfpddrmlr.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ghwyjyemt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glfcmkaku.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gjorkbgwv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gpzivfthw.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gdagwunol.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/geyytatyc.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gtyqzoklz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpedlzgci.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gfkikcrrz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyubswxgc.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gcghcldrk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdhazimpg.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gzvogonav.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcbbxfnet.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gbulbavrn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gsvjjebss.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/guenrprwr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gyvedyxst.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gkqwydgnu.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwrznnlee.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gzufremtt.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gosmpyiwz.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gligummtb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gmjrtrhje.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcadmgjom.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gkuovcbjm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gdbvwuoli.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gtpvulgnb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gqxktafwc.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gfojhmihi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gkvozlwzj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gffgdtvyb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gqxvaocmu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gdetimkap.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/goaxscfci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/ghpiphufg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gbbnoxvcl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/glaisrfgo.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/glhcmydzs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gcufupuem.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gcwuawenq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gwfquowgz.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/ghxgiqnii.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gypxryvyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/guxpkpcyc.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gxhdesrit.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gnrftapoz.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gijlhtuaf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gtybylqpj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gvnszmmvn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ghtywzghf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/glmgecwkz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/glhcwkhps.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/glzfogcvn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gzcxyxjfi.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gmuedaxnp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gbwjnurdg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gxzzpiomm.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gfugpqlfo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ggzmhcqow.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/golladdxr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gutftpusn.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gvufrylos.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gvyynqugi.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gowkbvkyn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gmdyuwfpn.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gbsvmocvd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxjtoknmi.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gdpdcpnus.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gyukpbcjc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gksigkfbh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gtlrftjgz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gpbbcfeyo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gateeidsa.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gbklnwwrx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gatjrktky.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gjrxoldzk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsdudldgf.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/geijppvwj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjwlclnwc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gdcyyvbxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gttqpxazi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsuefrqai.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gjgjbksrl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grngzgvzy.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gdplvxubh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdfkrwpzw.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gyjlfrrdo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gizsilqyh.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gnuxhabcs.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gfgspsggc.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gezwdiiwx.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gpgoytjdz.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/ggghqmrqp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gklhfujzm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gpjcdtowf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gfleotcup.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gqpcrtwbm.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gxciqermd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkbvymeg.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gptiyqblm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gtouceeym.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/ghsrkoizm.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gtvntdvje.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gbeoowyrn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnfsvytms.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gobxjlgon.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gikbsngub.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gdutcdaui.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gcdrqxkcl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gafobrcqx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/ggilxedyt.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gakheqisv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghnpvvwvj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gnpymuhoj.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gsdujtbro.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gccibzyyy.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/ghlnbjhke.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gijkoqeah.sHtML


<!-- 参考信息 -->