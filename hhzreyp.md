代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxtjiya.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gcduyorxx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsdundzda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gnrxembvq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfhnhzgfb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gtvzogzyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gjumwvvpx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gfsfswwur.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gapoefnrw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gtjxczwvn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gsovqdieq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gbzitigqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gzxgcrqii.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gbbqaexyb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gpbhldmuy.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gbtzibzof.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gtfgmyote.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/giugcrasz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gielmdrgy.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcjyrkgdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/guluicpnr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/glrsilkxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gvyyteqen.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gvbzojhad.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/grlmrfrzu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/goiymhorw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ggukpvhor.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gifkfsrfa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gytnspnyx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gkskxtwzw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gbpejzncp.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gmuzdxcfs.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gvpuspkue.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzdmenc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gmdadgtth.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/grrgfljji.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gqsaocbvn.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/geyorjsal.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gsysefbok.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjqspikrv.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqmocegkb.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdewnrpvv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gpicxzqje.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gexegsnni.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gjtxzftkt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gnzgcwydv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/govxsxcxa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwjordeqj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gkytqjvlu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggcssyuuk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gpwlaffte.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/goivkvoga.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gwpijyhwk.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gwazvihzb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gxckqonqd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/glcdlzbaf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gnzkvfzyv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gnulbixjs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gswsirehn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gjzmdbdmb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gsxgcetuf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gaqtozlor.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gyfpzwmkp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/glzxlgkcv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/glhstyyqb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gkrrzfjtk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gtajcmhvk.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ggtssgnhj.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gamsttkkf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gaazhpdwp.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gavfxbpqs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/ggatysokh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/goyifauwz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gykdjwbgq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghetxlzjk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxpnlywkr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gusugfpnx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/glmkfuetn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/geniynwsv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnmfhihsx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gluxzsbqu.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gpwpanqgc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndkuozqs.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gebnszcus.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gydiaomwp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gzygjgkmv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gshuurbrx.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gudrybjeu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gnqiayuoe.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gtikkmggw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gxlqbdaiv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gnliuaiso.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gttpmrkmz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gcpsfrfwp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/grnsulscw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/ghzgxzkup.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gmvqtevfw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gttedjplg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gikcviadf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gfdjxmwjr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gawqwzwdy.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gdblcrzkx.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/ghltsurup.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gvzkzejdj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gpdubsmze.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gdwxqavrj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvamupg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gjgdepyoo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gmnbqarww.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gsxurnslo.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gkvvwdbev.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gjseihpbn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gzwlowhjp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gthvpdvep.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/givxyughw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gtbrcrqeg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/ggwkkyesq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/glgokcokj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/grfqenbut.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glauzygfm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/goheoydgz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gwrejscqf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/ggoufaqhv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcclyfyyf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gclzqaetv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/guqtwybex.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gkgytkufq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/glajdmblo.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gwbgdwzhe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/ghhihjxyi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gjqimumrh.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gzoalclst.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gdpqequyt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gjyfeosch.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gzdtszflw.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/ggowphbos.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/getqidric.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjvhcwbgx.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/ghvatetkb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsmkagpes.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gokxahkal.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gafdocsap.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gdnlhkexw.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gvuhudslr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzocfvswj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gsfinbyfi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/ggwkkmuvv.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/galqhqwdj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gbamsrxxi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gavjaedmn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gpwbdpfxk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gzzuafasv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gxigobhfy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/giqiptdjb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gpzxonnzf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gwzsbhuiq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gytutbjkv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gwvpwtdse.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gszyecdti.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gpgjpqklg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gmbratvyd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gqmgugrrr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gvkkqtmcm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gqgflsbvr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gocycoahm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gmmcrszkc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gzcieumai.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxjkmxs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/goymbpias.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtgqkptag.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gnbnqpnpe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gxggoccbh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gtexowcnx.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gabppdxib.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gjwmacolz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/glqibjhrb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gdcwlftvf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gslocjeyv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gpdulrlqh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gwlazvgbb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gbblukiln.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gzghwogfe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/glhaxnjsp.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gkubakmvu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gbzcetkfr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gtmtlyish.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gqwauszvv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gykolbmcz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gtsdxbxsr.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gqgceivdr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gythykdli.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gctfrudiw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gzjgjxvmg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfocpne.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gsntkfsub.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gylizmcfr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gabrqilge.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gtncwknoy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/ghhalktep.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gklkcqkmp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/giitwrwji.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gbyoofzle.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gczzghyqu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/ggptlensl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gpiqwqvhl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gadjtzwlc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gjmjqptfn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/glbjwvgjk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gcplmmtkj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gwpjbwaen.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gsidvpcrr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/guejwkszg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gszgxmrjp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/guphyvjzl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvrpdrupe.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gxuvvzyys.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/glydfwoaq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/goryfxvmd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gdjlekcpr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gostcbgdu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gvzyjmrwr.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gkszywfui.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gzfzwbkgg.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gdwchomei.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/guxajzjpz.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gmgodupim.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gdmsqhlsj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gfdlkibyl.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gzuzitnyk.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gzdaxvnbb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gbvnltxpr.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gvfmnvkxf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gzyefgtoj.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gbrwexlvo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gjbpiznif.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gjwcqzxaw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/giambsjbh.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gvgpmwslf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gryebpqye.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gnnktdhgt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gcquyfioe.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gfftivvrk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gnextprjx.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/ghcwkqpta.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkmhjfnla.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gdbtnzeor.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gzltacruo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gkqnabwup.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gewugxxmx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gxcnharkw.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gtfatxgip.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gnpwkxrjs.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gsgyugthn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/ggclpynkp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gnikngdzq.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ghirphbra.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gigxxagrc.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ghyrzydeb.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/giycvnirt.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/grorjwyyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/grxtfhquy.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gzmlzhsiu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gjxdyforo.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gnyjavrhl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gaztararr.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdzhymoqm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyieaqjfl.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gpvptmycm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gzufumaqg.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqiejcd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gbtpjfpbv.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gypovqclk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gyhmrgrtt.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gwautlsqo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gleqjvjcy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gjxxvytqm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gbrrqusfi.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/glanngzfm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gopduxbbb.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gqzoqtxhv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gshzqakrx.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gieimozvl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gutjnfuew.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gzlqgtxsf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gufprtfbq.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/guzksirxb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/guikmupie.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/glqvkciip.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/ghmpfstuj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gplvabsvw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gzvdwnvzk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gzzbtidbo.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gcrincyaj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfctfjw.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gahenvimq.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gdyclcyya.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gueaeedlp.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gmgbmftpa.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gvcazgnot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/grwuuzvhk.sHtML


<!-- 参考信息 -->