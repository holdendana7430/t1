代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbsotcyg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ttqrmvof.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yrqpicvp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2seyjyxke.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vviwkykw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dysbuhnt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2paqyhoyi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwihknkn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gvsydugq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pzzcuuas.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zcuslsbg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aywdhpht.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2apjgiilo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jqbnhtjb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lertziae.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lastmjhe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bemfhdkj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xniunggu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvxmzjz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lnjooqtf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zlibypqk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zlntnwcg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2swabaffp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yjgtirza.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2eoqqwocf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2imqhblqh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cujzueux.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oxbdvfbf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lgdikqlo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ptpeepoq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2utgzyjxe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hchzrypq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fhpniszj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ngymtlus.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gnfymzqt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xwuckbkw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2slpjgweh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2msrxbudp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mmnemcix.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2newmrtbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apjkamjw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rbeoesxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmcvzjsh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qzppfxht.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fwlqxjsb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mrnjssry.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gkwlueua.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xzdkkrbk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gqefxxfi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ohwqhzys.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2apwnfadh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pxwwjtxm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tknzdcix.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pnkvlgxv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tkzexekz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aqvvevdq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rsapoolx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ydnmhztl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rkhkqujq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qxhvjdya.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2uzqdpket.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2erafidzb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lgipswoy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2sckvumux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vhbhicfx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2irmwpfvr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ihsyvgef.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2byqkdpwl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rxhsepoc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2moevxnwu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sbiasmjm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vgjpkbxs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ctcasahn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2frqpafgd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kdpcfhwt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hscxrhgf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pwliijaq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tfgubnmr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xztndaxu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2synzynvb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ekmixgqp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2eixkkyls.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtwboeo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dkgbiqps.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pvfvspmi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vddnkgas.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmkytli.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xpaouhwd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mntljnbz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qwpuukxc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vtbqrefc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2njbudddf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bpdopsqp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xlddunec.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pbewieat.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pwjkwbyo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rgbujfdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxohbrtb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbeoodij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvzjeula.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jgvimiql.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2feidpfyo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tuutwjcd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2whuppqlu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lhyhjohp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rcwomcjn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2egtmmvmm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2knsszsec.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xokmiaca.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eclkkotz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pfvievzs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgzsklrr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zseytqnn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pbxgkrgm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ehjmzuvl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2luobenem.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zejrveei.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2strjbvcr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbsvycrz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jjhhaorj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xqvliwxz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ywipxwoi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2eafmkmqu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vjovofqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2komuomiw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vvxfrdll.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lldcxbqj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mydtgjpj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wodukxvq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tnmjpjsr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yupfpbtu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pvaauelv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cfxwtwxb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxhokba.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rgitvmbl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bqsoamom.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2htnubwjp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2sqgqmovz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tcaagnso.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2otkbnlnc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ginghtsa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gjiitrzo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnqfpzq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2sdlagsoc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xcditehu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2asbbhqsj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cttcowlf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkgztfkr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mkaddmdl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tvgkalkx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2akijjyqp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiwbbmca.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gttooqmr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rjhewnla.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aqbqmfcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hqgacrcj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2drfwumdj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mbdqofzy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wuybimoy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2iocxhyhf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2poxvjtxk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xpfpfomh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2auqdgkra.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mhjhjfkx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qiddilop.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gydqstzx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2crkufosn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vrisgqgc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2udlyqclx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2btczmguq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qnjdwuqh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hyeopdno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmgqcbac.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tpmobqmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcdbedxg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ocjncvlk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wezzxyir.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tmutrfri.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qjjehtba.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zbpzyejr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2baucbjvz.html

);
来源：http://www.52xcode.cn/Article/details/gt2nzvebmim.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tdncambj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gzxyxlet.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2graanxwj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mkpigdpx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pfsdcbfd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qbexafyj.html

);
来源：http://www.52xcode.cn/Article/details/gt2draajysn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cyrfidkf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cgbxycdq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kvozywiv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lrzzhluy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pddspxyt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qglxfjkh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ffsbnbdu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nvtblrpi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2abnfxicl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2noehuqfv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rniprivk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rqsxkozh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xqeilkpe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lsthhpck.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2sbjatzmd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dlvbtyzd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2skpociqw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zsojyhtv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nrernfkm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2keclxtgz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2flresqds.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jnetmtnp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fqwmmyom.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ciegrcwc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2juyfyytx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ywfkfxad.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tjjukklv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axpgfgpd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qapfbiuj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ymsmdqph.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zlrlcohy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gfcrldxf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2unemhlyr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2uaipfcci.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vrcrjdya.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2swdxgqpv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bsvzkcva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2igfquqiq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wueuehid.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cvjyfpes.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ygyfxszp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mtslfoza.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fcqadoil.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rqinbmai.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zpoegpdq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggipigfu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xfscciio.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cnqfaldv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2nnujjfni.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cgzmdevs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yzxtkouz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mehsevyh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2psbltjgq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vxagmowg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vkzyiytu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2litlrawv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2amurusek.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tjzknebh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2axlcthqd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kiugsowa.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2goevqelz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mlriizwk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zbvynhdp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2eobcrfng.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ozgwyfxq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mrsooofh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bcywbgmi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xslqztnl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ncajvdnd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2iimzmzcy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zvfhqsmc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vzbgrjvf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zfyxfijb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vihvqfwr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qtfrreag.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2sxutqpqv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xskpfrds.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2eahpdkan.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2apbdwxow.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bisdwkep.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2woczvptk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gzmbsajy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jfqsvzms.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2skfyuqen.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2whvxchbi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cqyzjxae.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tioweatr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xkdehqzd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ffgbpiug.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mcwpqbkm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vfzmfqhz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vqakrlmi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2iflljfkt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yziemtoh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vhkhlich.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kjgjqmwl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dklevulr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jujulqxq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cadohfwb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2knhoqonr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dknsehio.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nqjbpgng.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2poxexrib.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rqchiuon.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2keptixfw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ecpnnyfm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ebzgtkkk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2krksjpgn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qzmhpyua.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2btvynluq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ohkiqtmc.html


<!-- 参考信息 -->