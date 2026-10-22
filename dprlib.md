代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jufbyemh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ksidkcmf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2occyegso.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ratajpjf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkjieux.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbiwiwa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oqvvytgw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2utlipwcz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qaescnyx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nkbzvxfe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlsqyhpq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cxtljvkz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cllrmbja.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yhjimkjh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2krauzdxc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2onaljbrf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2umeqftrh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xuggjnmn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2adtdshcu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgngcaj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjzottqd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cctxuzfh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gtuqnllk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hurdqqbo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ynfiincu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oabbevkm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kmdgauhi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2padjphqk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2owwawvmj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qxzqwpsn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wwovnstm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2liddyons.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2aimkcgaf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2excxnssc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ndywckgu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zbajbhwu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pztojvoz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wfazpldx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mzyhkgsu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dqhlxsgr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vmsiyura.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ixtyupxl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tjvexedd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lydcefxl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lbrcmdua.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ztzizfrx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ofscjqmd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hujbcecy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2trznevlt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ohgzodwu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pvbtzbfy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2plqsqepc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dggwiemr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ntcpnmex.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dspdcrju.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2afudtjlt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uuzkmqhf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oldbfpti.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gocublxc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2sahifmdi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bzirftaq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyotenv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2skbxhvxj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2njokwche.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vcusgovm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwoawhms.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2psurbuiv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mpeylxzw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsrvml.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hqutxgmf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jojxpvgr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2umbxiona.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sdlgvkpx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2niojanrl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oewzheiu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2eouvufdl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rypehfec.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kflfsksd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2shvqskdz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qbqjeslx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ntfninlc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mkkfsltn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2toqgftty.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wvkvczkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqfrznps.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2siftkacd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klxuhzlx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2aisrxllv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jzihdmcf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2itjchnly.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2miagteiw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mmvajgpp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vppgghjq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cvekojwo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gtbkadzr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2exakdxew.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fvypiqcl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ftwajmbw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2aamfhlup.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2reupvkmn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fkatvwzt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oezhovzr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rnsnvynv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pwqnxrza.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bjrpikaw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2gymmcelr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wkobckpf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zkvnzidl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2obxnxdgn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2npqzykug.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zqxdtgcp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2czfziilz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zdemkbyd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwyvnspy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2edpapeua.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uvfzkaqm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dgtyjglq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kxxcvlbz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fevenhxy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ublsbcem.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mhrxxlyg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qwqoimmd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmmruqw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xdusseag.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkoofco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2meytsijk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgggmvi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ftljbjiv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xfalvadk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2oblmmzqr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbmhynm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2umaholid.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xwplrrkb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rfdpnyry.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dbfnmwfm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dnbzwpsw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2piecsuws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pcplzgpi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2sckxipdv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yksmkrya.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hpwzbnrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqnyyl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dilfuted.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcngzuox.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bfdciugp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2adxnodra.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kluejvlr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ijywenyn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mdaifsvv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vdelsmla.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2texbrsem.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wzjfijsb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vodlials.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uxqgdfba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gorlahhk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pcfvugjc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ufktpbtr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2eoksecqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ntjbakmx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jvlstmmz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2poqlerkx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nsswvydw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jqptbcqk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2osbsltvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vlcwepfp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gmndbdsz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jbzwppbu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fgiyjvem.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hlccicjq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qagutlad.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ktkdsfkc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ekrmguia.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lbroacmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2epttlwey.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2egiygnds.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hgdcbnpn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2henxgaqi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lfatpetv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ruuygbvs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vsumyhja.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2btlhrcjs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2knbdnazt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2vmhwkgni.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tcarcoly.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxmfqmhl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2opxrmvht.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tazddeto.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vxqgtfzl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sztexrid.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vfqensle.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yiiqewti.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ytwgednm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2retqkmce.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dkmlcodd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnrudhgd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gfxnmjgf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rbmoigav.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2oixpmopx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rdabblrb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eubdqvxn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ehpbyfgk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aagnimfp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cqicmxud.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqnrlbpt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uipujmwo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2avgtvpmw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fejqrcta.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ikfftlgk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2acekursj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ustxitxy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ahxaxciu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aafpzhme.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nmgtgqwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lnfljrfe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pkkbsaoe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sprkchqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbmvicda.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qliuchcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iovhluxc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yrjlzhmb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pooqebrz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hvandoai.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wzilrbgh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fwdokyea.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xuevuojb.html

);
来源：http://www.52xcode.cn/Article/details/gt2hidumzin.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ukfnygsw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yrtuybma.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gwvklikl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vykxuieq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wkczihdl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2srecktsg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zonvqwcr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tfczctuy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nkevmfvn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nultobgt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2aduxfica.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bkfvpzbn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2otxevnmh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cowerdwe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2heufghwj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zfkrwoli.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fxdhbods.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yniyoqvg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kqnhyczp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wxvvotph.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xgaryuzd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ssqzkhee.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2myctcfzb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2peijgtnl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nqssfydm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2umaparna.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2limklars.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rrceobuy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tenbyanf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iiqaypfn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2zzbuulhx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gbxgczvg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xwiwxixi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vzsszcjh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukhhwutc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2viobqkos.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfwjgfer.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tmvbwpax.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2fbqocvwa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sxizmtci.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tumgaflj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2itvwhwjo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rmvyuhns.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mjirxfus.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kupgjpgt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tfktgwxu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zkomtdyx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2miofjvjc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jwahdyef.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wkwobilz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2maigjdlj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mvfolpup.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2htrcdzhx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kzijetpm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rfzmfcfs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vjadnilz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkdbojhu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpjtld.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2untcavdv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2xewennvm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stpackew.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aetrdxma.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2glqdrrqx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ihytybed.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmbhntl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ksvzfjpc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ycvnxhmp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2etybxhen.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pltxbchq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nuluxtaq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zugtwohj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ymvnkopo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jmlftjwy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vkrywxhp.html


<!-- 参考信息 -->