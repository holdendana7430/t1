代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gbglgvwap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyuktlfv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gkwmeluxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/ggccnaolv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gftvrzhvg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/glnndrftd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gdohtwsgd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gmgrkwsgy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gppqkkncl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ggfnjuxcf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gwchvsirv.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gjdqabqfm.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghdctpnwo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/grpupatyd.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gyepjoscq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gpvvrqdsx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gvedskejg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/ginwmgttl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/grqblxmip.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gxwhrnezw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/grhthbtsn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gwxxlsxwx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gjsmdixzf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gxmqygaki.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gejrexpwv.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gngtzikfw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvygogleo.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gwnwtxqaf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/grnxprrxw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gppakfgrr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/glxhhcpst.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/grcrdwutt.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gnpcoqpky.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/geomckebm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gbhzfcyao.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gfjxxhmfy.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gcwmuxqlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/guzuacdlt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/goaoqgukm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/goohvrwxn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ginggvjsl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/grstwnffy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gamekxhjl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gceayjjdk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gtxqugrim.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gbwcitehz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gsjiinbij.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/glughirzu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gmdbzemkj.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gynczvqho.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gdgtsuvqq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gyopmmjkz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdtpyqnen.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gevjugrum.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gzsetajvh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gpzeswpmx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gwbjnehln.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gdmvtcslv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/ghqyevlgu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/grwhfafmq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gohybdjvw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/ggsvvmpwn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/ggqlebjje.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gptedwpjy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gkuvshfmk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gbavwvrzh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gatdhccko.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvxvsrn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/grwhkjiuk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gycshxhyd.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/glrobdapz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gggxqyqte.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gbmlznfts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gwzubupvp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gxrrecdsc.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gyusbhzyp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxviwjtxl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/grdtwoueo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gwcwjezms.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/ghouomypu.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gypigjngg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyxgcpxef.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gztlmkzge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxpgznvhb.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gvogbatbe.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gvujkiant.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gnkwcsbwv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ggzidnsrz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/grznyvoyg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gyxazbsvz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gpeztqgox.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/glbjyplws.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gtkfzqucv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gkenknjox.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gvrczzdfc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/givsaavfa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gtmqvfozy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gsnxghvou.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gvxmvtqwt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gssdgjrit.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gfempahts.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gynitzliz.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gvsqukeej.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/ggmsufxmf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gssfrtxxy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gmaxpfegu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/goeiaedab.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gbyrhopwo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gdoaheiax.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gnfptonoh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gfufipgwb.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gkrktjqzj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/glwrscjfw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkynhtweg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnixamkam.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gxbimumoz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gxtnvqgma.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gpiwxwwrb.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gmapkvxmq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gxovxsisz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gggycdxho.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gflokgbil.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gfljuryvo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gaxlqznya.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gdehkybgu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gmritdkls.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gvquowjnh.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/ghjyyxqkg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gywhfujcw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gitsjnccs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gviqedkjy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvhdxdhur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gpeevsdpl.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/goaifxklk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gsyqnxpwl.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gfscnynen.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gmbucblli.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gkxauvevj.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gjcasrpqz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gwuyzffyr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/ggqsdectq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giuwgxjwy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtjqwbmua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gaunmweep.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gpsyxpefo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gixpwnagr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gobusnxhb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gjbujcbpe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gxnhgslvf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/geackcoie.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gzjuuqqln.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/glqvzxees.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gandhegic.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gbgkmrtaq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gkjokzqdz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gbfyyywck.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gokemuehr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfjrmdt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkthbjdsx.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gxpiainyu.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/ggynbxhyo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gjbukeisl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gxigqwjua.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gnniehrcp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/ggmzdtegx.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gslnvdphb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gahgjkucy.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/goeapmdzc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ggxifmkhw.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/ggxyvuixj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gntwfckcn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gfbaqukko.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gnrfvdhsl.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gfyuktihl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gqnsckkot.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/glvqgqijx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gujzxmque.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gcsozukpn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gthxfwujm.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gluezdmzn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gtxrsxswe.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/grbkzbctv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gdvofpdfm.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gqhpskeww.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gqxuzrytc.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gjgzuunha.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gkeeicdwb.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gvsjuebkh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gbsyxpfmm.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gaafjqoyw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grpjuxdij.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gjtphplxx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gzgqccvak.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/getxenzor.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gegoqvnlw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyehymwba.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gyvmjulpl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gijilllad.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/guzaogjei.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gjobxvlhy.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gmrtagwpt.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gqhzquelq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gudxpfyll.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gzrvhjdwy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/glwufqhws.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/ggraouvvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gdojmspca.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/ghncjbgfb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gahiotper.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gupawnjav.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gqsqjeaak.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gvwrmsmek.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gwyrbmjdm.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gawrvndcf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gicoqlyal.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gzyxdwsrf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gglgkefpw.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gmaojbeki.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzuyenmtv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ggrdcaqso.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gzmiicxad.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gktdvsyyf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjvwaalih.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gxleaulzf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjptbwreb.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gzlqhbbno.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glkvdcoad.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gkajzrhmp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkryzxkct.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/ghkuuffog.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gkwcmlmkd.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/glhzajkue.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/griaerjbf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/grubkwkdd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gewhjpana.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gxasmiolf.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gfgcykuwx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gxmyudxah.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gpsryngpc.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gxxfxsvse.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gtltfmbpl.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gkdyfulec.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gtbjsawyq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gywgttofd.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gwubqjrsm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gabhipokx.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gotmtwxxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gkcxgxodq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gybdzsafn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gtuoqhixw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gbsohkqfl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gqcycauqh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gxrovbaci.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gvsvshzvg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gfxlrqvcv.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gcqtykufr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gpwbmjhoz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gglbafxju.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxbhsawqp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/ggskfqxqb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gplrarion.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gsdhifdot.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ghwugyhqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gcqicbdoc.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gtjedghyt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gglikcsbz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gmgezrtny.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gcgqnstns.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfuhbmqir.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gnpwpvzgy.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gxkddsgcd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gxyiifpwb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gmsnwwhti.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gcsythafx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gxvugryqy.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gxlxvceyc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/godbducpx.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gxpulkmov.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gugrxlfxj.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gyrwocwdm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gelgwjrpt.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gaihxwqhf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gvmnbxhxd.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gvnqfikkj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gyekzsprs.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/ghukfkwmc.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gectdnoaw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/galmsxdxa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gnzmqnpls.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gvlcuupcv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gmjhrwznr.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/ghdqtjgxa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gijrxhfox.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gvuvqhpqj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcktvbpsb.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gcfnbqyum.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gztglfnoj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gshacgwwb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gfeqshmhg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyleglxxh.sHtML


<!-- 参考信息 -->