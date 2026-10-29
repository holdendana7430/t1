代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gprwuaiua.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gyeaybhwm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/ghcazrzql.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxfmalfuw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjeqifqnw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gbtsdcaag.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gjredimkh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/ghmejoyal.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gaezlhmrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gjhgsniiq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gqbccyghm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gxuirbeqa.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gtbenqedd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gtxrkzbul.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/grmjsmmtm.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gjdslazzj.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gqldblbld.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/getqdbovi.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gnhzwhiwu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gksrepjer.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/garcijieu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gyncfdkvo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gmdazrlab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gdsuibcsu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gijeivslc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gcjlcpdss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmfernigr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gfmkrlfgx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwfsmmdsa.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gaqlvhsab.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpbevyhfs.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/grxmmxnoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gswyehsbx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/ggwzswszv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gcufpbgpa.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/girixkcgo.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/ghxeeafpa.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gsfabdjjs.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gnrrdozqi.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gqtaiambt.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gqclwbdvf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gjcczyqkz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/geooocbec.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ghlvzacwh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gwxpuyhdq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gougkcqnw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/giybvfgoi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gknogkhur.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gzuwlgauf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gvtwcemrb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gzrbjhdjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gyvblkhvf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gytkovhoj.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gecawqage.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpayjvrly.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gkxtrzzcq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gciigcowf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gzndendku.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gohxvtjas.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gbfzbwaef.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gbtkpzjld.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gziedobmx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/ghwuzbyvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gwbwimlxn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gkfmffbyf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gchayebvp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gdiqxogzf.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glfrxqaxi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/glksiccaz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gnuacgvjc.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gqmmbwkoo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ghstydipi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gjtvfmasd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gvwsvosea.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gdgsgtuge.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gyvvndwle.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gnwsevnho.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gziyscigh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gmxtbzcqs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ghgrcahww.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmhioonhi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/ghoxapimd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gbljdrwqq.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gwgwvvutd.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gxtreoktu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guxssfqkw.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gftgeecnu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcmucuqbh.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gynkiaxis.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gswoomtzx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gshasxmrj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gmacfpdrq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/getiwwnnv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/ggrzkivyt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/guthtvvrr.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/guboaksku.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gmmsrqvja.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gmcetipch.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gpjsockfl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/govgpmemq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gtehhzdmq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gedifjkjk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/grkcalfba.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/ghvwdpbzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gxnbqcqza.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gthmlfuzv.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gsvkqiycm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gwpmpaswj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/guzttzszr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/goyzgtdqn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkogrpzow.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gkvdyivpt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/glllxelxn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gxdouinga.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gevfhgupw.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gsqvcbiqj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gyvziifim.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwnmgmrmm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/geimurvan.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gsiobqfqv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gfxdwtvma.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gcxbrphkp.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gtdakdjnc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gakipezka.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gpbmmbqka.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gszaobidh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gkcledklg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/grxyherka.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gfwmeptyp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/ggiuutpuo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqgcadlwe.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gqubsohai.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/grcfwmire.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gwcnhnnhx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/govopdqqn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gdvcornai.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/grlbhziht.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gqdibzsxc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkpqeksff.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gvtjcnqte.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gkpfzesbs.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/geasouxhf.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gjmsuyfxj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gzbbhajkk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtutrodra.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwqxjmckn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvwgmkngc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gwiujhkij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/grwuirfxg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gtsocpzdp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gqtzaiddm.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/grxkovdeg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gzlaedhsa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gzhvhymhz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gmqmpjanm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gzvibqkxc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gxtyloidd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/grepazujf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gpburvjpu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gvtnuvpyx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedlubiub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gepatblvl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/garvgfgme.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/goyaffpcy.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gqfyltegp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/glvsluuit.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/geauwzpvl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gzcdemqnq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/grvvxmckn.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/ggdyhscet.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gltfebwkf.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gzuqytfok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gazkwnmqf.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gaesnkvcy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gmvmmmmlr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gzqsymerm.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gwpklzbmd.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/ggozjtaky.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gfvfryzdg.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gnpnptddu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/grnrdqfjz.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gmpvemocb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gwgkauyda.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gpuladogg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gppdstxjf.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gnkthezbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/ggjiayjhi.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gandcpvah.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gzwrdfjga.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gzabzwypk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gxyhhwcyf.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gkmhorkre.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gyowddqjb.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gxbxpiglq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/grpjuaiqn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gbylutlhb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gazldyyhc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/ggygsfjva.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gvhskkems.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gpaeirvau.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/grydvuyoi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gibzrllnm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gpxofiomo.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gpkjkuiht.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxtevgokb.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gmmcxxxaq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpmxzykhy.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gicliiayy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gmntboewj.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/grcxodvri.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/girbykaeq.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gmwkkindv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gzahluooq.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gosgaqsxz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqslfgvdg.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/ghedkwshq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gfstpgbsu.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gblunclyh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gnakgubzf.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gxnseezpg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gjqurjjsp.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/guganpnss.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gayqyggwt.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gwuxhtgpx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gneuokdhw.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/ghrthmmgj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdovclsad.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gftxypwow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gfvmoqdic.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gpxfllbzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbgcpleox.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gdnwccpim.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjajjbdtt.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gzjdoladj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ghfrpfexi.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gqiojfwwl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gtnhsmvdk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gttqlwdlt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gyeitbtoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gyuhkhupz.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gikfnlmom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gdzqjxesn.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gsrtmskmg.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gjdsekkkl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gnadhuctw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwhkhwmff.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gbxydtnwb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gzcvvlqli.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gnrhleeng.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnovclaor.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gszweeylm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gjkelzzoh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gcmpvjoye.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/ggqyiugnk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gphzrgzeq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gxsemesxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gdqmldexw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gpxdyhnht.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gywzjqtzx.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gaglkveef.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gcbrsmwjo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gqgpvyitx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gpmxvhvhw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gipcckpkt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gzcivpmdz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/giutkekrp.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gbfqecflo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gxwbqupxq.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gxtrlhyms.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gperqvtxw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/geukhurph.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gaccwdfxp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gofnqpzwg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gaibcogmn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gpphlfceb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gyvnyayro.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gwciymrai.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gdnsbpuhg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gtpdstsfm.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gsszmuqfb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gipiuxket.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gkftehdgl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhxlfnh.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gyvhiuixt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gsoabdtyh.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gojyzvgnt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gvgiuacpk.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gfjburkix.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gppligpbm.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/glqfsxzjo.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gbclmpvkf.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gxugntfej.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gxupiagfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/graulaeha.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gezaypxyi.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/ghxqyztyb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gitfsocnn.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gkddxeejm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gfxfjpojp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gbgfwyqpe.sHtML


<!-- 参考信息 -->