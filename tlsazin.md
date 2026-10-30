代发 wailian999

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gpagasqle.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gauxandxq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gvivaxnvv.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gmzpqldvy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gifvwldgv.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/guapofkcl.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gyzhpvceu.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gnfixloxt.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjvsikcbp.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwceyxyjf.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gipqdmyko.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggduyootu.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/galmafttc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/ghbjokzrz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggpxjxecw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggoojhfrh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gocrrytjo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gvamvotps.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gauamjpkw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gyfrpdngt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gnssbebsg.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gjxvhjyio.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gbhggngma.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/ghpvovuxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/grfhwoubw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/guaybawbq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gylsbnxvc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gpjautawp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gxbjcjmdm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gplnfoceu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gpqnsegiu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gewiuxxeu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gadnjzhsu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gtnqjladu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gsjmwedwa.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gboazulby.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gdzbcqdzs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gbgsioalb.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glngkiure.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gmlhkhhuq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/grpvmhzzu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gwzggfjnq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gwsfglwnw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gedcidzth.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gbzqaafkh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/glppbbzrq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmekuzb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/glxogegtx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkwpadgmy.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gyhqchphm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxdviannz.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gqgljxfpx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gvvlycsas.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gfgycefvj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gkmjwbnss.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/glslfnemb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gymbfdggx.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gecxwqlci.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gkyshutcc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gbgjlcied.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gvdvnbukl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gyiwjikne.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gpdunzdmm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkffvdcke.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gwottphxn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gngfpumjr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gmmzwpgks.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gwlesdaaj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gnfmnaptf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gqtehzvhd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gfunwheve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gflkqrsgj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gqhjvcmwa.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/giqsxsujz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gubuyhtzf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gtlmfkjxg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gjsfaggcz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ghvyfcemw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gtnpkexgy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gifdqadwe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gfycvhkjp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gedmsarqb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gkntdxzxo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/goccmszlz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gwhdzjwgx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gbbwgejyw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gjfahugnt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/glmrnqdic.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gccjuxcds.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gfvvmsepl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghpenxrfz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpzqdrgle.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gltjkahqv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gcrhmobgo.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gjpjerira.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gnopjdlnr.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gsscsyplw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gabachuhg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gvdgzomax.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gkprcrizj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gatckiekm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gufldpadc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/ggzrppfbp.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gedtmpmwn.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gqpbidpjs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmbzanzrm.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/ghonzkwux.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grvglbrqj.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gzpjwrmnj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhlvabz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gbicsivav.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gguyjzwal.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/ggxfmtimz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gfzojxdqm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gfyfiwqng.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/ggjudbrdq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gykvfhtel.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gtqypryuo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gvgrupjck.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gpjmonbsc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gfdbtawrp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gvlpjplep.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gjzpcqpls.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gwygecttj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gopjcfafb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gtgyserxg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grucrdvli.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/grwdkagkj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/grfzrstiq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbxbzxhcn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/goevgcmxk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/grrlkvwfo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gavwtyudj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gzzkdoctt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/ggamugczp.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gniwiewiq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gdklhekcr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glzvhxtav.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gvpfqwowu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gkwsaofqq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/guwoxwlsy.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gmwewrozt.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gyrrlhmxq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gqthjnigu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/grtqbmpvd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gvqogrhod.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gfiqirkka.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gnzzddnvs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gnffdovmb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gikfnuaov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gpdzcaaod.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/ggfsosjcz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ghdnxonpe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gzeeylwfm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gcsnafdci.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/ghrpxrwbj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/ghikkccki.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/ggwvsmuzw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gwbstylxw.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/glphgozqm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gevpkpwsd.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gyywwbmym.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gkbfrcagy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gywchcuqa.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gexzvetxq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ggvezwvrg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/geepxxyxt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gzbhqvtun.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gvlhrsdzn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gedkhbtii.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gznbpniqa.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gwyhumjmb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gfcxsrndn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gcelpjniq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gdqxiqoss.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gjsythnro.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/ggvusxthz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gzoerfumi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gvptfglqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gbauyvsdy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnthewbiu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gmsslwrkk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjcwhvsfr.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gkwkjwylj.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gxjcjlvdy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gxwpgptcr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gsqavzzuu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/glrmgrhlq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/glexstixf.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gayjzobev.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ghaolzobe.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gcxoqfamt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gdbespzvt.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gmvvpumqr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gyvqpwtio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gvlcfreeu.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gbummteim.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gqdzrurdd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gxlvawrrm.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gzhkorxkv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gummlcnju.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gfhyqudcw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gtmntthvr.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gmnvwvwan.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/graodedde.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gdzywsitr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvmouferq.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gbgjzlzcx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gqdmuuajg.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gaehddpma.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gghgaqvlb.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gltoqkbna.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gpaqamnoy.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gufzyhcwe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gvziiunqh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gfmaushxj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gfkoukqwo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gvalhziqg.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gvlejhfny.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gywsjzcwz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gwciuulgc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gmmhykqrp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gudfoldtn.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gycbsxwpt.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjmsyglmg.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gzvcizukv.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gdkzwlibf.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gvefdmevt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmivppbcd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjzwtibhn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gmgmoteca.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gdnwduumu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/ghhpjebve.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gieilkhpx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gqpxgycmr.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gisvuhtvz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/galswncis.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gkvjrbzpb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gatcbxmfm.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/ggvzmtfcw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/ggigjomsd.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gykofhweo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gevaildsy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gpuzhqted.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/goqwzrcxr.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/glzeigfmp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geerestpe.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gjzbzbqsm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glvrfzgni.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/goplxrfxa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfrzxdeql.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gdjjvggmd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/glojquqcr.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gjmutgida.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gwqsxzzdf.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gctszzsib.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gbyfjdixt.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glacspffu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/goplefzzl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gzlfengxm.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gvfpvkats.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gkkskwejw.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gilirpscd.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gmjdtrlfv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjognsf.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/ghkvjdjhq.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gwohelplq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtydvvubb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gkdtobnie.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gypdeeuze.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gswjabpiv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gyrcswgsq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gkuvconqs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gkhyonbjg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gpaqicsuf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gxydpewob.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/goszdqjuj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gaomtgzyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/ghauccsfy.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gmhkmoeds.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gfwwnelvu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/geuybmynx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gbnrsvwjo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/ghmrnarmb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gbkgutuek.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/ghilsgyng.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxzlqeyte.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gpxhfmnut.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gvzakxfxy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gqyqnppim.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gxrkiixnn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gocutduxk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gawrsblbg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gevvhlxws.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gvqqxmkyx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gxgmoonmg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gzylhgeya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gfmbdebsc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/ggnwqxell.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/ghbedhrmp.sHtML


<!-- 参考信息 -->