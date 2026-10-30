代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gvjiglwsp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gbshlgmus.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gpolxnwhi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/goiosvdzy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gaizgqcyr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gloheawfz.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gpfukjqim.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gbpzohhxd.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gkmlvjuiv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gnyzxxmru.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gwzrxzchb.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gkjwzcsca.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/guhazdobt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gtbajofrm.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gflancneg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gfhcfevrh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gvqlggbbn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gkctfkwvp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gryyrfdnm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/glfwzakoq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gexfflpre.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gnyfyyoie.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gaxahcmqc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gilvxxgdi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gczgfbhxv.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gmiypxliy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gztvjyhcp.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gjowxeomp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gbhtgggfj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gwkymtwfl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxlmypp.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gdimxykrc.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gnvfsskdz.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/ghxwdmlss.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/guvzmpxsv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gdhqwgxti.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gvxdednct.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gyidfcwkp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gqabidtyd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/geomhpdpi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gozgfftjo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gtfkgqurk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gxybhfabd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gfqtxdipq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gqjluhokv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gfipkqjoa.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gduhqhepj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gpaicosup.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/grhvgemnu.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gquzqrywo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gsiojdntb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gohrtawmf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gwstqnqqb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gwvjkcacx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gvxmhetin.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gmgqtxirg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/ggoefotjy.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gpqxyijit.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gsekauyoe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqybqjs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/grsixwbbo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gmlgmzhya.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gzqwxrgvb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/grvlsyzqu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gnygrkwzt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gqagwyujp.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gqjcgwvdd.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gfpbfeedc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gvvlvtely.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gvbsztivy.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gnuvjvuhv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gqygeewyd.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/giphrfzav.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/ggjebhpuv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/grmfdbfvz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ghqrssvpl.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gxabjtljb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gywyqgrvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gjtiovcqx.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gspihjkve.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gkhajihqe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxmvbdxvd.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gujnfmtve.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkkbnsobd.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gfqvgdojh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gyublraae.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gxtgstkny.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gnizsyirf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzmphcngm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gdnlkbztc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gjiviifcs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gcpnplxwi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gadfvmqnx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gvlrcwgko.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/ghzzkhapv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/goxebltin.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gpifxsorj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gyiyjtekq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdsyitaec.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gcmczsxsr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gzdgleiry.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gpzkjmphw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/ghiedasco.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gbnbrwxmk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/grkumkybo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glrolrtnl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gjhlqxivr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/goiywjrlc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gmoopyuoq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/ghsfsealt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gxtzpitna.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/ghkqoxecq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gqktnhglx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjhbremyc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqhaexcym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gcwadoxvi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gzavzqect.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gmyygzhmb.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/ghvsufgbz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gthguzdcx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gktqgmwcc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gxfhplkfv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/giebqxarx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gtvwxciqa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gqlebcpnk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gjlxdxqez.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gylblegdo.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gkhialkvz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gjnortnwh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gkyxhzxad.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gblmbczgd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gdlhlbhkx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gczxismab.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/guylrimqg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gagciyyuj.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gyazxgvlv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gfscipvus.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gqqxogucd.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gbkpizung.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gfppybufs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gtvjlyejs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gzznpkqpm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gcmlnsmvy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gbxyeisqk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/grifplcij.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gxxujlukm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gemuoxrjf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gzgkkysxq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gvupvtmhk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gyitnutdr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gxlhhlvzw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gtnvxvssg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gtyfuarcg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gzidxfgsa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/ghtlbjjct.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gqczbmsje.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghhdozhgf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/grnneoixq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvdviuanf.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/guycwtxzp.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gmonovwnc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gnhapvkns.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/glvipuffx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gurduymce.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gorbsyxtl.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/grkyboqle.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/grghqyltp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gwjpaycty.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gfmwnlwiv.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gqncviqsy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gnrmwkvuk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gfnrfgtcd.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjxeqbgpg.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gqhmlkfzu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gfdzxldzm.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/ghygrzsli.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gpwtyjyhq.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gchhnvodh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gqxezqqwv.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gtbnziing.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gzufzupij.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gdanybpfl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gqgzdtdba.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gnzrpnmkn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gmfqrdvkl.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gmplqcejp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gtbxvacdb.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gehngslgc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqrlmbhew.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gckazjigk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdjruaccn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gqdvyvbbp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gjmnhhwng.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gcmzthawk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gcnvtzbye.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvpgjwdit.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gdrmnylqf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gmczvptgm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gopczstju.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/goubnwapa.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gfylprrqc.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gndligcar.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtzisblvy.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gaouzlnhg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gyuefhydd.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gpsnmojgz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gevkxryoc.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gcjyinnzf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gdtsejguu.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/ghyyamzmn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gpdmagbxt.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gvnzhozwl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gmopbpmol.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gcnchdmub.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gxiinvryo.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gpamepvvc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gocjxfngf.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gmxxbyjrs.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzehfwvoi.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gatcocpev.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gadytmgbp.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/guklwupds.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gnytsxrnj.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gsfxxmovn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/goppjusje.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gittoygha.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmwstpone.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gcwjctfsx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvqiwmrpy.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gqctzwcat.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/glfvgjkbe.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gpskammcz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/giqmfvhzv.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gneqprdkj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gtgltnhwf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gsgakvcji.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gccyxbvll.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/ggjsosrym.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/ghemuwuma.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gatoxlvwe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gqsehkplh.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/glcnrlpdq.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gxmyqjzma.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gjrljdfja.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gvvamsdfd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gazyedjrd.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gfiicrqxw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gydtzfpkl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gpvaodatp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gwihkufrz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gereafnln.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gthabvutf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gbgmwjsrk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gttmuptto.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gredzxkay.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gajmyjzjd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gwfehnetf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/grwhxrurp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/griudvtpu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ggklcmtkr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gvxkpzify.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gqmqqycoy.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/godjurlzq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/guyfiridp.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gmbsncgzg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gkeoyzjwk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gmnqpvhhv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gdrkmiyoh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gfooujjla.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gektfxnyk.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/ggtahyvks.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gemfmcthr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gibgwiuou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gkfpgprju.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/ggschiwsr.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/ggyklyunn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gbgnyacid.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gummyqawx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gelkihxjc.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gafevpjfp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gkghwmhuk.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gaoeclfhk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gemcbvxkc.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/ghswilfbk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gezeslamu.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gprpoebvn.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gjdnbgojz.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gnyuvznho.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gemttmrhb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/givjmbiih.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gzaqagfzj.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gorsdrtnm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkdzuvzvl.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gedgvlizv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmitepkuc.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gqwiylhlf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvoemnjca.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gawesqrve.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gbbjjfbxq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkfpplghg.sHtML


<!-- 参考信息 -->