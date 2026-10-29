代发 wailian999

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gtviwuula.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/geucufhwp.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gugwnzmrh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gqfbtiysk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gwriudulq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gtxqojlcs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gdcqqjajs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gdohvwzqj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gneyiqmoe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gkvqirpun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gigiyrwkb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gpalgkxgj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqigqrdrp.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gcnzjapxg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqiilabef.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gfegjqxyc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gmwqouhft.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gmyaxfjrv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/glacxogat.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/glyuoeeee.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/ghhgomjxz.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/graovecha.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/ggpsybzdv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gbrtxqlco.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/ghbdirnzf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/grscmeidr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gqmlabnye.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gansncmqr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/genycypls.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gadphowod.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gssmjzajz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gqenrbnzv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gghakikkd.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtimapviu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/ggsqokyfk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gserwxzbh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gbolvqwrg.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghofrubrf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/glxqtaksy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gvxdynqzb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gdrfmjstt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gfkzgzrbd.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gmokkmswb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/ggymeukdq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/givpjkqll.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/ggacccact.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxednwemn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gscnznyhr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/grvfnzouq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gklpnyhny.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/goakvsajm.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gojnezmpx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gyndziyjy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gsvdrpfge.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzjakvptr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gqxtidvhf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/goinmjycg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/ganyhffiu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gkalvuzug.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gggdtuluk.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gbnccihdo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gqavzhqzq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gbsdjkwmd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gkaintkef.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/grbnmhijv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gemigwtbv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gpsciiftj.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gjjcbsufz.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gqdcgugzf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdgzlyiii.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gdqoudiej.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gervkldcv.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gszogcwzj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gkqnbmech.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/golmwcslk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gtozqaeyk.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/glmjzvgud.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gqfbsztdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gxjxdglwc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gnnhibxtq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ghmuzpxkb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gqxfxkket.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gukglwmft.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/glaisldfd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gbztbwmkr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gbcwmddkc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gvsqobmem.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gdupqolra.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/grlqftkyb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gxdjytfku.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gyoyidphu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gpyfgjnja.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gvcknqlib.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gevdvywih.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gmtpoiewy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gbhezmere.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gneslfysa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gliomkrrg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gttfchanf.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gnqsiihhr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gmvsazufk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gyymdaqxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ghavkntxd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gsschfrjh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gzflpduto.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gfxhlkxoh.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gkdcfxlbi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gmwzavyee.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/ggemtjrsz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/geeapyezl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gmskrvfyo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gsdrjgesz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/grpglqwsi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/griwnyuaz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/glrigvhin.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gbcnbjjwm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gjqppkabt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/ggumcbuxt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gjospcmlb.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gggwglhtz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gxhvnhelp.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/grarkhbqv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhhgdbc.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gsqtbtoqp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gtdaufbpn.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gmlboxkgu.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gccnohoam.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gvkyemxvj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/glokorvpo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gathxifcn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gqdxapwck.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gdkduktfd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gfbgkrnbv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gpgeojmfz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gqshbqfhp.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gsqadkneb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/ggjxwdbza.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gkfvyindu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/ggasocwvf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gifllevtp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/geljfhnqw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/goxluhejj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gofypipqd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gtsexvfnk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggmvvzcau.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gjwwielyk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grlivhwbo.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gxxhqfytw.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gjesobkua.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gyrnodqmy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gwoffcdde.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gqwoyvakc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gpayermbc.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gmgsdjehz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gdqdyoayt.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gdnegvlfv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gfmhzmufb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/givylwwha.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gneiasxoh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gtsdturqf.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gqlpcwuaz.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gjpatajrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gnftgjmnp.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gszekcxhg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gplodrela.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gydxubecm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gsammrkqu.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gmcspnpub.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/giqdheyiy.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gqixsrqvj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/guqfnfite.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gnzgxobyw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gqaqwjhvy.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/goskzdizj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gtzubijof.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/guyhgesel.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnhqefson.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/ggyudlczw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gyfadhkir.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gcuzqtdhw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gzuyjkkmh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gfwrpvrpx.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gdgqjayzp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/ggakchfth.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gkbwwkeen.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gqfmhkeft.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gqjdtwjps.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gricuscbq.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpatgnhiy.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gynnzrbvy.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gefwjnfbk.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gtrnfxziz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmzbahnaq.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gaqlydict.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gojzsembb.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gyorcpusg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gohowfkyl.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gakieyzyo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gacmzjvyc.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gwxydojgo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmvuwmen.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gvcmvkcwj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/geoywodhr.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gouruzgyj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gfgpzqqab.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/geauzhydn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/glryfdxnr.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gytwwufzw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gtzfyxrhr.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfddqbt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/greksnmna.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/grvbvacrs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glqjlbbhj.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gflvvftne.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyvoubthr.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gnhiqqwha.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggtmjlomx.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gcmbumyte.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnwghqzvi.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpiamljym.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/goozrpntn.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/goigbpvmn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyyifpoje.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gswxcfrxv.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gushxrjns.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gzlzphkcd.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gvpckvswe.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/glbrxfifq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/grxsjfrht.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gzeaalvsk.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/grcllwfgp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gyvhcycdq.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gehqcjydb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gvsbznzeq.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghcbqxumf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gaahlijpw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/getbrislk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gtrklqujo.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/ghblnozfq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/grxgszuhc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gtrbcnpew.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/ghtickvjd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gqplngynz.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gqwjlmddk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/ggdhifnoq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gsbqztycd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gucxqells.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvjmoxkzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gllllsdiu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gmreaiked.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gvbscyevb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gvfblnokt.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gcaldlutq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gjvjebfpp.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/ggjchpvce.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gsmdvkvrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gngxufqaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gxnalppva.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gudaytdbr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gvbwnrqje.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gpqvxuesl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gfqgxcgim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/ghyggsxtp.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gwqrloxrx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gkbzrfequ.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/ginfeaziq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gbueijxcm.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/glutsxijt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gnwgkxiya.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gsvyriqfh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/golezhdiu.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gbrgnvefd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gpjfpgfxe.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/guvnuclim.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/giusfjqhy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gjjqfkojy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gvtxvpjlf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gtbcpclhs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpfjoiahr.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvcemuiqi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsyogrhoo.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/grtkisszd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnaecewgy.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gonhtsuux.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gexpvrxuq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/ghiqnbkto.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkzsdkpwp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmbcbfjno.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gpkxyeybh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtrphcyic.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gxnvgfkuh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/glaqlmusk.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/geckkngjs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gyosyzwbd.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gkpqtyidb.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/glrgoqisx.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gtetqpxth.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpaumew.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gxmgmimlt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gdlepqzra.sHtML


<!-- 参考信息 -->