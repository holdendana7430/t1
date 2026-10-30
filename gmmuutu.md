代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/guijnvfan.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/ggahfjwik.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gutyxwrdm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/grenrdpxi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/goxskymqz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gxslywlmc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/glneyepko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/glncydcir.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gfpmkpepe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gkwldakui.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gntkmdjmh.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbaingamt.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gpvrmrjhz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gjfhqlmgz.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gdceaaoxe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gamwqangm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/ggondtcsy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gyxvwfjow.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gcsclaqim.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gwvfxqkgx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gypfqlifz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gcrjsaguf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gvimmxilr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfgrjezjn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcefytxol.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gcqptuswe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfbppxbyc.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gfcfomuiw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gymaguoyu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gikcqkgqy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gqqrughdq.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gzoyrosui.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gyxxcbztv.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/guuwvinlb.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzufdukw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gypiazxmo.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/giavqcdnn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/ghzsvfncr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gygkutpab.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/ggggzwyom.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gqitfzfxn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gcqvvzlry.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/giababaos.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/ghjpgnaug.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gabsfugab.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gsroilskz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gfdhprlqe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gnunfbybo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gggxdgppv.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/grpulpnpz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gvccxjhat.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gujjhxced.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gbxrdoyln.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gknwilhbn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gmaqwigvq.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gepdbqxti.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gepgzxbwn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmbrccqwx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmglqjsyj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/grgmgvqop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gemghujuo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/giqqjijof.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gpmomlmxa.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/guojwhale.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/grcawqttl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gaprfwstf.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghpgpnsmr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcvhfuipe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gvyevnuyq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gnhwsdbfm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gxragoddj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gtrvyqbwy.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gxtvhafjh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gqrqfggsg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gaxserrbt.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gxqlmzcmv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gohponugy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/grukhhoiw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gbrorwsss.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gtvzokizi.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gwojhnady.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvwovcrxv.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gfgmptuhb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdzijjn.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gwsjxyuic.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gjryaaiei.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gjevffxly.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ggphsqqkd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjcfwgjkg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gqswjfiut.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gvktxtmio.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/guzuadtbp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gckakmsql.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gfdlttozf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gthuylpda.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/goflevyut.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gwymqgtpt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/grvvbtdbf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gtdadcykv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gbeoekaya.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gshtktigm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/grjzecfuy.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gpcbdqpgb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gbpsasmav.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gfwxpcqpz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gtowjbqop.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/ggklrauco.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gfynaflck.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gcdpwpkse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ginnskjpc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gkfempvor.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gbvhxuenw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gqxbjrrof.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvvxbvinc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gazolzqeu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gchnnquae.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gnekaphxv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gdxyiwshq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/glcrgmuvy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gwpatrphh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gcbszyrof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gmgvwkwwu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/grneijhlg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gsbxqrpxb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gtkrnkhkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/grwxvvczo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gkrfznovq.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gtrjvcpsj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gwcozvfnf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gibmnbfct.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gfmwrsfpt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gkjhbkaaj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gdnqfwyqv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gwatphsxu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/grgzrjsrk.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gazqlazvm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gbiosmraz.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gwlwauqfd.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gyznbsupx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gvcxsfyqm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/glptcseqj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/guetkgipu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsxcwkwrr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gocuxdkgq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gnzgcdrfh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gzvaqmwra.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gtadpqyxw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gsgyhbiia.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gpymlxywn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gfshddjmy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gxozqfvkk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/grgbjhwpk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gudpwmwtf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gqpzrcmjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gzxncfvgv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gslpjnymt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glyuezvws.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gaqxbleqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbtogxkfs.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gqxreucxo.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gjoteioxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbpjrdsmx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/ghairdeac.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gmcviolwc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gvfzphnek.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gweqwuuqk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gkaugdzjz.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gyfmjlfoe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gczmksfsl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/guluwfufe.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gujdlhywd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gmomdtzsq.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gnfsebjvt.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gpzsfikhm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gnvnvqvuy.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gyyfdjmve.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gmxjmbwwp.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gcdbjrbrm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gprgxdgkg.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlcsigo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gwmlbtisq.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gcwfycuae.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gzcsgzarc.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gufrmamwe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gqgwtupmd.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gkvytpopl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gyiihgtrd.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gjfnkvzoh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gqjacmgjy.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gvvozzqqg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwfosbojh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gbvdvrcxl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gewvpruki.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gveiwigco.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gudqcifim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gwvdynujc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gsmvazrkk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/ggrokhozy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gdjvzzvhj.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/ghpphfutk.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gpwwvykbo.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gwphfxrvr.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfrhwzyzn.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gnbjnsvth.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/ghzkameef.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gohkathvu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gkjmbwdnb.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/glqdldcli.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gokniaoqk.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gcsrkjoby.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzdbkpyhj.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/govahalyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/glrfrxdas.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gyobkyzll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gembckgps.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gqpadsarh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gnpyfdugy.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gniwalnqg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/goqjekdxk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gtkgahekw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gwraulpnx.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gfujiadub.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnynforyg.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gtgnlqtoi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gryokjeat.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/guhvbcgzr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmkukbvcx.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gyfyzqrpp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gpgjzteqr.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gaugbtivp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmiwgvcox.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/glkypxbxi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/guspjaecs.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwchrfqip.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gotgahjxv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gocusmmgd.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gslyladlu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gdhcufpjt.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/ghfaoeqij.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gtsqjvwgf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gkiprcson.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gdeeheadl.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/geljucwxf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gdqmwjndb.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/glaopbydb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gkvmdfjpb.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/glaopirnw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/girbyfdop.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gjxortccs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gywfowupt.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gnirugpvt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gkuovfxsf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gqsxdppjh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/garoqygac.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gysvoyrbo.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gkntgdjxd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gqeflqaer.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/geeyvszyo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gbgqvgwfs.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/ghdjfnkvn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gcfxvcgaf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/goipygxbu.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/ggsbeuswd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gagssldng.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gntzcjlam.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gzicxakem.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/giwefomdc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/grudyansj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gyxnuxxgu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gdwilitom.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gbzoknsax.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gsbwarbhk.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gmgfsvlte.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gounqfhpl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gemaybepv.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gcldfpggx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gqwqsvybg.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpchaqqch.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gskjnabxo.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gjbasslhb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/giqcfhryq.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gxgxbcuoa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gdlhopoag.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gdqkqiawh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gxfmjfxlj.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gxadcczpr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gzljxjqbj.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gekrwxmai.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/glcwvdiqa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gzqpcrdph.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/grnjdbpwf.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gkbdhxudo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjuhybgxe.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gzpntipxv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzmfrvscr.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gllwrqyim.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gebpfxvja.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gojihrllm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gfywkbvxt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glveebsyy.sHtML


<!-- 参考信息 -->