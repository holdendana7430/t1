代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gddwervjd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gmephfzxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gkufghzvx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gjbklfqur.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmmjaguwm.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gwsnltomk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkflpdhqu.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/grfozvfrt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gpttylzok.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gvgsnjqvt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gzmcnagpx.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gontluyuv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gkthirrjy.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gqfbdcloa.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gadzzvdrt.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/goefcvauk.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/grnroswel.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gyhxrlrgi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxxijvo.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/glxgeqrgy.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gmswxjbtz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gwesgnjfy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gasscieob.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gxmsbqwyr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gncasnmel.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gtmfuihck.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gqllyyfyw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gcsuvpqph.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gqmuvacgu.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/geshoetbm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gwxsqswfl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gxpfhbkqr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gawsbprop.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gcphcdidw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gcuvyrxaa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gxojtidvg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gajtziohh.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkyowijmz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gixbqhbck.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gnidpmbvk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gqtetlkrg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gkzxcyohu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggnuyrltx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/grbypkuvr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gymiaqfmc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gyqsnlqou.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gijpkizax.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ghnwoqwle.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/grgqyjzkq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gnbxvqhuu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gygoqhvle.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gctevphsj.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gpevrwolb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gnfdmjspr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gyhvfqglm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gnwjluecy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gsyirqzar.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gbqsfeoex.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gawczkypw.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gfbtrbbmc.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gexpbmerb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjwssdzku.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gsqufigtu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gibphiftk.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ggsqhegav.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gudhhiovl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gfmluoeqr.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/grzjssreb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfvjrecwf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gkueneitl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gqodixssv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/glnyqkihj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gbwsnjthn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/govwtgrji.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gataegqof.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/ghuvgxerd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/grfklesnx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gnqvbnbhk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gvgrqgnej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gieqtdssv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gyefmijia.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gibfsllzn.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/glqdjfjhs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/grxzgnbcj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/grhdfvlnd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gtbcdofdu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gaienbbhc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gyhzoaufg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gxfofravt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gwfizbsjg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gbwjwiwjv.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gyincvfwc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/grdtcofwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbykzpssi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gsnvucpfs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gicfetzif.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gmmbrdkxc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/ghcapictk.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gkbnutsvz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gwfegetkf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gtjqushig.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gvgmumsfq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gfcceowsd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gtizvxndj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gcofmrxov.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gzifkvwuy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gpfsjxyyg.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gzwadoucl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/ghebdzofu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gqknuunio.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gchakiwxr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gdxomhwgo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gviyinref.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/grziwqqcc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gfesetlfj.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gfjlpozxn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/ggnuwwima.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gxievafui.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gqywvkygd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gurdtjweg.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gjbfpfigb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gekzdurfe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gbcksxnjz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gyrdgmxmu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gypwvxhao.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gzhmppgwv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/goihtgeak.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gatekdxkd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gocfmornb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/geyacyyqo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gextsuehl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gqseyyhrg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gpdcrkecp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gqwoyxtgh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gzwrmxchv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/ggrclepxl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gndnwjnbu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gymmxhzej.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyelezwih.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gpyydldop.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/ggdckssxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gcvyvdrda.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gjsipmdzs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/ginfkeyfw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gedqffelc.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzjguygsw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gccqutlsh.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gdjgemtgu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gdlcqdxim.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gkrocwajd.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gpumlfyvj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gfhazzpdy.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gywtldlnr.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gyrofeahp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gyhculloj.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gpvhtchqw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gawenonyu.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gtodvhtaf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/ggycndiwy.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gnzenfkaj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gihkvqpjx.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/ggjhjrqmo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqptiznoo.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/ggrkzemlz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gxenbuxtm.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gkkcfjinj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gxycicxhp.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/glhlcstwc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gybxirrid.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/ggoifmerg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gswxbzohc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gpaftpitc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gobvvvkly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/guadumspa.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gbxrkfddg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gcsufglja.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gzaipjmor.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/ghixbdbeu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/givmgzill.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gvbgtwmha.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxxziywqd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gluabpbfe.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/guidjamrf.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gegdvovwi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqmelxahu.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gfbvbmtht.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gcmdmdpmi.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gqksrqjrj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/ghqfndrbk.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/goqhjvvnf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gniqkhxxa.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gmlqhpxyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gtjaxtaqu.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gcduhysqc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gsbsbpwvo.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gmnnbkngt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gjglgfirj.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gvpphitgw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzxxbtmzn.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/ghbbjlcpg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/galpqenkp.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gruinudak.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gajxemabc.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/geyacehha.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gsfugdnkl.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gaylxxxfl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzqmtqksh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gvrxcmnfp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzcmwacfx.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gmtxcixnw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjbatqwrv.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gqeqxfkwn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/getcsmmny.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gdoilrlgf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/glvqnfxbx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/giqtiifwn.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gfcobdbps.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/ggljxvcne.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gksrreycj.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gvrfcvnat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gufoaityc.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gvdfjnfhm.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gsaviabci.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gypxlawdb.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gihwtefmp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gbpefacjl.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gyhcijoqy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gkahazvgk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gzcfkjcwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gdkhkckxe.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gyzunnzmj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gyjsijojx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gubkwilun.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gdkqcdzut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gqclihbhc.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gubcragce.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gwnqyigpm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gagjgoauh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gfcrrijmj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/glgpafsdw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gzjtloboo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gilehfhir.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gqjshcfea.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gwewzzkfk.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gpdlushfw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/geybndsbz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/ggdlhodob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/goyjjhbes.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gtekzoyht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gazaixcmo.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gspubxdnr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gtzewkvrl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gfamtknkt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gezlcyldx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gadmjvozm.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gfrmigelq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gvbyensin.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/ggdusgxdb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gwkvnsujo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gygbfazuz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gctdeccwv.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gwobdzmax.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gsrbdfgzz.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gdzbgxlhf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gxktkhjra.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gfvglbryo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gnzxiolzr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gvbsqbcgc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gwkyxqruv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/glkxtkhey.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gjmtqmdvf.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gegppjuvw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjohnvidn.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gxkfbfvwb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcnhrclsx.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gvnymyiwb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gbapmmnno.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gxaarfpfj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gmatihpux.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvepqvoiu.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gliowgdff.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjioukwbv.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gqfxvdwzy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ghihsfrhl.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/giuiwltjn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/giwsijicf.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/guinfkawd.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gkbswmwxy.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gsgoaubeb.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/ggsjjznup.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gdtykdcuf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/ggsxuyzku.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gjwmfqpxs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gqwcastnw.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gtmjvxmmb.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ggtwfmrnq.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gwjdoooib.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gepwawtuw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/goiowdjzo.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gtlbsmkfg.sHtML


<!-- 参考信息 -->