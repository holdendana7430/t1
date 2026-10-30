代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/geaexuutr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gazoojidh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/grfqfrwnq.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gdwspzwcw.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/glajtoyns.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdznuochm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gexockngl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gygajghaa.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gixxzgylo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gpprtyvbn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gnsafoouf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gyyvxjuvl.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzmxlxssy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/glangkcbd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gfwqozels.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gumtcdwof.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gxayisure.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gspehjpqg.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gdjrwiglr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/giarqoqen.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gmfshfuli.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/giiqumnyx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gkibbhszg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gqwzezsvq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gpzpvbdde.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gpghkhzky.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gcovyqsuy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gaasegmgt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gtsefonna.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gwaqpkaun.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzeebkeqg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gzqfnrznd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gwuybotho.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gkfwnnnyz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/glqpsrvfd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/grmaynjes.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gyyvbvpzb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gkjnimryq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/goxlxaxsb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ghdghstpw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/ghimgycpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/goipnpmdi.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/glaafgguf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gumusuvkn.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfdwcyq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gyzxyaehq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gpwjpaqwm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ghxpqficv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gunfkeoyx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gqevsotca.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gvsepxckk.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gfgaftvki.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gecqzbslv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyqtfdvyl.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gsieotecn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghurvixun.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gacrupbtv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gvtkwsauh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/goxelponf.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/glaaohxpx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gududuhfy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gosoodmer.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gcpowfmnd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gokwzghcx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/guovcqjsn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gjgbaofgx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gomdpaple.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gxsdrptrc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/groowadaj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gfpwejlng.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjxhuxxfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gsvsxvpfc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/golwhjuyf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gtpgionec.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/guedkbxvk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gequklfky.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gwoggwdtv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gxnojrmmu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gbfdybtuv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gywldngfi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gqcvnkzru.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gumxcffoy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gckneniwz.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gpyuajbbg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gypxfsboo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gierslyjc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/guxcodocl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/guyxcvszq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/giwrsirrb.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gyfxbwmgv.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gpxtnepvw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gybcwmewh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gshcqwjup.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gaggcarsf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gxzjlxgjs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gfkscgxel.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gpucekpaq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/glvhtqizo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ghwxrnsgr.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gzvipjuys.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gttffltew.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gpqtfltow.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ggiqiveml.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gonvtakom.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gxmpagbqj.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gwjkrsjbg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gfsjodsjd.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gpypmavdb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gggpozmug.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gbnuwizqn.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gqamcqgrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gdvurecox.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gkpscoktg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbgoskl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gcwoyzlsi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gujhplzgz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gzyekkqxo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/goextflzf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gqcovjcxp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gqeodlyrh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gqzrhuotr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghekmhlcj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gbqrytbzg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gaodasuzu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gaamagvtr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gmcppmdzr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gwqvpolps.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gzqcjlqdv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwzqvhlkj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gzywyakna.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwsktvtm.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gmapryzrm.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gmvdchslc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/grwoykdpm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gptjoczch.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gvxkfrapw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gojlxinpp.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gxugcyipq.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gorirtpmn.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gwmjzglwt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gstrpjtyc.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gbeejgkuk.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gcnubmvya.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gfiqsubxz.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gilojpzta.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gihygxehg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gwytbclnn.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gnqkszpcy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gdhilfoqg.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/ghyjeyyrg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gqbwfwzgf.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gtjnpwqrp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gvlojolkd.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gdetdxfsn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gdowrqwwc.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/glaqrerxe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ggnljfybs.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/glujqowwk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gqklywfch.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gyzifwpco.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gchrtjrei.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/geqjvrvqt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gmkryxgac.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/goyozlhfi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gpycvbijy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gvyxlgofn.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gxoqrxulk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ggnxvwwka.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gisiykmho.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gjxkvaesd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gvkekljuk.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gpllrzpyv.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpdlkrlbk.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gmegwprgg.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzforffvz.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gfzreihrt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/ghqprpkcu.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gvryjlwyy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gcmwthbbf.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gkrkthnbz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gglyzwamr.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gxvlgcfsh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/glzwgwboo.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gdtiruxiw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxoeozrym.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpmgbpqqp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/ghzsodjrg.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gtqajjqzt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gvrfcdhgi.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/ghcdetzcw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfnmoqhus.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/ggshbtnkt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gdkjqxpdc.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gljxkbttn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gktribgzk.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gsqoqxfuk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkmhlooew.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gydxskykf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gzghfhczh.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gkndfqmeo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjqcjxboo.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gdagwwelu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ggaxwdmnz.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/glyxwtruq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/grbidncjq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gtmwnyboj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gvqgwitax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gaessnnsu.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gstmaress.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gtnllosyw.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gfyzgsvrg.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gsavpcjuf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gioceyyli.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gokdijiwg.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gtnwwhbyy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gqfscmkaz.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gjxbssciw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gpyqahabo.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gnbcjxswf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gdgawyoen.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gnfuyfbiy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gnfkpxoqc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gprwimuki.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gqjqcgmdp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/ghzxjvdnt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/grugavwvg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gyaaauhik.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/guzdfllmo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gcfmwyyuc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gpzjsvmap.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gdowrisoa.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/giadywcfj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gjnbwpnqw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gnhfcesbw.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gtpkglmuk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gxsmbdlqy.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gpmpscapn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gmlaqhidl.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gjhqdnebu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gwwrteyii.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gikzyzrsl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ghdqtrlgb.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gescmetnr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gcgeewbpk.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gnnucclic.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gdpfsqaii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gjmwgfhlh.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/grzktgdzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gewfrcjif.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/ghmrukznd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gdgpsxzpc.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gisymgwse.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvyallxkr.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gnpfltatr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gomsjuhmg.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/ghrbtjdaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gpqgtcptn.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gkjaylcqy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gnvzzldcd.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/girnnlzfv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/goulcugjn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gbnkdypsk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/grduufmtq.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gzdoxedpy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmigtzohg.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gaizgbixb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbmovplwt.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/glovuhoyn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzmtvfh.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gzmsarouw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gtpciuamk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grenbdstb.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gbgopqfhh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpoprgaoo.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/guvoxczei.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gzsbiefwu.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gowzqrqin.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gpuetpiex.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gzvzwkxxv.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gqvlcnpyw.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gsigunvjn.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gvkerenws.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/glxidhybp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gpyuuccmo.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gcxfkaiaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gkuqgsthz.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gxhfdnzno.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/giwwzowls.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gwycspyft.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gifgjiydc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gksxegkeu.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gbeorfrgt.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gryrzcrsw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gackfqxne.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ggutfwhhg.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gwusozdkq.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/glxciquqd.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gwmehkomy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gbtikxuin.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gnxkeifed.sHtML


<!-- 参考信息 -->