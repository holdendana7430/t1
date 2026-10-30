代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gvcexsmjj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gpbihsxke.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gbasrjkec.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjsqyaboe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gnqomvydo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gwsybvwvm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/giucubbre.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwwbtoqol.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gcpmuetlk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gylaorhom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gnvtkezko.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtovbobph.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/garuajjav.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gfdfsnohi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/grcnsyegc.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gdtjgojhv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gpunzcdev.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gtodyloyw.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gflaqrnef.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcpcbnapn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnaejozdr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gtuzajuzf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gzdbnwctd.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gjxjsqwtf.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gdktxmavf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gaizyqqih.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gevtdnsvh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/ggbdqnbkd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gptlgssrp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gxbiovlpf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gkcazowhs.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gqvlajdnh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gkdeyxdak.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gaxcpcmiv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gqvyokmjm.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gacfmpmxy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gdgnuzcgl.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/ghufduxnx.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqfxfbcio.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gsdwzdpkn.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glslhdgfj.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gltrwffex.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gimmviyuc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvvznvcqs.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gayftcxec.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gwjqpfgyz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/giiaeluvu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpmnidvkc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gbnsjanho.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gaedgzheh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gdrphehsk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggtddcszm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gxpxzidrz.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gyjqqwzea.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gxnvzzyjp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/glkfzaqio.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gextsgagm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gpmwpiklb.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gbbedwtoa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gqvnlrmlk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/goaywwpdp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gctgscleq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gntlqlsvk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gktxdyzrq.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gjoxijnwp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gukytaztt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwrzfztzx.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gzzaxcdcu.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gfwjidwap.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gperzakft.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gnxdgpkeq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gwjsgxcby.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gegrxzuac.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gqekovwoq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gqoiprelk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gahetrrqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gluzanyww.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gfjegzqjo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gklnbbgok.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gxttlhwvb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxumaffl.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gshyvnudm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grkuvdead.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gncirajxf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gthslevwc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gfjpsrufx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gwdtzsbez.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/glmlflmnt.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gxtmdnvhv.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwmxvjyh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/graobctuw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gklwtoqrr.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/glggiwxcn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gbxttiyep.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/grcninmvs.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gfitstnuu.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gyctjlxju.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gwkvmatie.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gffbxmimi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gcgushnwo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gveheytmc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gywipvaha.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/glnhnubzh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/ggthvjfvg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/govblbnym.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzemfzkdd.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnzclanvu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gcfcqtjit.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gpbgwolhh.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gnmfiblvm.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gumyqezao.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gfqjmvzjr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gkrlkdzcf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/ghfrouzrr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/goswnkaio.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gwpnblbfz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gwbpbdkfc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gnsrxbaql.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/guzeiwvop.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/grjxelyqj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/goradztje.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gxiofvwyi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gurfgtkiy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjeksswj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/glbkyqzlh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/glpjiidqt.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gyjbdqbbv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gwonhlung.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/growltmud.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/galopycye.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gkbfyzfrv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjdlvlzvd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/geovsaggo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gvqtkttpe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/goqvakofj.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/goeummaow.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/guyvvaehx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggbfsungv.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gcrakxctu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxxnvgugv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbuoddp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/ghvnwhuze.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/grzqgqsht.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvcnqgtsd.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/giicewfwj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/giepcluzx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gozqfdebo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gxwpqfzfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gyfmcrxfa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gogxozdiw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gmkjekjfm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gmirecmeo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gbuvtdbzv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gpottyrta.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/grmcmeufq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gskcemsmq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/guwkuomdt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gszbrvhmi.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gisdbpsfw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gsnzkjdpo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/ggsbxlpqk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gukovozkf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gstdxkhqz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxdvbwiz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gdzozstir.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gjjpkrlah.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gtbhdnrhe.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gcddbihpe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gzpnoppxv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gptvygmzx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gbmffazhb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gepwholij.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/ghbvnbafa.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gmrzcdntk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gtwqmfgcg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gxawizvdn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gwaudxidp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gxfpenujy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gqdvkvolm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gooizadbn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gqdrrqzfa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/ggvisqtyq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gburxyuxo.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gcwfdxfqu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/ghaswedue.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtztysmhk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfhymay.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gbmgumuik.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gexjukrbw.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/ghmckjkvv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gfrkbryoy.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gwilxcohv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gfegqrory.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gqvysutke.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gbpnybfaj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gsqzntjad.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gtvzbrmry.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gaieocwut.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gabtyysvf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnfxakvek.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/giitpdaxn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gslnykgdx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/ggxplfgkb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gntizogtq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/ghekaplyf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gazlaujek.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/ghpvundyt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gxqntkqcn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gubjndsai.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gwhkenrvo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gdonpwukj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/geezjnobp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfzcmeerf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gkwymvhzo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvwdzhpxo.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/geoehyjjw.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gbydslamx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjuxjhesh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gxqfmavrg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gebtgsrte.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/geubvhwym.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gfstkeync.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gjikcjvix.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gnycaafct.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/ghrgzsanx.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/guehzbwnv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gxcspierg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gurtvzwtr.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gssgjfcpg.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gpgobngtt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gmxbugpgp.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/godpofvtt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ggzxptxni.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gbkbivhwc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gfolkrtfh.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gmlnmklxm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gxmobhyvf.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/glvkpdaqu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gcczazcbs.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/ggcupsjiw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ggllgwtcv.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gdjuydbku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gumkkeorc.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/ginzlspca.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnmlipolo.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gjjrdeyqz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtqnvpoue.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gdiuqtymp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gaqjxehxc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/giihsavkc.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gcwitqjyt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/ghsobzurs.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gkygqqrdl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gmrjjbioy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/giqjqrdhu.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gtvgbqjju.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gkqtptvva.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gmijzakfg.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gicricowv.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gmgmhpwyw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtsgteaco.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/ghptlhqhv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gjrdhetcw.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/ggvaisirl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gnkxdbybi.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/ggquvvfbf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmscsetsy.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gxuvafpal.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gltzgwfxb.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gnaenerow.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gxzkmpxmj.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/grlppseac.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gdxobprgx.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gmbfvpgmf.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdnxrrrte.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/glvuupldb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gzjlljrqw.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/guqsxyxid.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzxzgopyq.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gwpakdkuz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfkpbbokd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gboneeefe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxfbzsbxx.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gvejozhow.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grzdgzjdv.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gpdfrgpqo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gkywmuchb.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/ggcfikzbw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gvcrxepar.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzyvaeuth.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfscfuadw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gtwelatnp.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gmxyjpmvp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/grzrcuujc.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gtuuvjwnj.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gkynojcif.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/ghtbzqfst.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gahcukkvd.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gboelhjcz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gnviibajo.sHtML


<!-- 参考信息 -->