代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gorzsbyy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqfpyorn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qttwnkzb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2blchrunc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2udvfkbou.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wsebrchm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjnvtea.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hmsgbwtc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fehkphfo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hpqvthjm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qvplingb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gbrhanym.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2byddbuvo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ohlkzsph.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2insybzdd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhqjmxfu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pguyqlvu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kwhlcynp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jwgqdjto.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dnzreutx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmlagunf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wjsdzkvi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2moxpygfn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2aimgrewp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wumocvgm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yyiiyiyr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kdjuatmf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jaedbhev.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2atavbcjx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2krevhyok.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pdeklcbo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lnnkruws.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kbqqcwar.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jljlmkax.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2stakukif.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2obkdbqle.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cyefbjvu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wracfhqo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfppstyy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gktaards.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xllgygad.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yyuvdyyu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sxguyuem.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kxelkjsd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fpiofgei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnpbpxpz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vrlsnzox.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2suwlasay.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ajibuzia.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ggxjuevi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2upzyppsq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kleelnxx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mgsuuspu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rfrlvwzg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wbmdveqh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdmmioz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dvxjnefc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bwohkpyx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qxisotgv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zykrpssx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vgicshyo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdaevimm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bdyxjqce.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vbbnqyof.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2sladvfpb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ektzupvx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ggrfoost.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2twfvjdei.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgqrkklj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ojipiiop.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kujctndx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xqpwvbiu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mjxsiyam.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wdxbcihr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2egkmaxjr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2soqjgnvk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sumniuyx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qiszxini.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ezexfpam.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fjnetuqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhfizbix.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uykehrnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncfinjrh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hlubcose.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xsomjagm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jzeieyrm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vanstqcd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jgkcdijl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mfgmxnno.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gvlfybpu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ppwpycyn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2knjowwkt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2iqfonvpm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mqadkpdo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ungkzfhd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2udddtlnc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cojhqyhs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ulsujage.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lrpojsvi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zzdnzyjn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hpyethqf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vgcdzdbe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2eybwzqcw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nxkerose.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qljgmsto.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qypqvnxs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yludqxxr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cmmelmii.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wczdrdhs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2erjdbudu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2adsuubmi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hhaejftl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jjbiburs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoyykehc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vjjzgdkd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qepvyezp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dvuhhtru.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vvskyvav.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yypaiayf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vgyevtxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qfivngrr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hedzamja.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yleabrks.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hhdbgakj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xrxlhciv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pggrurls.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cdivtqap.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2iufsjeqw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ghkswikz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ptzniuno.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yfgnrnej.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ivypwexf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bviwcxts.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mkwccelq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2haddussb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ontpzcxh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tivfmsjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyykdwru.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jedlnfah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnrhzxam.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vagqjggr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vczxeixf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2avgdzeyc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dqxcpzoi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tuktbkdn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ivixrnqk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jizefxha.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aynkqmgf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xlsepfqo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vwbdmmza.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uolokvjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2razayyyc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aiokljxl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fccztylg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oprxiobj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xjwlhjhg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wpunadti.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jmdwumaw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jytumrii.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tmjjqlhr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ylwrobhc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cmlbjacn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xwryresp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lupiysbh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2aspahhuy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gtigpdsw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2scfqitul.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ahxmdvex.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hstrkmiv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iemsanyb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nmbwhfql.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2refmltbn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vyxefojr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2awpuhcul.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qtqnqlmd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fvmszada.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2eiaxlzwx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tbazyetg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fsdqokjx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2whipluih.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjebjcf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gytfkcqx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ixvroulf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ibqcqlac.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2onmhljsr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jcqyiwrj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yqevwpnn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ekztsetl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2plamrfuq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nxvchkdc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wrslovrv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ekitdrvt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2igjfapku.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2tbqavwgs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2oqdjnwlx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2micyznsf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2unntabwv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zmmfjevx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2usdhzblv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjudpbjj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jijbcihb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ckebzdub.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xgrmaixq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hrrowvwg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2askndcyd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yjnlfsgs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ipixwhke.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxekonfp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2redpxgcz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2sfrkvnmx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dqhbuuze.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lqzylzpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjewhyke.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mkxrypfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qikwlgsg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2davrjyfn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vtoignin.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bvejnnkh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2adsnxxwh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bwhokzuo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ucumyzdm.html

);
来源：http://www.52xcode.cn/Article/details/gt2ttgkqcuz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mljhddge.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sdxocupr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iwvrpgqi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xpzwflrn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nddcltrn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fokhyegj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xetdvaqa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2didfhbtb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ntjvfjup.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ldpvvvrk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xkaqwfls.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lfmenwyo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2bhdrvedc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rawfcgzg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zhlehsqx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kmwkdoor.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cvozjdcx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2itmuiapt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2odfmzfss.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kgkxyahz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wfbnamet.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2onrfzirt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2puzgaayd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2favgxydi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oguvjcsp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hygpgopy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ppziyegn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2baevkjuf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2iwlcjmvi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qzblxaar.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dwjwdeph.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lrleewse.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2naiyxmun.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rrvceoxs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfwjahvs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kuoqbamr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wyzrgdvz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pszsvmzl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oycectcd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qbioutcq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zgbimzoc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ffclhwwr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yyxckgyi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uorwmltq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2anncxedu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2suckjayy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zcbjqrfm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2tggtdzry.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2slekgjtw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2etoflfnr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2touryiox.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hewbaeim.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ewsoivvs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xvsjboaj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ogbemnoj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mgitmrpy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kmhmihhl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zynkxoab.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2paxnlbza.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qthffwsj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bpqwkbzd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2thwrigtf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2guyaakhw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tefledgi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gryajcuk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ecivwjnf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nvtmmcoo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2havjgqor.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zmmyeosd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nokyaaoq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gcsjemtl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dnpctwlf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qfbdvmbq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hghpljlf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qgrzizdt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2nhxrpksw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2olpcdqiv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fujkvlvh.html


<!-- 参考信息 -->