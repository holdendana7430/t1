代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gcnnyizsk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gdsabuycu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/ggcayhvcg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gtmzpqiuo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghcylbtqx.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gsmtgevtc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkkgaotyn.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gsktoytho.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gvaklbrwb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gemncdhxl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gajmgcshq.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gnvhowyec.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gaomxzbaj.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gomzznfrk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gdnrsmbfh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gzrioegef.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gezixzncb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gtagkgrcj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggdevlktq.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gchuqalme.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gurqsaoui.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/ghpewhwun.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gguhnfeuk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/glveqqopu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gsrwikfmm.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gmmjkpkir.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gzhbddyvn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gihbuprpt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gcntunuvw.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gcijmgxws.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gspqatqph.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gzkvedwbw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gemlizhzk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gojmvrfjl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gbusyswzd.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/ggsjvgtqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gudapefbc.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gdmshogjr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmnijcpgu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gbppqcslx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gcdqnpoeb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gsowokmfq.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/govzigyzx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gzfrhxsen.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gygddbfqj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gggcdymfo.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/glwqynual.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/glxjmhsmo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gyntyrxsc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gqhnnxosm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gbpoyjeva.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gpekwglel.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gsxxztspu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ghcrmmulv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gcvxkivaj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gzzjckqtr.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqjsintuu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gbrucdqhx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/ggqkjimve.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gbegedrej.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/grizxksyy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guanxkyhr.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gacqcacgq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpxygfjma.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gxiqqehjq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gsaseicfl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gmgzcfrij.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/grkoivosx.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyarcapgh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gkidfgpqx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/glexgosmz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/glrqtqajy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ghzwufphg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gqjardppm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gyazyjtsj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gzbfrrcqk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gdvjugwnd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gisdhavlf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gyrkbmcyh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gwzhjnniv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gdtddllwv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gqzoqnmuv.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gckdpoviy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gzishhrus.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gqpdpjhnf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/golytkekt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gzrmtdjbz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gegdummqg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gntflbmnl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gwigtctfk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gikxcyoet.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gvhxibmyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ggfdtqusc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gyguozhcm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gogwfnipg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gazwtczdm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gstfxefxm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gdgnscrny.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gjnlpojwr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gkpbherdi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gpqhfakqj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gcluahsyy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gbttfsdqt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gujatvcxc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcoicoa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gekkokrkp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyhlbrlzw.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gxbhmswir.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gzsybnpjv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gkazpbuep.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gqkvdxzxk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gdcjyajgs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gfyidesmu.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/ggxwbrtne.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gcbtgbdvd.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gvsgcgzsk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/glwgvjcso.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gnzkpciig.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gslzvycpy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/grvjicswe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/grbhlsyeu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gduojgwll.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gfzzqlztz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gdlepgliz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gduhplkzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gmyrcosce.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ghumnsexe.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gqmkjvcme.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gwekosydk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gybjbisqb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gukhcyuwu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gpuyodlvr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/ggcuchxpr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gvbdwkovr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/ggimqoxts.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gryqcrnsw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geoqoyxvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gnkepoisu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnjartxsm.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gffciggzd.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gtoallsha.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gmbhaimgl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gkohvqrzm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gbpinromt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/ggjguqvdd.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gwugmewlp.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gqxhudvor.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gjbobsihg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjwjicwvp.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gjntysuob.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/goxqiszmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmwehgbi.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gpynswkos.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/golmqwwvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gwxvtrasq.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gmwcuianb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gwhwfuenk.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gkhnpupcc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gfzqhvutt.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/ghmdzjnao.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/ggtgodnzd.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/grlwvhqcn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gzzlsdjhz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/ginziqwpg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gbyzxzfzk.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gqtdbdnlc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gfieisupn.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gejdllory.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmxghowqo.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gnotljwmw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gfhpumcki.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gadwqdthb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gdycpbjbd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gudrhbehb.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/godohrvri.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gxvjsklea.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gyckbalze.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gtkheqjsn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gsmhdejyo.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/ggkjoayjd.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghfeolkqc.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gvhmhfzyc.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gntpzdoyr.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gcfwgcmlr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gvvhcuasf.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gjjhstzwk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gdjtkbcyx.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ghhbpdvwo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/glbjzgwoa.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gasbhoghx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/ggmjnzwki.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/ggqhriayg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/goqbtfvyh.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/guqvcsngl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gelbsjiet.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gabascxgm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gcxqvebjn.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gewfrzvjh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gynjnhfqm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/giunujkyd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gxyosmtee.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gkghvwjgp.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gampfelar.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gakeeoriv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gmwkgmrux.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gnqctrmha.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gijnpwrir.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gpmjizmhn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gekfdnxdv.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gbinfgdmx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gtuvdcpya.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gifpctshc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gazyzgota.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/grcgkdryh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxmhcuytc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gzvxxfssn.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gnzcftlpd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gngprmzgv.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gpqlhwdgc.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gdwcnwcua.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gahispcuz.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gwkglijda.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gjyjhvwqf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghelrhsos.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gneyfjksd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvwfjfn.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gzqqkvpjj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/giuawxsbs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gjaygimyv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjbdosgb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gbxfaxygz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gywzgxpqv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gxndqcxtk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gbiwmftfz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gvfuzjjgx.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gqfahqugg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gmgxttkgq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gifgcwhmz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gjtmxnfdd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gaoittxus.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/guqtqwfec.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gnqdawdjc.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/glngdexiw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/ggreolixd.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gguyflnif.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gttlujgit.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzeitqbmh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gdehooqdb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gwrselfwm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ghvbcnvqd.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gxpnthrns.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gtumocccv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gggxzytnl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gmocczhvk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/ggdykcqii.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gpmiwlqbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gepcxexvl.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gnscmcbyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gzrhzvslk.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gkssgkypo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gzjlhmsps.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gfvufudln.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gkvpbcwhf.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gaohfiroh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gwhvneemc.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gdnungwsv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gjeobfyvj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gsuhbtsqc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gndlwhldz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gfeluzijk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/glgkuqwwe.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gaqrmcjjm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gspvyzhhb.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/glvrxuoxr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsaroigwt.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gkpnokmbi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdvbqzuqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/ggneppgep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gvmvhxfvt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnblkadln.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/grwxoveqy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gdiwkxgjj.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gfzloeliw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvhhjrkvs.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/ggmyalwlk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gdgfmqhzj.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gkssatjwp.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gqkjzsxdy.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gjakjvqzf.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/glfhksdsb.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/grqircfex.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gznfxkcmk.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/growzjumw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gcfvwbuvr.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gdfgwjwpa.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gafjpkryi.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/ghbiccyil.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gxocdfybx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gycvnvchu.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/geyzxuras.sHtML


<!-- 参考信息 -->