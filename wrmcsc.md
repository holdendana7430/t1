代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iftzhmqb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kyfrktxc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3axooilzk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3srigjkod.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3irwlzdma.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tnpbtrxq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mmzntjlm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bvrlnvqn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ervuifoo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zgjjtdlq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3frmopysw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dfsijzyb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbedkibp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zgvmsjhw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zursdbgw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3thgdknzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzclxyz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lttqscyk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wacqefmw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gymgpjwx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3exeakakj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qoijnfmx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vyrbwohe.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fcgakcbg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcvnjgcs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rlfmyezz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rvrihljt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3swxlmorm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qduoavtt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yuuzxiim.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3svqhivza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3atphxfft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gidhgmqs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ukdlxftc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rbzrljrr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fnnovren.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpimdyjd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wyteaome.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwzlokpd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qeafhlmf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mjvvvveo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3foohvojs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uvvrwdmv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ntdvfxwe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ecwlavfv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qpfduekp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3psgkpizd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gmwmcrzs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vqzwfmyr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kozrvzib.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3biretunj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3szzguvyv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mzegkufy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wqjejhgj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hjzkqbcz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xmdgsddk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hzboeaqh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3iosydlje.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdccavoh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ugpjlyxw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dmcucvvv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vucczmhe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywxiuhvf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3figcsnke.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yqzswstm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3twizrfnn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vqxqoren.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zmeamper.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qiakhrwo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlvgjtqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkvkhqgq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uhizdxxm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3slturddz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ldmcxupl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eimcyefe.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mwrgbbyc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpmxwaz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ozsseoxf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnuzbju.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iarexwbp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pfkudeov.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3remsejdp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sifubtxh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcmtjomn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mkyfyanv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mhlbywzu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3crimfrvd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gxaqxyng.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3byziqrai.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bnfwluos.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3stjequoq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fatcutna.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3mxuvnvfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woofmpig.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dlnqepfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjkizzfx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3opszxjcl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nseaylwn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xfhbrpnd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ixumrtvb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3payqzgrz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3clmahyuv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nlcasfzy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vifotghp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oradnyvd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bmbbtspl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vtvoyoim.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ypaadgjy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cfvelzac.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xsawvazl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sdoaalvw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zvbluzgu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3iqbopkqs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kefigbzy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rpgqrhon.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xiazkgma.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3plidhwph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nujhuens.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dgacfmtz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbbmwsj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eoztlmqy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xbrpkpvg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lanzawov.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ixjoacvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kmismzmp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3czayznzs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ynthbvzi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hitkgmtm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yrjsrjmc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uatuclyb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3afpggcyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vyxsyxgz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tnqkiiak.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3edpsszmz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qgyqbksh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3juiumang.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdygiof.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tpwlpqmn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rqyzceer.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ijezcjqi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3otawvhpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pociogun.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mqjayhst.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dspltfdm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qdahceus.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwewwwcy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvhffrsw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wltevzfz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ropiichj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhenag.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jmaaxqzb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zbklopac.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3irpxxals.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3abingdok.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fsidaaai.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xevpfxut.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tfcynuqq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bsdpmlkn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ohcniljf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ceywodmg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3uhwelplv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3trloiocg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xgqeyitg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ggdjhkhe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ltxgkdiu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hqaphspm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ocqnfstc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gakdlzai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfqasnmw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3huwhnkgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhnajhoy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3klwtyhjb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xbdvdgki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tcsmbbfg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xjgbyyzh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fltzzsfo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xftmbqbl.html

);
来源：http://www.52xcode.cn/Article/details/gt3lxnfmyzf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qahpgeyk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3gibkjdvh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cpetdjyj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bptcbmya.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mhdxqort.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nnjwkrrv.html

);
来源：http://www.52xcode.cn/Article/details/gt3swdntbgy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wwvcfffb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3beclisin.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rriaqcpz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3txeypwin.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3iipkczxy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ltopvlhy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nihmelic.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mwsusgaf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lyltxllu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qfizfupm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3webcscxj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3shqneyhl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zaoqxdfv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3krekgnml.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yjpmfign.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ylqzmsac.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ifxjmxzx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fncyipyr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oocxcsrf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fjaccqkl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3clzijxvu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vwdnlyvw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vlugizsk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qlzyodha.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wpwhdfqj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ogbsrezz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mikhoiph.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezmdygjk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3kopsjdcj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prvydbxp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pkapmjol.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pkukashr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3solytrbf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gghjmnsm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qfknrfsl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bxxoxuyd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3npawlipi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3eceairuv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qdmlhxbs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fbvjmiez.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3quikfwup.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mtrcoyik.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vjcvtdzm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3putxbgho.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fcdhllfi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmvpnoby.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3amaudgpn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mrtpoczb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ialnaszh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrzycemw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hbroobmx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qiavxfeb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3atcwrreu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3losiyans.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fykfoact.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zwimdcnf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wiskgflg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vomjtbkr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jzsxvwqk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fvngdadz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jcdvybaf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gtbwobbh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zcujxvwr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ylvewujw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wqkfjytc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qcsztfli.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eskezvuw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lreqkglo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3twgjivdp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hyhxruhw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qaoedelu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qapjdmqx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ygfqmgae.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mzovsoux.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3yvmqlnvd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ijfbtpey.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tnrrolji.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vonizgal.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3iwidgxed.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3libzvnwu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3taluqwky.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bffwwfoj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qnycezaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kckwebbw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3yfqlvlwh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nusljfdr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eildgzmy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pboxrmxh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dtisuuqd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dtidoqjc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bwehfetg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kurgecbj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lrvfkvmt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qswbqgbf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xqdzfbtg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gtidwwwn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3icfrynue.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xacmkctm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wmrtfqcw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jxyjslrq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3bhplcqja.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3owvhpzmr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qlzklxcg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ohcpvzav.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gnwgqtnt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ysuagdai.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mclnybxa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3otilxiiq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3elbteixg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3elsdygqm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zmvtdsiw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vejnnfsm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yutnudtt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3yblrihbv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zmdvhamt.html


<!-- 参考信息 -->