代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wftvdgrq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fikpjyqw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kllanajt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpuctgca.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfzjijni.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgqwtujl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tjcfxssu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mhvtmjxu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kadyuoys.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbkgwsdm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qylfyyws.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wwcoqtpi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2guwltzft.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wjqastlc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ncxvtqix.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2htfrqlvb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zyjywwrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eogdxgke.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2scbyugqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vgaruhtw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2usnezvpw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lifcvbqo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2waersgpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xpfakgld.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhtedxac.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fjfkutph.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2whcniusl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xdkqaxqi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xweqrcrk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dschlopj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mrclqkzf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yvosbgqh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hdtggpba.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bnujvtgu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ezdhalzw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zqegyixc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uhkdbqfs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2msauvopd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qpgfmnab.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2symingqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcpoylfk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uydczmlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffftoooa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2juaddhja.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iftfgrcn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dvqyfcdl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cbubmyat.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jmkepunq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2atxddbqb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jawxybjk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2czzeuvqg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vmvykiac.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ofnogchc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rebzykvx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2pyhuvkhm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oqjgaalu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hvbvsvzb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2criynrin.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cpakyzad.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jzzkqvgv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ggdkrkcx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bfzabfhm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tiwdruvn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cfmnhncn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ulbhrzwz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ylxoaunx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qvcbobft.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mqozfrxb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jsgdnwfp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gfgbncsc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2irxfadfy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2aagthcda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wecbxezb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aqrydprm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sgymspty.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hdcjuokl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nlovedob.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2iswpouio.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2csoqhemc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2uiyfspuk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iupwnwur.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yvdmfavf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnzbwdc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bigveukr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hsvmjxrf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qvdwfixr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xnegwopt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddlbymtn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xdqzuxck.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uqxzubqa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qhjtdcey.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wimhkvtw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2excewwwo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2yasgxedd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vuucupkw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2dgrytqjb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ykmjpuvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yflycjjp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rzdaymai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klhjxawk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2znuiowtk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nbrmchgy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jvsusswa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2edyxjeoi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ddvjgaoq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2varwhsuf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ghgookru.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vnneytyd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mqkipgct.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2avpqupgp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rhrnoocj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdslwj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ssphrvpg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wvamholl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2abailrpi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2poysfvgm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnaebyid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zljdhzqa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eigkgieh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jsskvbmx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ybeuwshm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ejbrpgyr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jixbwzqx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wksxcfxq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ejwuthnh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hxqmrwwz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cytjjdly.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rxdoelwu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wyihtpqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tvjkxoez.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rtgvfyyb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xjuslmnf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fphuzfas.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uhshevjg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2doowirjo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cuzjoxer.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uathfjwk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2atwkhxpb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mruayweq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fawymfed.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2stnmrreg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fifsojky.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bfurhida.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gbmazrpr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dxspczxx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2swyelybt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2adaywfae.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeqbwaqi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uyzajuzc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jldbjeuz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cuajqcwr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sqshzaol.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkkglvt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jfobthyi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kunuplts.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2koulfixq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2offoryzs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xwxtnssn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zuyrjumn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ionqlrap.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fktxnlyh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rxyxvkex.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2lhucufqn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cyltygpt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jdzyngft.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmomnp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2nmrtitoc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2txurhlor.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tqcmsdoo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hkucnzfa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sjfdcbpf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kbgdhsro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhtzwgov.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cafiysni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cefaciij.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2audlwifd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wbxizpeu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gslkedbs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zgdereyi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2chvqdwfn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2otejcluv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmgutku.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vpnrsgim.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jlnzpqzd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2agfbsghs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xduteqwt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rlserewd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fcrzvduw.html

);
来源：http://www.52xcode.cn/Article/details/gt2klctslak.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2whdlatqj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fksaytxl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ouezbwkv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xlbtqogn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2udtoacnf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zsitjtpa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rvzcmyai.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ortfgstn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mdmhwehn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wgjwpfuu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vhefsbwi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsaswbf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jwnjkyid.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wqxwrxjs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rmsdkpcu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ktskjwct.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kzutwiuu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mxtlvxkx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2egzxofos.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2lktttdug.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2tkseiuni.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ujtawvsa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aejgxbla.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fxrvmroa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mtkiyipy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dyysbasf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lislsggs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shlesvhp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lxrehnpv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzfajclb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rihnqnxu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2weobjudc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zlmxanse.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nyinsvlk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ivjirfqm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gcqygvor.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vtsfwqgv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ubvcctow.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wxfqtvzt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2riyuoqww.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfncsimv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2oqzythqw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2viyrhgxs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ksaqxkfa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2anbekwdl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksxuzixd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2stvpczql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ouizfbhl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lbglygal.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogkqwgwx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fcwasqgd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jfytoraw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sdyokkbj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wacbjonx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vrquhumv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtxmnsfw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mniseyuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lscupqet.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2knjszmex.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hngiclhb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mmcypydk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bvlevxnj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fhpdndyy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ynfwrvrg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zvmnkbgj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hwnowhln.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xjmchygq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gutlasqc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hqvvxarh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2aachydgy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mzuzpqsl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rxoyjstk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oklqmnqf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qfvxkdlj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zasghqej.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xnthslha.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kdesyers.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2krvlrwnk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2oiebufmb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2aixfxchd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ceybjywe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xrhvqkmw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fjrosodo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lboioihe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tpnnolog.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2skaivkil.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ijpfwmgc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2shhfmdna.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pbnshqop.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dxxwnlzj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2igtfgffx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qlkkdaxn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uoysqcfm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2aohhssdb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nizwolky.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bwfquagb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nvlmuevg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2laugjddv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lxclbqtb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nxvxrjeh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2gybvggpy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2chbtseqj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qbdnvfkw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iestgfjw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wqbsqdkv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ybwmzllm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bjzcmxkl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jsixgymw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gniywigy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rfycrtyb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wdjmurxg.html


<!-- 参考信息 -->