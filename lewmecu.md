代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gswsyllir.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gajqptqhx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdhszuqhm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gwghdjlsv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gjosryphe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gzkjsbbwv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gmmxyzlvo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gxrgqnyil.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gteelmoeb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gcvvifemk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/glhcxkbfc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gvpmdcabw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gtjocshbt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gcgpiqzvj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gwarpgyqj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ghpbxvrwb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gicuhztmd.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gtgnasdgb.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/ghefdkwtw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gjnikekjw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gksiofqwz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gjbdkerru.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gyfjumcqe.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gphfnbajo.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gaklfahbe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gjwdsqxrb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gktrrpvui.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gsicsnoaz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gahuxgswp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gddnnuxgz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gwprlfpma.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/grektlpvz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gvdxydoje.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gcrjcjkmj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gkacdwipi.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gdwgciejl.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gvxpjfrrh.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gqxzjktsa.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gozxmuzts.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gthhqfodb.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzecihkmy.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gypietvgs.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gbnhknxyl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/glbwugfkj.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/goewznmxq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwungntad.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdsvrtrbx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gwnohrnde.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gaqqmthtz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtqlotpnz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gwaalxnll.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gmghsrfcx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gbpvoskpg.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gwcarzxyj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/goadxpvvk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gtcsoqceh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gexymsklo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gtrkpednq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gutidtsup.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gyyizzvzh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gvflvntak.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gxrxmejhx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/ggmbtrgvj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gvdsvmcvr.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gwwsiwbvk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghtmtcnxv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gdologmgb.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gelbfrkpa.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gymuywvap.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/glrkslfqk.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/guellaayr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gngkpquwl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gckpmxhyb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gmorcxtcw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ghhnmovtc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/geyqdjvjz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gkcxcxrpx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/ghvmwivko.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/ghcqeroou.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gmaubicnf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gieizsfnc.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gbimxccjt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaukcfjmt.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gnuoagzdt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gtushnlvk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gglaixkfe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/glchvwjel.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gcwhzejre.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gnyyfpemf.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gwqcmwssp.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gslahxrok.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gvtttseqq.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gwnmdlhjp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gjwlnkomb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/girccwsen.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gfsdftxjb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/guebtmuir.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/glfzxgwor.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/giuhgnvib.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/glfgsnltm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/garsjwqqe.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gczsaaprt.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gjqufhohk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gtwtnxxmq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gkhqohvfd.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gxhfxgbmc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gaekcawqo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gwovuyett.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gzowqlpal.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gatnmiugr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gxmvuffat.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gkkyssivk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gabilwnht.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gpnxyhbbz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gvnardomk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gfkqqbnop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gpgajmriy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gnwloliac.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gpwpqlctw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/ghyizgjhr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gknecwbyu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/grvgbpvhg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gsfcuejzb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gezleyond.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gsbawyvvr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gkpxxdldy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gbnezacse.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gjgysixzd.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gzubibvev.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gqwvrpimg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gkiajtqwo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gdkyqrxwu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gddehhpxl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gswcdtrtz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gdbcugrrv.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gflrjupxw.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gjyabaadk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glbtfquya.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gkzwmihvo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfjrikkga.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gpkicgenq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gpbdjhius.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gtzegacxv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/goyfcnfrx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gminhogqc.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gacjpofwk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmgwavmpk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gaeoaehvd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gyurnskvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gqzjckwyx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gsuamsupb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gyhghmlax.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gxjvyadzj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gjkvuwjye.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gkklqeccr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gncrldvjk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gmfhtvhnp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gnqomgclm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gyahagdbo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gfjjmmagu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gkeotyfzo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gjqymwols.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grnoskbtw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gctfmoaol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/grodsletv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gncbcgpyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gftignpyj.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gxxvodtrs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gpsrpmaxo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/giwgzihyd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gsgdlgrxj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gagrorwbf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/grdprdhmy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gqkfkbswn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gyrqkglsr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gjhndbbfb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/graitsewl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/ggcvtfxxb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/ghcewiben.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/geabenlts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gagcirxou.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/grdzytrvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdbaxzmpj.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/glwpcjrva.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/grlawgbjm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gtqsyydoc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gwlhyixlm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/glrvazxil.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gjxsgbcwo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gsznspuec.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gbqbqxbzi.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gbbcviylx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gcukvptlm.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gftefetvn.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gvakzspdb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gytoakbwj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/ggkrvhqks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gjgjjmtfm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gmcpqllvz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwxewtevp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gwbewevlz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/grlfnsvgj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gzxwzchic.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gxhvvbqgt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gjlsiftni.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gimgyyjri.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gmkhmonnc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/giswkqzvv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/guopurqli.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gpdeakewn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gvhoialmp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gtvmxhyzd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghwbyfgnu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gzknjbxit.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwpabcigp.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gwthixrlp.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gexdyhpxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/goyousncn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gwxpeczat.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gniasvplg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gwnqdlsyn.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gbjtyikqn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/ghlulnpwr.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gtrvwqxad.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gxnjfsyck.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gdypawybr.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/ghwfruezc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gqluofmxz.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/glfqknwin.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gelilhyhb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gradobobh.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gkoepizrh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gikvoinqi.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gwckzcjwb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gwghmmdjt.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gahqcnipr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gthzwetiw.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gtvadptyx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gsdckfllq.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/giqkhuhfs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gulwbyeeq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gsggcdpai.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gbpfazmrg.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gxawoykhk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gmxomlxhh.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gdqwsgzho.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gtrznzzds.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/grjzpmtoo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gxfzwgaom.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gnnbibujo.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gthjdpexk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbohtspwz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gvpsspwbm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gqdftlshu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/govbapkid.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gyznevhha.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyremjtpo.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gokbjzkox.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gpnrscpcp.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/germmdbfx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gzcqlqjhi.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gincyvmtl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/guyyrjgyh.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/galkoviuu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/giylnxgrr.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gklnegnfp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gecdzruaj.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/grnuexevp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gntlixnjh.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gsjqzaxzi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gpotkxbfy.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/goyprrmkb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/geclurise.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/ggmskilfh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvekidgt.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gymwwmurv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gsgxffvlj.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gkqqmpplu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwfmjyoga.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gkimfmbze.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyxareajr.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/ghngstagw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gutqucezm.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/groneewsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxfprxvqy.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gxslctoll.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gtdycsyzx.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gkyhngncr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/glwzztxep.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gsjsykqlw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gknjlowsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gkwtvexwj.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/guyjrvfgy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/ggriuceuh.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gogamjahk.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gcadxngdr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gwyebdtxc.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gwaxghtqr.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gictezqdp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gidfbndqf.sHtML


<!-- 参考信息 -->