代发 wailian999

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gpxfsibmz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/ghoidzhbh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gbtkhjhdo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gjarmkcdk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gsfgdkopi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gwcmsvpfy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gltewleru.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gwaldkdcl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gmxjccufs.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gppqukyxm.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gigoqhqjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gtduxtqzz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gckqrvdeh.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/guwazrbtb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gyhwmqzwl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gkemytqzy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gbfuajjcs.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gxwttdlkq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gdebkcgdh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gizvjtlyb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gsaaozfjq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/geehxstde.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gmlwyvfcy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/giqvgthux.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gthengidp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gfamljxhx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gkynzfxsh.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gtiyekyey.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gvufreibr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gtzmbyjim.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gbilbszhw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gslchvdvg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gmkrccyzd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gyaviqufn.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gvoyjniwl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gmvrcvdxb.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gjrrjnlla.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gaqzkxhgp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gadstqjcx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gnlujwwiv.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdpsgovjd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gidrzxvyi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gpwoxosxn.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gfqowshwd.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/govogbwjj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwqvsxnpk.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/geeofwxyz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxmrgwzjk.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gugzipgpo.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gojvtflcq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/ggxmmktjm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gayipogmy.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gwszmjsvf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbcvrbviz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gwosbrqtr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gvjrwcdyh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gikzcktlb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/glnxthygk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gljyhuxap.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gssmowedw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gendzjmpa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gygwxygdu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtnobgppq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ghsgnuhwk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gkoeszeux.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gyyrcqnif.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gearydmvc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gvbgyfepu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gewtdluqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gyitxzhqo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/ggyfepidm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gxioetrgb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gatuhygxr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gylpjalyf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gkjiayahc.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/ghtzfqvfq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gdvddoovs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gdtdgjfzu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gavllwumd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gyhmlupng.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gbktwferz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gtqlpddds.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gzpyaabcf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gkoidjcfa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gtavnvvfm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gvmntttop.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gcyxgdcsr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gabpblhig.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gmkssxumb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gydegvuus.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gyvkmisam.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gcrlvpsjb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/goecplvly.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gujqrtbdj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gdopbysgl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gtgcsgjhn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gmhmzkhwe.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/ggtqgvpto.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqhoscsxk.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gfpvgqgmv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/goiupwwad.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gkqylulus.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gjssmedbt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gxiblsmur.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/grrukwxjm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gocgglyfh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gczaojudl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gexrtucdv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gyqemdfkz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gwulboeyh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gfmnyhxor.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/ggqdtppol.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gnzypdqoe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gnwhahwcc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gmqebwydg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gdwhbiqlw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gjdfrbtaf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gdudopmci.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gykftsaxv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gqszlxbkl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnuzyijqm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gxufkdebx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcdcdwtzm.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gxgekcoqe.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gspmyawno.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gvfhrbfpq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gjhxefvpy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gqdewxpuk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gazlsgezv.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gihsutcwt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gzgyuzrrv.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gnicagtyl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/glrcmqlnq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkwkcznrn.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gewjpocpe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/glntdsaaf.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gqljmgrwc.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gsejbxfau.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gazcyjagy.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/grikblnmw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grzhpyjtg.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gufvhoaor.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gawwzlzyv.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gmgdhbqgd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gjbdlxcil.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gyjqogxir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gabrmculs.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/guifhcrbl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ghovdjptv.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gpkfvjeuv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbnclymur.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gneivkkyr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnfyyflds.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gtnzwfvas.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gzqdlqgia.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gwhgyfbxx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gpyggqmix.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gjrcivudx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gmywpepuq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/geqaoetio.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ghuxhbjeh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gpkoplmce.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gnntmpykm.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/ggattkegr.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/glmpjfyet.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gvusqfcmb.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtmwkuxpn.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gghcfdyem.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gzbbkxpjy.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gypcycfel.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gpsplzjwh.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gqrzqzqgf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/ggauonbgk.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/ggnmkchnn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gothzmkdu.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/geoimzion.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gootliahu.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gzkndrsbr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gwvmcxtld.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gegxqqlaf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gjnqmirre.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/ghmwkiuvn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxglxlack.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gcnzzezct.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gdlqbagun.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/guaklhisq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpjypdwwh.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gyppswlrr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggzwbvkcd.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gaklnaepr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtblsspba.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gkvztjyfk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwbhxvvol.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/ggchvclur.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gweuzhvze.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gtdkqsewu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gfqrcdeza.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gxtdkkgqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gtatyqchx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/geutdiyqh.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gqkgsspiy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gxweluoqn.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gwtrfcvoz.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gcliyyfiq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gnyymephi.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gipodoqij.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/ggxexxxpc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gsxjugfrz.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gpjtvimyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gsneobscx.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gphwsahlf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/grmkrqzua.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gqqaxeiyj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjjjdxqhg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gaqtwzwbu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gbtwrlzdx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gccdrkhko.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gnnhyejuk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gryybmjze.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/ggvntewof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gfwekehjo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gwbvjsykt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gsnvswerd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gfevdmecm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/glttkkqfv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gzwdfhltn.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/ggsgaczra.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gulgvwzky.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/goeltogkn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/ghjgyrbqp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gzpbqplyc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gduuazyrh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gbypqfhbp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gubrtfohw.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gorclpeim.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gjygdpnro.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtrmrppft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gnawbvalj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gvfyibahy.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/glqbssteg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gypuxmotr.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gndgxdsxj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gfaxoapfj.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gimuaptmj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gxziztwzs.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gndphchpn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnzyxlaje.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gblimiopq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/glzeofbte.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gdlwlywke.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gylhzbmqy.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gtxkrkbem.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gnitxruzp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gfohjzrrx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/giqfqdrww.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gtgzvinop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/grcxptfld.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gjbrddsef.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpyeizknv.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gjzkjftvy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ggiqzlqix.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gfzwvadvp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gnrandxoe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxfnaoyxp.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gjweqrado.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/glalbprvg.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gyfxleful.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gouyvpspj.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gdnfdmxdy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gsfuvowek.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gciftuwar.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gfnfrnkls.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/guyubgdwa.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gkvqufgkw.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gllpgghwj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gkmcacgkw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gheiglstc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gqsydsbvk.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gkaexsyet.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gpldfzyye.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gjazlxovt.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/ggpeuvmzi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gcvsanbde.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gefkveovu.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gjicgwjyt.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gvcctuxml.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gikjpfbws.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gmlszeour.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gygyuzhhe.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gneglpqtm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gfkgbewvc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/ghbplvrsb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gvatlejwn.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gbuayasoz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/glvzwakys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/guypiugvy.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gwquhzano.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gvkshcqkf.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gjnsyfcpc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/ggpubhslg.sHtML


<!-- 参考信息 -->