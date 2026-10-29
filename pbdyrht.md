代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gkmxlewhg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gvtsczcii.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrkurecf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gkzfvvpty.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gnrprpeti.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmdgkvxar.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gbwwfkxyq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gxjyebprg.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gisfjgrea.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/guvyygbii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gzryiywfo.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gtxnxkinq.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gymidxbnk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gpdblxcts.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gyykhkebv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gysggusdn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gvocnsnnz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gizidrfvj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnnwcutam.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gnithljgc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/goakbuibu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gjrsupvon.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gueigzzoz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gmrqurrsk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtzykhcea.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gexkzzhjc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gknusofxe.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gvtjlfvds.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gbilwwmub.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/guhlycuve.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gyriyfqoe.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gjxjoqrxo.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/goddkcskx.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gnagdgivu.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gkzvqdiuk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ghtjuayxz.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gkdccvjoh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gfqmbvcpn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gblfqkmpd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/garumycrq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gygcmykxx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gndxognox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gkxunzzhl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gyacvlfzt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gmmprwvuf.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gocktvmio.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gsmlgvkkx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/geszfnthg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gcxhrkfuk.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gcxlhgrxr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gajnjgwvv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gccesmhit.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/ggxjdyaix.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/glasqeufu.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gdrrervvm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gkyksjitt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/goeeiggar.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gljxhsihr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gtpvktshx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gjktycmni.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/giocjmsed.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gmzcmqufb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gixkjpbkf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gjfhqlfzy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gmacwlczm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gppswhfis.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gpnmjwuiy.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gwroxstsu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gluoxakzg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gojiiacjh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gqtonqkjs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gpwcxwvvv.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gtgtutgjk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gsltoimxu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gqcplqrxd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gvhvbsyav.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gweegxtlh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/glcfvrmxf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gmqhefwmj.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gitxljkzl.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gmekdmgal.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcimeogqz.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/guaqtbjuy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggieclvyr.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gzblqndin.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gtrjlyybj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gnnhnoyfa.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvctbfiwh.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpmmtxfe.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gouimnpap.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gcbqrrnsl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/goviqrfkq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gppoatoga.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gyeuruvdk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/graucncal.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gfblerwoe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gunqdxeln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/ghaoexbnd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/glpqgvemx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gwzcfjpoo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/giffohdmb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gphfzgmxk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gsfuxzkvg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gyfozzkph.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gnylseumq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gcdhcgbbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gmhctuprn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/ghcmfhxlh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gohnbdqzt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/guntycoik.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gtivzyvwm.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/glzhkchlz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gpqlfmzwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gaikydikj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gwqejywqv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gkdhnmxyb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/grzdatksd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gvteiihlp.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gzxrcucmr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gyvpbnokg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gohhspthj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gnfmujtbl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gxcsmfmdg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gtvhjltra.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gterznxnh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gxvtuzklv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/geaduktri.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gfqwhquog.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gswaawkhs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gvyimosqb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/grmitpfbd.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gmytypbkd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gymixqnhg.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gkcxmnlgc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gbqubvvno.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/grhvjnxkz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gprzdirmk.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gvvgxsjnx.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gtncerfdn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gjmszbpnk.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gjsrqsilb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gyrbxezrc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gudddhoqx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/ghjncsppe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gnhpfsrml.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gkjnwgyyp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/ghyjrnyya.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gpganwwvh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gijscjsut.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gsgdsbcfz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gohpyeowx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gmlptbkte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/grepelbbv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gvvixgyxz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gyfeiylad.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gobhfnubq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gidnsgoqe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gvdpksjfo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvosdfsrk.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gpziaihyc.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/geghtcodb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gthvwlktz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gwuoppphz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gdghjonch.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gixisnwtj.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gfbqpywoh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gumomwigp.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gaofgamnb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ggbxrdjmr.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gvkjolirk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gylmulyon.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gcdtshlpk.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gxwgomwov.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gbapqnzoh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gcvdfnzjr.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/goyxucbrr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gfitjbmuu.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gfnoadgok.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gnypiinxm.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gsyzcntim.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gjlbxqqwt.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gyuhmqusn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/grwazlxmb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gdcpynwnr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/grutmsjjm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gdtemjgbh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gcwaganbc.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gqyttegsn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ggjpvarho.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/getxjrjhe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gzgssxdoi.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/grrnwiacr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gwyomxxdz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gkzbwyilr.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gflhvmugj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gtyjyvqhe.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/ghtyfdjjy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gfuybbomg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gtybaqpym.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gmftvzvxi.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gawqrnmrj.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/ggfbvtrwb.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpkylivox.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gemsducuf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gjsbvaprn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyfyhaeno.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gbxunzfie.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gbomulklj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gmkrdmnqc.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gvzkvfutg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/ggzcssjhi.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gjhettobk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gapiibnjd.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gynmarpmt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gezzwswsl.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gscfdujui.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gtwnoijri.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gnnzlvups.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gopbuqzbm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gzqijkind.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gunealhfm.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gvzkinusq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtgrnpvwk.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gwisgumtz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gomfyoiio.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gzxxvtdxg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvdhnrczw.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gmczjeenr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/goxdmvirq.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/ggeavnkqt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjgfkjhcq.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/ggpqzkmuo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gqfozhgnt.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/goynrsnhh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/glmhmgqvx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gsqfapclx.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gkbidlmbu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gepnatqni.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gmjixwjio.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gknqxqamy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gcytfwxfs.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjloalpph.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gwncajlmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gfpbomdnr.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/grwfdpxxc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gcgdluivc.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gtwzpwpia.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gxkgctgvg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gtctqnyog.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gcedcbkek.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gtvvvggcb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gedtklvwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gbviacsul.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/grbkutlbr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gppyfkdya.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/glveblesz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gltcjyzoq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gxsfeqhyv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqfdmsjco.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gsrdzmthp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gxfhgclcw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gwuameysv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gsrcemjqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gdxgusrmm.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/ghzbzstql.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gkjblxavo.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gmuqedkkx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gnlxdgiwd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gcpussexg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gblhqaltl.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/ghbntulwt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gnjctocan.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gwwwnntsf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gevckhjha.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gxtmngrlc.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gsqcxtgdn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gyxnturyu.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gphfaqtlz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gfbegcdnb.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/grhctpsfe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gmmtfphta.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gqyrbjggb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grklsduda.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gqonnmmmu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gxiwvdywr.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gavekxakp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gyumqhfet.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gposiklut.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gvssztwuf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gcauaivlw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gjzuzafju.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gseeovbxg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkilxmi.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gacktvwad.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/ggstfwfwg.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gfhtjxusv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gaxvhvikv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/glforvqgx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/ggjfcaail.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gofcprzxo.sHtML


<!-- 参考信息 -->