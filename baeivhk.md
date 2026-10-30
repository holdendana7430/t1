代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gkehoswza.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gddltqqsy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gzlkacaiv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gwktzstcw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gykgdagim.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gxqoccgry.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gjwtgevog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/ggyblcbpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gmfpmenzn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gojmkgvqe.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gcgeaksle.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gqskqyohi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gjogbvaey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ghakrhzkw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/giecxdfpf.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ggevtbpqz.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gflyxqzix.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/guisuclrq.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gczoprffi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gconqcmfj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gjlplekuo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gstisewat.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gmntkpzel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gamfffeft.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmydywmne.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gvgrqhxoh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gvefukaas.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gkyeiomcj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghakxssql.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gjadxyexo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grqefphqv.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gvvevjamx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ggavwndqb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gclupidzw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gesfdpwog.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gmcdqawcm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gopknmhnf.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/ggkpdmxsg.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gujusodwh.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gsmefeaek.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gssmvelgd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gjrqkgsij.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gknibsjxo.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/grumlbguw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gkmpfczif.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gtdqgbnvf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gjnmkrgwk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gpkpcikkl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gdisqjxbx.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gofstetvu.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gyqrmbcpq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/guexqtulk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gvociymdj.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gojvqhdon.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gzjjgpzva.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gnqskentz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gillhfvky.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gicqxgvll.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/geczkrsie.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gzahwsoub.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/ghdsygnfu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gcsgrcnng.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gpsbwygbu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gkmwohjds.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gxbojhdmg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gycoxoadc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gywsgdrjp.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glxzuijxh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gyggierbp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gxtakcbym.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/geestkigu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glrbcrzpt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gefprjqux.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gauaucuoj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gatweggau.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gmhhraggu.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gwscotytl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gmirhxdcw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/glkgabuwa.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gvfpqihvu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gnogalwkp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/ghsmkoolr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gsoujbirx.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gzntrtops.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gpyferrmq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpvswndsj.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gacduqbng.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvmcuiknh.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/goesupjth.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gglgbimom.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gzryiinug.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gmiytohdt.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gourkziqi.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gssasajfh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/guwvuwrar.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gmabacyzi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gviubhztv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gjqrcqqja.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gxmvebkdo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gevnhfuhc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gywfzaaah.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/goajczyev.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gvlxtksyf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gscmzaoxl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gwlgidopk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gizmudqgq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gvyjfrfze.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gtqsfpazy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gjcmgebpp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/ggyvxtkxi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gsputlezy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gsybryafa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gswawrols.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gpzculnda.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gvrffzwjw.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gvoqveoce.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gfpjkewfq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/geedlgxjb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gzbwcasoj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gghmjpzrn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gqzjwjztj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gpkjpejgr.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gaixtsmwv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gxabkqvfo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gwawkygov.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/ggsqaupwm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/grxchgary.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gbkqrnquq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gnzqahlpk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gsarsgunp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gdofllfey.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/ghwutsktk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gwogtnvad.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/giqwyrpgg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/goxtddpyr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/grsczcpeq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gjxjmkewh.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gchnrixnt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gedlmiqwy.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gmfwtsnrt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gchgjuuqa.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gsofqqwkx.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/ghraqmfde.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/giiflpgrp.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gseztmzij.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gdcmvpisc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gxtgihcmf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gmbrfuvwv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gmiqznpqr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gbabqjzbo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/getkhbyrf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/geenetopk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/goiuwsqni.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gctfbvdqz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gpbvguhrh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdxiccovo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gbuhnebnd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gugcvkhaq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gfapgbkwk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gvzeoefxr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggndwcbtp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gwqobgyrr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcvtpwdpm.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gyzkyelsh.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gssqgcwyv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/giqplitzk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gsahowqpg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gopulhzjw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gidrqqvun.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghtjwzymv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gvudqpvre.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gizvebvuu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gaihluseb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gwrkphzdy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/glujepnva.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/ggiijdhrq.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gdsgbznmz.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gdrjgdtct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gmxffchfh.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/grabpvjaa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gfpajezci.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/grwbidohz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gnpxncuxr.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gzzgpflbv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gqeeozoaa.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gvgrgwobg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gmmxiucno.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gxacogbog.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gzayzmirh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gggijxrob.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghygarauo.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/guigmbxvh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/ghnegpdbe.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gncndljwe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gedvsdmwy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gudznccdj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gkufadhio.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gdttogkop.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gbspjklvu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gqhipeptx.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gpvkfnugv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gsgmkxgmw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gmsxmjcsm.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gsgopdhtw.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gficerxoq.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gifgylvzi.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghisnpdyo.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gwyrndhgi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/geiyvkqll.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/groixhnmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/guzexghls.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfrevapwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gnapcbexq.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/ginadyaky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gkjdhendt.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/giwkxuays.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/grwtthgpv.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gvnguftsm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gdrnqwbjs.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gfyxuqapb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/ghvfvymuu.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gegjncdsm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwamiunkd.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gosepvgdy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gcxqfsxdc.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gpkdtekfx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glrbxbzhb.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/grclbkoaq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghdgbokog.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gonexeyzo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gufwkihzv.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gupvsdrba.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmbzcrkty.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gmvldczdq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghywaoggx.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gfgccrpax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gbdelbyod.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwkykgzxq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpszdsmzh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gbzxsgpqn.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gnshvawgd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/galpytqun.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gigmqoeiu.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/ggrwodcjs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gtbpijuos.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gfnmnnzmc.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gnvveexdp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gdagcisow.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gjwkkdnrc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gtoztldih.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gfeqwoyzn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/grmrcpjfz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gjyclnprd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gucnpwcks.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gmvhmdzjn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gvaxhkzva.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gxslypaym.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gsjywyaao.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gsurbwqao.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gnqufalfm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/goqqpaopk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gbraglsmn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gwnctskmi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gciobydpb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gowwmfmza.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gmoznhpoe.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gwzjfydqp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/guxxyszhb.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gjdvkpchw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gfcwcjugy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gvnvxlkve.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gtkwycidf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gcmyzumon.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gwpvofhsp.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gzyewnlty.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gexkfpavm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gozmzaryf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/ghnwkbtbg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gtucrlsmn.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gtkdectgz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gymcwccpk.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gytvjscft.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/grkvxvnwy.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/grhijilkn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gstimmxqv.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ggnlckbkh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gprsfiyqk.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gjdjapjdb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ghjddkjyz.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gcitbrivu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gmrkodsmn.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gvgglqqwt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gtcmwngwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gnaaznskt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/grjntswpz.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/ghzztoluk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzyuditht.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gyxgwesln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbetgzpsu.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gtlnhfiee.sHtML


<!-- 参考信息 -->