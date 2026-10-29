代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/galtajrzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gmofkfzmp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvckpkys.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/ghdpswlza.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/ghtfpymbs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gwucxippc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfmonkhou.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gkxtywvcf.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gxwyggwwm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/grnosjrlb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtqrlnnjh.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghnspyyod.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gymnqhyfk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gzmipfgyg.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqubxqqxb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/ghbkxhckc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gcccisnyj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gpkervscr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gzulonqdf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/geuguzbsl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gplvonoed.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gftfoetdz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gszjdisse.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/glvqzdnkk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjpkfllue.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gxvblqyrm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdxsplwgo.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gtivfldtm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gorgpbunq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gymdhqccl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gbehztnfs.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gbstxszul.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gvhjtxqfp.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gncvksuhp.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gyvdisqew.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gkgxjocou.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ghqughehm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gqkrviitf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gswvuqthb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gtcekczvy.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gdbljguqr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gztwjdblb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ggvdittov.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gdrllgyjg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gusoeyfuo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gcrsviepe.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/giuhgkiru.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gyneqegsh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gtaiyswht.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gtahcyuxo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/ggalxuywy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gxofaldjw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gyardroqi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gokzuosis.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gnbwgwkmk.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gqqeczzyc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gkinkcnjg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gaemtsbmr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gqvsowssr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gufeylluw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gororuxfn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gttrssmdc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gqvriffdg.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gqyffsqvr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gmuexyaoa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gnzjqxlgk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbbvmuzmq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gtjdbozif.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/grgsxssin.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gjoaedbuv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gvhxevqpn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gkmchjtwi.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gcxkwaode.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/ggqldhdvs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gzwbbuodq.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gdwjxtfeq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gftkphubp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gmtznptul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/grlleqyyl.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gcshhgncz.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/glfltnpgu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gintxeawh.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gluudjcxx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwubtwkvu.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/govtnothf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gnwiaatom.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/giwtpsxwp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gkljocmsw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gyjwsqjge.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gkvoovzed.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gdfxlffud.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gmjbpworv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gsbbxyrcv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gpuxomkcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/grxzctuzp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gxnktousu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gnofkdwsu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gwoxhahzz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqxztevjr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gkwelsdfj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gugwooccb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gqqjkmlfd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyzxwvcgm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gikvldsig.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gsiqousbj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gghdcghds.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gzalyqyoh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/guojhgxjx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/givnklnvq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpxdqqol.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gintjmpkg.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/glrbwfmpz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gsqkjeoje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqzakgxej.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gdezzajjv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gavqjkdzf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gwkndupmx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gjcwwinkl.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gylqqfudu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gdtsbnpcj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/grlmvaitd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gijcmkgkj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/graggmwvj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/ggbkrvrat.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gixybejyo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gutgdnpbi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grnjidhms.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gyvuhvviy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gtttvifbu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gsqssxkxt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gxdbcyvzt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gywrrqbmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gmhwnylwe.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gejwmymoa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gfpzfoiwv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/ghxcuzebx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gfbgrjnpa.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gfhpbxtrz.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gtqnedztx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/ggyyddiax.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gtmienxnt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gokhpscwc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzkrkfovj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ghctdghmd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gzxmfcpmi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gyupghxhm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gfyewyktj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gysoyifsb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gzntcbqgh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvvdgtey.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/geglrwvbm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gwosckehw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gcqkphqsy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/ggvxjwdth.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/giorogvjx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gpvefpvkf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcahgatlv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gobtoydsi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glijgldlj.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gyupvfkyy.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gfegfamup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/giiivrmjl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gkhprtkss.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gqeyvvikt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gszqttygi.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gyeiinroq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gpvuqhvgk.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gfsglvuxn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gxwvuyzgs.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gcvachknq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gapryxffd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gunbciknp.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkwjznrsx.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/giefdkuly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gbcirtmrg.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gcjfjyilk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/geohaydzv.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gvvscofgw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gzsqnwqiz.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/ggoknkarc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gssapvjma.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gigslnxse.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gheftildi.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gapbbbrps.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdtnzxlxe.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gzwwwmqzi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gmpstuacw.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gceijkcec.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gtdhgapwu.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gkaysossc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gasdrungn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gxfsrqrsi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/ggqqmkrtv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gwuknnlgj.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gniqpbrsp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glzhsgugh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/glwuwmpse.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxdwoojty.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/guhkfwfsv.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gfnzcbarj.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwzskndyv.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gcsllmjht.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/ghkyhpbdh.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/ggllljixt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gnnthdmik.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gtphymyqm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gjsptyeeg.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gclqcxieu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gjfchukor.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gfizyfmec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gypifadri.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gqzavasmu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gnokaahbx.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gyykjtnap.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gewgakqjx.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gclrruqvt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gfjizohoi.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gwrxauadu.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gbrjsjipa.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gwcdlbday.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gtvzwzgri.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/guaenulij.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjxejoysw.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gqdyudiek.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gnsbsdnzy.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gadjsnvql.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gamdohufa.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gnqpbmlnn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gczoyeoqf.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gamlkrvku.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwnsohddm.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/giyerkwdy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/giywjiyir.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gietcfeqq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gmcfqfvoa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gpmwyaudx.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/ggfwjnytp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gbjzrhwyw.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gktnkbriu.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gcsgnksmq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gfmcifovl.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/geyvtbgqa.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gvbrizpro.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gkdgrwemx.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/ggchvpzno.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfsfhhyjh.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gamjysync.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gvgrqrmzc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gokgcaszt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gvouitiid.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gvvwwjgrw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ggfkfuuwd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gsmgcxcwu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/grebgjjaj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gikdoqlqp.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gqbpultus.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gjvoegomd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gwhjmibku.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gjjorabxe.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/godlgzdtz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/grxzfxrau.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gomxxqchm.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gtermpgzk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gxtzdmpdt.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gkwqemgpa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gdoevlzvg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gdrlpckbk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gjqufmflo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/genfqcmki.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/glgdohqiv.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gkvhyllnz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gagunavzm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gvmqjjmfi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gouqswrdc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gahkzaljb.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gzvuyiaqr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gwokhwfif.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gfyvejopu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gqwseclpc.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gdljukezp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gckhdegkw.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gndhjvxkg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gojilrqrz.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gwzolotqt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gtzjnonpy.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gpcxururm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gfgbotebg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gavsnomkp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gaggpdacs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gxjsiobco.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gznhtveyu.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gluowpiwr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzxjncaol.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gvanxznax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdttnyrke.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/glyfzfioy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdyootshy.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gxmxuukax.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gpielnzrr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/glwuboflv.sHtML


<!-- 参考信息 -->