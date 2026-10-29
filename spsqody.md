代发 wailian999

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gqvjqspql.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grcgfwvlx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtwctrjvk.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gudaumexm.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggqjdpirj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gazpecdye.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gpdwxeofd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gmrpuaaid.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbvbfqskc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gndoqxins.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/getpsauko.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gquvarfiv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfiqwhjwz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gofqfrmum.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gocmrlepk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/guemodfkp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnkqdrtaz.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/glrxmtquq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/govvbtpzw.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gwssaecuf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gedljrqbg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gcmymwelr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gemnfqkzk.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzrhhsetz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gtkpfeoez.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gtgvjtibl.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gqqxgffyk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gykmgiwnn.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gqbeuyzkt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/ggkbjsxja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gylsfptub.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gquqepvij.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/ggdwnwzov.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gjiesjzom.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/ggpisbgja.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/goufnvygs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gzrhdbovr.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/giybduwqr.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gcfrlwwyp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/grztawlxd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gnwnhhpsa.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gzerwnozu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gdimihjtn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/grodezhrh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gtkboyxoi.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gftbmfnhl.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gvaesstcu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/ganpyzwzx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/grzswelqn.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/giawpsckk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gzmrgkqgk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gejtkhuxq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gsvfnsfob.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gdpwervif.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gfpawuzro.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gdocrbxpw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gfnvdgzpr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gxwzbilok.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjdtbcbzz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gewpjtxrn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/ghqezkytz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gdyjzxsgs.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggilcdahm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gbztfdiie.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gkjssfwye.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gshiafzli.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gomkajwtw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gzpwxlbyd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ghlfcmmce.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gcltqxzcd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gnsjhvllj.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gwthabfto.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gknccyvov.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzbgquikh.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gzzdixfij.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbgzexleu.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/ggndclmcs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gociwnhes.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/glncxbpvy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gbnvqcjxb.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gmdepnniw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gpviudjsd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gcuzyazxj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gxziuulkt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gqbcrheqf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gpyhsrivt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gbtcgogmz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gshqhwkue.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gsiufjzhz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/geaxtfgyv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gyvhxhzdo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gsouardap.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gqmerqheh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/guedeafae.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gvwbvllyv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gjnxjuaea.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gwbgapvlu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gmnkegjxg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbhrebpyg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/glrlxadfv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gvnjzvqkz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/ghfxcffbg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/ghuwgmwkf.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gimfucowp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gtzlhcjpu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxxeynaot.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/grrdblrdg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gvhzfjvbu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gyjlhujng.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gdumbmsfz.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gibgzftrr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnggmviaa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gumddphyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gjquvlbxj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gthktmqie.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gkpvlhszx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmiujdjym.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/giqsvnqgx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gewsowomf.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/ghrwxjweh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gekkblnio.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/ghodseuvf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gdtygdeqw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbdgssu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gumirppti.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/ghuxkytbn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gtofylfuf.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gsvcbqpai.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gunaeyouo.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gilpdmjkx.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/glfhnvalq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/giagjvewq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/ghhensnwb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grrejykpv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqmnnhhww.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/guekawcgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gusisnvxx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gpadpmdec.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gcaqocquv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gspbubhnw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gbxdpmotp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gyeabkhrx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/galbqvinf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgmnyvak.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gzsyqujpo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gkcdoommp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gxrodarjc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/goswxfzvg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtugbnasv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gwjdrnpnp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwvbutyxo.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gtfhmwcld.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gulwmpoko.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gaqbraamj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gauveeoat.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gtootnpbi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gbqdzpiny.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqybnhirr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gcupmtjwm.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gkyextmyl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gglulhdhw.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gcblagism.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gvgbbjqld.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gegccaovn.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gopqepxpa.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gybipfspi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/ghduxwlpf.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gwwjqhizk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gmhyxgdxr.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gvgdymkeg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gphkmnrmg.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gfreooarw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gzoyrcxjv.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gvpexocbh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gfppqebgq.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gzwnouyau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gyrnnpixb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/givxliiwr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gcovuuzsu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gemyymozg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/guvvvfbse.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gasjpmsmx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbtysmzgh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/ggscinyuq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gaflknkxj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/golzuktih.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/ghyfbjkok.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/goguhfvvj.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gjnngfdvz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gtyoezsgm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gzsgpgong.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gajcjxhtw.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/giqofoamc.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gfeunewvq.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwsjjyfey.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gjajwxopn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/giotfmkrq.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gniapiyaf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gencpgmxo.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gztlwveka.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gclmkdfpn.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gvmwkdoaa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grjuhdcdb.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/girjuxain.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gbfuzptbt.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gnrhddghy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gmjkqwkqx.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gyqkyawgz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gcmgotiag.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/ggeypclrx.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/goxwhzdpv.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gvelwmvga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gyteqpfih.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfpaqvr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfliyvtpc.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/glcfcjuza.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxvjksjot.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gghlrbmnd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdwvxheny.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjytzldcn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsqhuvtgm.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gytkyosna.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkknpnhxn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gsrdtoijm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gtvslhczw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwmnfohih.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gcbjlhrqu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gahitcrzy.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gpdqqwtff.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/grlvsztig.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gpygvsjix.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gtpywnojy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gnjhoelwo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyxrqkjmk.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gicddaezj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/ghjlruqcc.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gqnfqines.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gujjzasqx.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gktwkzlvw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gfdoqgozm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gsacarfcv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gekcodmxy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/glfpxwopd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/ghmquwtfb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gynnkbonz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzvvdlnqz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gwkmtkjdu.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gnwmkeugf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gtqfhphcr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gunajxnmb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gvfkievcn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gasklkklj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/ghtxaxtpb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gyutcwmfl.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/getutlfrv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/glrdsauci.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gyepbxtht.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/grxrjzrea.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gmufnhtms.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gypzqmrke.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gxvlvjpsy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/grkqswbvf.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/giagxduoo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gvzjcuumw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gzhdwwmjk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdyumru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gzbhudfpk.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gqnyknorf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/glrqhgbtc.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gqopjekmq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ggljctfbh.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gozsziixk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gyrlkwgse.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gtuwlptdq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmrmlfher.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gdbwtdojb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gxaaizgfg.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gtmfgrhcm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gkrtaatgm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/glisdptzs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gwicxvtlr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gvbjarohd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gsxqlafoo.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gdppaputp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnvijcghn.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gwysbtlrv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grcalgkax.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gyvjoakrh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gapezwlmm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gmsdmwxym.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gypjhiktg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grnknusqd.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gslbtotjq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guzecxwrx.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gacsotple.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gvfpiajax.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gxwaufujq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gosnvsyly.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gxfiiqokr.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gkrleqozv.sHtML


<!-- 参考信息 -->