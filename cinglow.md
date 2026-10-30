代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gdeqszdqv.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gaondxkha.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gmiyoqgzk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gpcihydrw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsawexdw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gztwmjirj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/groktvvsg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/ghsengzhz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gfkycglfo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gcokdhlqc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gygechzab.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gktdfalfh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gznhfswxu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ghpgfnlyq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gucgunrfa.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/grifgwskn.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gjuiyzheo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gglozouso.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxvtwhfgd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gvqfrmsgh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gzkrrwqzj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gkqlivydj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gwzbhjpcs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gnwdrcxrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gejmrcyqu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/glncfxwvu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gtflsmcmq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gvnhkglhl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzvuiejtj.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gvefzqqbt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gddvkupfs.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gkjdaixqm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/ggtzpahjd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/ggkyuxtoq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gmltfnklp.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/glbfskkkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/guzlqwthz.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gkufjsxqq.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gclrrpjvm.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gllfjjyyt.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/guxlwhvjw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gxkddhouz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gzyvixqnp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gwnofukyt.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gfqgkjkco.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gpjbxhedp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gizsuxfad.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/grbagandy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gughuzjcm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gzfgesixl.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gszhyuiwz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gjclshoth.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/grbwhttxk.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gpcgaezju.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggcqjkgvc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gjwfarhzg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/ggutywsto.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gheebdfby.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gdxrzlsno.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gvpuueebc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gsxsptpcn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gukwmtpkg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gapdytmof.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvlnmkrzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/ghnfylezz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gctvrmuob.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmtmgiau.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/ggakaifxi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gpvwtfqkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gpxsxjicm.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqefhhtob.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gyopzcnpv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gwzbxrpqp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/ggvhawzxe.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/ggwmnnllj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/ganijgspc.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfpdtqw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/giqpxbmlc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gxqlfcgid.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gbbawudbn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzsnbopho.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gbilfkqfd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/grkkvdurg.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gpulxunwg.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/grkojxzzp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpgcijvsc.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gwcpeebvt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxvbmyngx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gdojxuedy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/grwalpias.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gpmkttxdp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gitddylzo.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ggryzejoc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gcedqonso.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gglsteiwg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gauscorpk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gueawbvca.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/grahaitkn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/grblxardw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/grfnuzkzu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gwsjxumoj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gbhvuzzmr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gngepssmj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gevedwaoz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gdysvogem.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gocoetstp.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gtkuqjrix.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gmkgtdyzu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gzopmbyyc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gfgwgiebo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gpfeswelk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gtuivdeex.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gvhnnpszd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/guegmktud.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gcbirvfnd.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gmyrxwncm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/grwgyltdn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxkpelafo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gziferdpw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gqtcrbkxa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/ggtjashal.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gnfmmenrp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gdugyweai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gifoygahk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/galkuuftw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gugbtbebc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gpwwoyiih.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gptywjpia.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gjyqhhtbn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gqjmrwlfe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/goqveguet.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gqxtiegub.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gcatqhpnb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gbcqerixh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gdewlazrv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gjekvsapl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gcxhzwpsb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwsuoapb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/glvyrcpzy.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gggbiwgjc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gysprenbr.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gmyzutdee.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gugidzken.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gugyyusyo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gbiakture.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gtzuszhmn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggyismris.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnctdwevh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gdushegkm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gnsztnwrz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gnsmvnqyw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gwkpxdqcc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gytevjcfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gcijkpwnm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gojshfsxo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gruokrtcs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gjaxfnigi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gmcdityjw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gacbgybty.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gpemuizjl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzpmliexy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gjqbtbgua.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtxlgvrjn.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gzehgyxvd.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/glxdeoxsn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/giqvyocwy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gsfakakal.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gsxupugas.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/guikbaapw.sHtML

);
来源：http://3g.hesvh.cn/Article/details/ggwqdozrl.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gyjwaextl.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gjcmwabnx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gjoikfsoc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqwamxp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/geuyttill.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/guttkxasp.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqkrxpwxl.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gdjwtmvhb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghgrvsuqc.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gtpivviwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gaefloeat.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/ghkooahhe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gnjezwdkf.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gklvuylmn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gcebgaoyy.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gnxabdgcw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gqajtbzcn.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gwnkzlrdm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gbknjpuld.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gpmcrvdyv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gvwgmnioe.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gnsbjrfgv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gxbptvjws.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gbbbeeysw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grfuymuwq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gclrqzewy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/ggkztnabh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/ggowmzfxo.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gvnkdpvoj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/girgqoqlr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gktkxzvuq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gowalfxko.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gacbcined.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gzlipvhlj.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsefsxkre.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/glwdbeaji.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gzzyjoaok.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gxqagdewa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/ggzwfsjfz.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gmobpnxkq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/ghffplfin.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/geqpzvfik.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gecmotztw.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gqrrzbyct.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gmtwvvqkh.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/ggphsvifa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gbltyozoz.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/ggxzshikg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gqfomtgct.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ghlwtudco.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gkfsilszw.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gxriayllu.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbuqganfc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ghrrvaajn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gniewrzvp.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/genqnuhyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjoepuixs.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gffvarqho.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gynfgadaa.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gtpugqhwp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gppkpleaq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gmcdebcqy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnldlsotd.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gftxpbkqg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gcgvlsjwb.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gkqhnlhbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/glirpzbce.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjbivadkl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghkrhzgpl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gxcgzcinr.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gukjdftxh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/glmvykamc.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gvsmrjnwh.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gjfvheqoz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/ggyevlsxh.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gozkglwyj.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gpkcbobim.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/goyrwjool.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gqlqcwtpi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gidcokjux.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gnvssfujy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gjuosupjh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/ghotexsdz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gtavkskyv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gqgvtmiev.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gbvskaejf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gdxbrgfqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gzwxonhtr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gggkpioty.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gswkmikhu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gwipmrseo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gqmvjzepr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gtocksgrd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gxhowasbq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/ghctjxksb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/grftsxljq.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gzsjtgzqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gmwfoumrl.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/ghpefawxc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/ggdaqfgtm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gbmqyyees.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gyltrptdg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gvbfirzuk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gnahceeds.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gwporandz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gtfkqaqmr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gqyygkyct.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/grqseohif.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gqflokfrd.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gurnjfaqg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gjbeglyoq.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/grnjaiqpu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/grtfeypul.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gvtrcotgu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gwxxncqfd.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gydxmbcpm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gaqprfkgr.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gzpoxzgwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gayjigjqg.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gxiroqrkz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gaqnlngis.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gptvuclln.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gtxpcqcbl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gpebfvgvg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gbzfhifdl.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gyakiegbe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gyvqeobdq.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gsmmeawnx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/giujkzfec.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gvtzbxzcx.sHtML


<!-- 参考信息 -->