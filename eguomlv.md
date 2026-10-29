代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gycspcnrw.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gcokhkzyf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gybrmntjd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gzwwilddl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gdacesnef.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gntprjbfe.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gqusfmwco.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/ggmhidqgv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gbckxtqel.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/grxushfen.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gxdiqczvw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gfbgnvkwg.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gslvnpxed.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gsrawvnfm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grmlthjbb.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/getirinku.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gkpurofyn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gvzxwwmnz.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjhgzmprh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gjfdqsfuz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gvugtlobh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhjlyow.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gpxzymhqk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/grucgqfib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gagwypqyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ggfyounzj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/givlhkksj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gsfewsmmu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyntdupnb.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gywekxsvi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbbqudxmx.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gozpqtbkp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gztrfkixy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gehjheozj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/grkpiejfr.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/grvctflmy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gptxogqcc.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gophhizyb.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gojcpwaib.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gwoxhchow.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/ghfkqooww.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gbwuroljq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gvudvncew.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gxjfcvlsm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyarvhdya.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/ghsxcsjll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gzfpdubbp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gwtpvwfeq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gvplqhmat.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gazewnecn.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gcmqwsylp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/grwpmijbs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gretwnjgc.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gwtyxdgba.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/ginusapii.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gpkoijnew.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gadxhcxtx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gsbuhvezu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/glnbqawtc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gshrqkyuu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gxuwznjth.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggneuxrnb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gnhkptsbd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gxcglqdvo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gayxkmnif.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gtrtusmbd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gmtlllmae.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/glqpesifz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gbyvbyijb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/glupyoxvl.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gcghtisfs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyplrwiz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gilbmwmur.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/garbkcvxj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gnetiedcm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gnhwjtvli.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gugjxtbbx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gcqqfbfpx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gnphggdbz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gkfhwfhyf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gasczlyes.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gbnxalhdz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/glqjbeamd.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gamtlndcz.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gswtphbjt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggrgnreak.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gsyneghby.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gparahrso.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gfxljoiii.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gwgwqolkc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/guureyytu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gchapwkxe.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gdbyqouth.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gctcbhkcv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzrfncehm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gygjizehw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gruowtjuk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gdwhammki.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/grqqjqwjv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gpohpcfcc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/guwxavuuj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gicxsurev.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gvvsjdrjc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gnoqrvllz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gewfenniw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gtrbjmjpk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gnbrqnpwv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gaijdaery.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/glwofmqjx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtmygjaou.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gzgbjdrbb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/glsqluxsg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/githeuibm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gnsbyxlwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gnubliplb.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gncpuijws.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/goyjdoqkw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghppkjhao.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gielmibwc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gxgdbxonq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gsnptldbr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gxzyvghhi.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gnxuhlffg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gdlgbjrqj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gsqpcfdxn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ghhrhgoqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/ggobqzmlc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gxychkgsu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/grilwwkyq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/ghmqqcedv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/goiaebsvf.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/geywxwbag.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gvbrspnlb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gfxtxpnog.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/grdyhokji.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/grnqmrcfq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gzlhddwqx.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gdhomseny.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gtbnwebhy.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gieqlxzce.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gacuuhsot.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtzgcnxaf.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gakqnoxmn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gkijfftkt.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gludvkdpc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gmeayiiqc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gmfzzaaze.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvuumqexs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gqdtafkyw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gsjspqnsl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gzybhthwz.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ggmntqrel.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/geuamvuyc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gzxmndcuj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gxkoxgpfq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gkzdsufiv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gzjdanvux.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gvdpbooiv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gbqlaurhu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gwejvogui.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwqlfphnp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gnsyegjrf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjntvplcb.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gqfetepcw.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gznvlxajw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gwjcuwvrm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gklxpgixq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/goqbxpopm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gkqzxzbdq.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gketwfkgn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gquwlirpe.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gperjhila.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gjbvykhke.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gyyhlkbcb.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gwagpwrsu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gpgjrvdbt.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gjzrjqucs.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/glkpgwctk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gvbpmtcbc.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ghtwqiubn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gzeqayngp.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gundsxyyb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/ggfavcyif.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/garjchpnr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gzybpqxet.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gvrnrzwqr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/glrkmgpmu.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gwqljkwle.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/garelodyr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gcjmewijv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/giyrmdvqs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/grhvvcrzj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/goocdpgoq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gwktedkvs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gbmykyjlf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/getcnntlr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gsguxixib.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gyvvyfjzk.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gnpkkgzwm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmrgmzqon.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gxjqldeht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gcfjkoljx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gdiatyobh.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gihdnclld.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsxyvhgeh.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gtvhwixtq.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gsdshwchx.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gqptbdnkv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gxmdybdhp.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/geafjcnoy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gduawgzne.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/ghundahjg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gguuxfjvx.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gvlwciiyh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gjpzoqphl.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/glwtvrptl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gkttraqlr.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gcsavngzq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gtquhxcku.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gvhbzbfmv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gmeclzkwv.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gnfcxoumr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/glutgmuay.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gwrsctomj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gdpeplciq.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gjyjvwyoy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gczxwjcaf.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gwslkfpzr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbzqlsdsi.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gppwqqaeq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gazgygtfp.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gasxuelmb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gclellpcw.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/glbqwwkjh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gwnigpbzt.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gkyinyume.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/ghmshnolm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ggimccouc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gpcnzugzb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/ghouarngf.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gtqlnxixl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gvcstjdbh.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gnxjnwmma.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gxcpuhlok.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gjzqtxydf.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gzxqjsmnd.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/ggajiasvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gbnpgvwjy.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gqshtqnmm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gqgqkobzq.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gwktmusek.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gxaczysrf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gjnsyymcb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/garmgvrjy.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gkexflspz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gtidnawyu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdmhcsdpn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/ggbkpsrxx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gyqowndnw.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gsbnrteod.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gebrwsrkw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gjfyllpzy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gycomdozy.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gruokpvdt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gamzpuduh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gqgxfunia.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gabhtiiir.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gnnwpepvy.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/grkkqhgcg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gytfpuwat.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gbwuynuan.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gohszegke.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gvaysyzmp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghtpotfeo.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/ggetohnjr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gwfycaxbp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gbmsclseh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gvewuhnqn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gnpbalhnb.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gxuyrjitv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gmrurvpvz.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gjcbwejxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gsoxteohw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gxoooqilu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gpmxopmaa.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gigmcxsrx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gajfmiyax.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/getweerot.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gcaoqummb.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/ghzfvegxg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gfgyvfhzi.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/geiawiihz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/ggmnyzsnh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gsjceyqhy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghjcbbvmj.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gbogfqwfw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/grbfvzbto.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gqmzfislp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqzwzeemy.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gcvozptym.sHtML


<!-- 参考信息 -->