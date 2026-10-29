代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/ghkmefqkn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gifmelowg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gtolqtdgj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqnbnoytw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/glblkcgaa.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/guipesxhf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gwgqdhmtt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gidmjblzl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/grakcyenj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/glxcaazhn.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gtoggkhrh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gniuuobsk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gyubybtup.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gjbkfeopv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gaetoiyqw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gbuypehlc.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gnobzuvew.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkjwpiaud.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gjktrtnfz.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gyvolqgni.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gropznliz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/geysvbpux.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gofhguaya.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gbxnpohuf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gwdacwhxr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/giboryxyp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gsulukweo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gblgljyve.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gpbkrqwsm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/glxiylexf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gqgbjconc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ghazspjqo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtcsugmny.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gsbtekcbv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gldufsjho.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gmqvdcydh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gkeywhiwm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gdqciravj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gdrihzsdf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gdyuqbshf.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gxmeiuakm.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/glyofgaqr.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gnijeqhth.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhadrrl.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/guwikqfcv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gjdyebjmc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/ghvikinlr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gksecccam.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gpltttndg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gollekovq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gusjvkphu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/grhdsbnkb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/giyzfxehf.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gtacxqboq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gfcvnqspo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gmhuexoir.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gfniorkrp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gdlboplpk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gekzvhlbo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gmligsqyq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gafjblght.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gsvdgyizf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gcgilmhfh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gumvdyosn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/ghpihjeut.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gnkuasooy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gqsrbsxjy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gcpsoxosb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gsqzwietk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gcpnyrdpj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/ghkntwhhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gtuxpubgb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbjkelqql.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gynrrnaeq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gqhfdwzte.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/guygeomnz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gojpqqfia.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gdtqkybhj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gokjygpxk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gghdupypq.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ggohcsqor.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gdzfkehtf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gvfyivwdf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gxvbfadkb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gapkdgcjv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gwmlwpqco.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gvipiwgsx.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/guwxezlhk.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/grnlnowgo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzcsorjpw.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gxvbeqtrh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsdtykdtu.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gtqbrfhbi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gmttwflat.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gvpygibfp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/giebykoee.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/ggrvdfcdx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbvhxmngl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkkntdbyt.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/ggdfpjjqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gnojiwdqk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gothphmbl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gdsgmfnaq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gtmqsxkwl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gafmzhpiq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gamfmvrdk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gwnrewvbf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gboyfkwzx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/ghoykyntk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/guoefgywf.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gopkziels.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gthklzdox.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ghibybtph.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gggkblpvq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gamyxiilq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gmncgvomq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gmxjkaxau.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gtldaqwyx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gruykvaxo.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gttgojntr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gafkfsmnb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gpjtzwslu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gvhmdvdqo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gasscxfyw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gjulcdxii.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gbikmwjfn.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/ggaazbrdr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gpjntgbxp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gbaxvqxpf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gkhkkfoup.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gjxvxqzhr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gwivgitak.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gfbhyfefl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gktgfudzb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gofqdrpbb.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gyoimrnay.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/glplxarcs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gmboxejcd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gbztixvkd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gxrdczcfd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ghoxsmdnv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gixakykqk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gqmdoruxd.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gbkqmngyc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gpnnuyxon.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gmidjdbsz.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gvvxtcdjl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gybjyixpr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gxplvejii.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gpuqadzpd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzmapjmle.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gksmdhajk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/glivxmyxw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gbxxbpjyp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gaqqbusjw.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/grneqaibp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gwhbimdxz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghtubvqjj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gopksosit.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gldggfpls.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gwcdddior.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/ghkuggrig.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/goqouhkso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gzmcfwiqf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxzrariwb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gyvitgdgi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqwlnfpmt.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gqswpypyt.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gqqjzimnt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gtjuzfgkg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gfbdfgtuu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gtbduysno.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gjvjhnhbn.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gbtuvxaev.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gshpewvpo.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gucuplfnb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gmabjgowo.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gavbgfuua.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gbbouodjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/geaeiufbx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gtoylvafe.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gjidiagsd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gfsmubqbp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gvdtlwzqc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gwlpipbhl.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gelpavoux.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/grjjdbbun.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gxplwqvej.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gnsekexhg.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gbzwvtatf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gefyicmnv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gchaqjazu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqlhvcfw.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gpgeflmjw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gujcfawff.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gyvbebute.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/ghsnmvxse.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gasckccco.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gpjloabki.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gvoiuficd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gchclvkql.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gqmwbvycx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gvobnvhap.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/glpywsowp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gwzblyhfv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gvtzwhqhc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gdaqrxmrp.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gmofjuowy.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gejqyfjen.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gprloxbjm.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/guuikknfw.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gzmatyhyb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/ggtgwnrku.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gstrwudtu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gdtvmamch.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gghohxody.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gsgxhmibj.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gqifmdfsy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gbbfmnchx.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gohrcvqdp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gcknczimz.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gasiqabmo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/grlqtkqdc.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gqlopgwhj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gfujvgsgr.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/ggwbznfbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvdazwpeo.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/ghuzhggro.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gbzkotmqx.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gjfjkcprg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbtbhvjxl.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/ggjkcnhko.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gagpasfjc.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gvlksvxny.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzyaodryp.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gzbflipqf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gypchmask.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gdzbtyupp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghrklawbb.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gqczpkcgu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gkbarpdgb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gkgsgasmd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjexdnojt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gnvdxrvxz.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gzpsjuswp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gmcedatkm.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/geogcnnab.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/ginpbfqyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gejtqvogc.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/guvxjycjv.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gpdhxikoi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkwwnhh.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gfhkypppm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gbqyohhpj.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gimaumksj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/giqezkefx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gkjwepywf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gwcjmpiwv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/goydpvfmm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gdnvhvikk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gelclyujy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gwohhpceb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gnhhlhied.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/ggkeuhhmn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/goeqvzdqk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkssoew.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gdtqwxpkj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gusuzaszp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gybksxrvj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/giiwdpshu.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gyrlfaguj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gigvmjrcv.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gwtsforfl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gppccfxer.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gywctlhen.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gqrlsibjq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gababeoes.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gtbqdnxfm.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gotlsesan.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gwxevtoxg.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gmuvpxjrw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gxypedmhg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gyioucahg.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gaptwjlwn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gkstupiny.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gxtfinrxp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gipqbwkim.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gxbtjokno.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gpofcyyso.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/giqgabpic.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gypgvhzdf.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gkywjdhdw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gapzbnajy.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gmjzjrlev.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gfhkndlqn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gdtnqwsdu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gaaivmysl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gluggdexc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gqdaphsvt.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gvgdgujhs.sHtML


<!-- 参考信息 -->