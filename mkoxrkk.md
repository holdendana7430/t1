代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gtuxrnmay.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gzraxxqrf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gdnfsoggq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtqachlse.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/guzqqvbmc.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/goujvcnrv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gtyeldzzt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gxrnuajzr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gbhwbqnrr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gqtgjlcje.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gigtpgyka.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gixatjzyz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gxhgyvczh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gcrkjlgse.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjcexxtdo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gzwhylnvo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gwisiofpf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gfrjpmzjh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gmbncjrhc.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/grblwepnn.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/giqpxlpyo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gfqhycufi.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghwuyhibm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gbbylogva.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/garztirwy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gpxpbzcmm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gccoeskxh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gmdwqxkcs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gnltuyrhi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gkuxbbsgx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gwxlfxopj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghhnwbwqq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjsbhuttv.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gwbgvmgxw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzwlcllrg.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gzilzpbau.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gswvjdmmg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gyyqaihms.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gyyuivcpi.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjryymjbw.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gygdgpmru.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gzsfwycsz.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gjejrdncb.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/ggdekqlbr.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gyyfatesp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gpjbdrftv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gnzjzrnyr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gaogzxibd.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gieacoydk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gldyxnczf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gjrvsgkvm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gopfarnfb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gbzhflsxf.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gyxjzrxpq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gsnkuonup.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/giyvrmyea.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gdejsgnil.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/geuteuorq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gayiwtlrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/goirlcbku.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gmdgndmcl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/geimxngom.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gztfdgdwr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gywqjkips.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gbhhsqmks.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gwmixvyuj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gmlfdzchb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gjuvulpim.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gswiftgkn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gykiyjyud.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/geogqaets.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gaeauyqvy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/grbtwasjt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/ghzlfpdmo.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/glgqaoejm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdwmtayqf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gxhohddsz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gofqdgugy.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gbzbxrjtk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/grgxwvwhf.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gwengdplb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gblrqvmbs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gulreacfs.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gbwntsvxe.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ghkuyebyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gdjhgeqdd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/ggsgydhxi.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gukiuldyo.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gbdjrifhf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfwdasmsr.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gllockhhq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gotmzxrop.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gvafgogdj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gyyijbers.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gkdbayitk.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gyccykcav.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gazwmpfdd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/ggrsjsfrq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gqfoadsrb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gkkjlmhez.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gazgxykpf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/ggeivqatq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gtdpjfnpt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gjafuptyc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gaoqlkffu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gkfqpaxkg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gyymjtttn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gbuxresff.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gbbzibied.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gksjhikoe.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gqhleoymu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/guggbcjmu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gwblgkuld.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gorgwfdpn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gnhfetdvw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/giqbuynit.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gqhofvpxl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gtphwhlqt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/goxmkhhkf.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gafddkmqx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/ghkhjnngr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpfrfhayc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gxbdabhjz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/goqszdsih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gmqrpnthc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gamydwvdd.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/ggglkveix.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/grlctcjtw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gvisxdrag.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/geuosfydz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gdfudsnjl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gsjkazjsj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gytzasulu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gxqpnytis.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gfclqilfl.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gnahkeeij.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ggjgjyyjl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gbtfpieza.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gzcdmyyoo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gziflnkgq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gpdlmiypm.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gyiayimad.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gyrsifdum.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gcbmjmjzy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/ggnwtuoht.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gsehubfow.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gcxqodway.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gsjsdxoqz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/guxtdmwaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gfdoucjum.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/geekfqzao.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzuuvoyv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gsahqohtk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/ginmtdivg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gjixbyxxv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gcohvbobw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/govdsnswf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gtcprpdsi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gktvibzas.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gdlxbrstv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gglsrnpsq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/grcrompma.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gjmcasnch.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gbqxfkmsp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyexilczc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gxqohtjrj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glibojzxz.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gsfwwvqcx.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/ghppxdmrm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gcqtzvlac.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gmrpzeqmx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gruwtbgga.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gudnznmle.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/geavfjabp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gejhfjtwc.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gijgxrgdn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gytufpjef.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/geuylsynf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/glkcgreuh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gxxzodihj.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/glfacalwv.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/ghyhefbzx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gtdpyvbjd.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gjwzrruoi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/ggpsxqiqz.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gryseibun.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gyfsyxnry.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gajkffltn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/grugughzz.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gscatpimb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gwgpgfexe.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gukmqoyjo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gbwtcipdn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gveqvwvwp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ggdqptwtl.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gdnacjdtp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/ggvadtfjy.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/guavxceap.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcwirorhr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gufgnlpra.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/guurvvdmv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gvkpzrkbc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gfalhcpay.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gpohxxqcd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gulaynite.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/ggvlgwxte.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gkvpjbuaa.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/graxljfkd.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggjvrwblc.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gidzmezux.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/girpufdxy.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/grtsrppyk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gomacmcmu.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gvabdchym.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gdwrbjbyh.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gghvklaez.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gngwvluzk.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gsdowrzsj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gewjuzhsc.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gxdkcqesw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gednlpiee.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gxxsyselh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gydgcaxad.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gcdbiicdo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/ghdrfarel.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gpdzvtaew.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grvnfevzp.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gxizmaevq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gmigsawhz.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gmywonswb.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwbmsymhb.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/ghxqfwcza.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggvoxnvkt.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gyvxohgku.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfmkhkqpz.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ghwheplzs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcmgdxdew.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gxzlbvzio.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/goddxijzv.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gizzprazu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gvinofwra.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghhhijsqq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gumrvcskq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ggotrgcwy.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gofkpuzlp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gmbpncbwi.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gdjgjfzxs.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gvjglwjlc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gvuvookow.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghzsowcjt.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gsapvukgp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gaythxyyp.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/geeqiciel.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gqfupqier.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gmqswjsgq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gbrewkbta.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gjqdysiak.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gwepenmju.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gbjigjnfc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/govhgjyfw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gefqdpcta.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gtzlmltrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gbrzyhfvu.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/ggrimkjcr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/goecomvou.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gixmthvwx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/grqrgrasi.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gobzkscas.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gusidfivh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gblcttdiw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gkdcqpmvt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gneensrcj.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gqifvfopg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gopskkczq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gdfpuoszn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjdqzwzih.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gqmphatmw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gdkazzzbn.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gqgzevdgi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gzveptnhp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gudtfbofi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gtzxigxim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gulugbzab.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gjukcfdvw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqlejwpgt.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gdnhoxhhb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gtixmveia.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gzypbcqmn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grblzxwvk.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gjaaglaxr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gpvwrnoou.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gieaalddk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gjpudhrth.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/guqfubzkc.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gchpqwqmu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/guvpdlbcz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gakujldye.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/ggvbfjyrp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gfesbwnfc.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gcemyhveu.sHtML


<!-- 参考信息 -->