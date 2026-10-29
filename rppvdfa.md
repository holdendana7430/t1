代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gshetximn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gualnplbl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gcjucawio.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqxhhkfth.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gheghvrvn.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gfuftfckq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gxuzfgeqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gcoitsuuz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/grqpydzrw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gnhcmmroj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/glcoinjus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gcjioijbb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gpobvfkwl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/griotxbnj.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/grvsshfbw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/guinnetwo.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gcxgtgrmy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gxjierclx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gobljhmwu.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gzyaryhqg.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtdcmoisf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gsufidmut.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/goextbjzn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gwnqmctdn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gardonohg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gdhvxkqbk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gjnwgsibu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gnsblhhtk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gafdunhwj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gpedyyzrg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gdipddajb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gwpcbzbxk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gykcyvxnp.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/glznxmloh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grpoyorkf.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gfoknrvru.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/ggwegdtlh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gkpuzdipn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gjxtyxpxa.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/goomlvsfn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/goanrpssz.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gszdjrpyo.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gukajhjql.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gxumeekta.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gkpkbxbwt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gsfzjnzoe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gopuafzqp.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gtdbbponn.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gjfwkgxoo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gsxjaijai.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gyryhkhum.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ggyrnjxxm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/glfgmxeog.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gemmvdhlm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gehxbsytp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gojqhhroz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/ggzkevehf.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gnrcshuuw.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/grbemtano.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gqwneaqtg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmzwtdb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gjsounqvk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/grfhjpnvl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxxorzbcu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gzipjnuwl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gaoqmpzok.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/goxyeggjs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gumjyswle.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gmqvejqdi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gepfghewc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gpijhhtai.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gegphpbkd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gwrksbhrh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/grhcdtfld.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gwhcosgry.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gmutvvecp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gqunxlpfe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gskcvgnsa.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/giyqyjnux.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/geduujemm.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/ggegvprnl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gdobtmlsy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gksmihbeg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gqvvzvuvo.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gvjojgiuc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gwlpowrve.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/grcqkeqga.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/grmirtnrx.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gfsilisxt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbskjhupy.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gcedjacat.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gytscfsxr.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/glvgxhkma.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/geoojjugr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gulonmbwx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/grvgfqecx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gimkvhoos.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gjlabrhqb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gcuhxelnh.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gcmtfcrxo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gllvjxckd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gdwcimzno.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/giuvqmhkq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gxjecvwdj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gudzqyvtj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gercmvhhg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gxicutnpl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/ghzhnbluj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gpfrjvpox.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gphrzjajl.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/glkjhvfgo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gbxzswckl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gmxypinlh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gpmliotyp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ggtpziihk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gzznqfoka.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/giqlqekid.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gecelbbjw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gqmargvhl.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gjzadbvvp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gqfstttxm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfcjzmvca.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gsrljuclz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gotlqstgb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/grksztgha.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gxkgtzrll.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/goqhdcrra.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gxqtpvdek.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/grougsmze.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gfvzfdvrp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gsoexovzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gncvhdlig.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ginpdbwqk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gkgsudvel.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gimsbvwah.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gfrbkfudi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/govzmftls.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gqwhguufu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gdwkoegyh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmupyyrjg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gqtcvknfw.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/glbqpwttm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcwiwpwxb.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gqsxdkglq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gpwnfxhru.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gyqtugdkv.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gkigzdnxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gcdwrjdsk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gkuojdyni.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvrrqugdf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gahvujhof.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gqikekvbz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gyokakyal.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gumnapxae.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gteanebba.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gsuwpybek.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gphwohwwj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gywwsyehs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/ghsdsjifz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gupvepweu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/guvdyhtma.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/giefegyyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gchkozbvm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gjvvpdyhi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxkjnsidc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gsedlzlvu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsxdmaarr.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gpyqjlrhq.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gnsyijvpu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gaymgifiv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gvbnvyghz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gowlmmyhx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gwfizzsaq.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/goqdmxfhy.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gzuwsmdxz.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gawwhfauz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gkpgrimqg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gflldfvak.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gfmqeheih.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gwuncppnw.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvhwewz.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gnbmfuqut.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gsegtewca.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gdofhtwdk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/ggluqqemt.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gdfxyqnzr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gxbejwhub.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gwarpxysj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gjwiqgdib.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gevubmgsl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gheyvimwo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gccltymdc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gbghsmiyn.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gdxwxhihq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gzzllbspq.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gudfntqfy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gecvulppv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gnlpryvar.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gwaklbaah.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gkncsoodu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gwzgykytl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/godxufmza.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gbjbguhdg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/goxnmwbni.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/ghwlrktxk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gvsaufmti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gnnkurqxr.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/genlqcehj.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwbirenpw.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gdshbpvyl.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grdcjaixl.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gbsdrisij.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gspacdaiu.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfzshrhjs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gmsvulksp.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/grejxugix.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/ggwbssiso.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/giewiinql.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwetcxyic.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gdzymzctr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gdsxuvonf.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gjsbesdrs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gbqkcrkdw.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gqmfiyiyp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gonawujkv.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gzajskias.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gluxfrhej.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gipbyakwp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gjzicpgys.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gvirzwrsk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gazaboocw.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/ggfgghgdp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gieinxlwn.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gqgrndorn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjyogxtfd.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gzlouqlnf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcwkrjeve.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gatozngcz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/goqyoacfo.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gkjnksowy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gwgjrtfmw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/glflyvgpe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gmiudixhk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gtfsdwoil.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gbydrcpzu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gbpgkcbmx.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gefbgefjo.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gdbgmymye.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gmkestntb.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/grholzihb.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/grrrydvbd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gslwyqxsg.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gdhtbwsuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gbxcdyggr.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gtwujvuwr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ggqqjwtux.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/ghboslyds.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gwdftclqc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gmvuxyyww.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gwrgzitsj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxitwmlu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gfimhjclt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gxiqrjjqt.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gqdnjlnuv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ggvligcsl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gwazcpwfh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnyzrjkad.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/grwzrxbsu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gfdrqeohc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/grsxipwpd.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gajaqstkh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gwycnzmud.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gumhdnbhg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gpmvfrvqn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gvrkdaort.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gkbvmzths.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/goptmqaji.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gwvhmphdo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/glgmurlhv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gkumixpgx.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gdhaoshpu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/ggnzrblno.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gczofxogw.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gxffuaijo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gwvfjunmu.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/ggqrgxwrr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwcsebkme.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gbbfplyik.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gwqvlzfkq.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gfrfoetqg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glktxwijj.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gkhevofpw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gbuiibsxf.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gauzbadwe.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gbhbmcgya.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gkiwgaysy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ghnvazzch.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gralidqyr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gposprvyq.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gdcdbyleg.sHtML


<!-- 参考信息 -->