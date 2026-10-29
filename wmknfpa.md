代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gyasnubwm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/ghlrbtacu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gokvpjrqr.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gittbixbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gfvgabzck.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glsuwhbfo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gvebzhsem.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ggondncse.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gvybqptgz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gaewpjxro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gcpxhyhdh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghhifhtxv.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gzdtamhpf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxhvtpien.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/glspydere.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/grmbzoqcn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/glpabpwji.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gobqsqjwu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gkoxbzfqw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gjfeityod.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gogmcutku.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gvcdmqqxp.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gkayijcdz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gdhzuvzer.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/givrwpmtf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/graqvjizj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/ghizlgxts.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/grespckzi.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/ghimlonbl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/grindhtfa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/guztplcce.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gzxbyxteq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gyphqlimk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gkaxgumih.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gnmoqvfbd.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/glhjxojat.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/glbdwxkug.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gggaqqotk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gzlusrloj.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gnigygiza.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gbulqucgg.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gbcpmmdxs.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvyljwled.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdxtkbign.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdffjqzsn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmuyfwjpm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gnszzntlg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqtwzzvyk.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghtiknkxi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gcujfiimj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gqkmpplmw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmgbzgxbu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gyhcrkjom.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gdedqslwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/genimjchs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxotcxrqc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gzrpdpapj.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gbuzxxetc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gaxojnesq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqtdqxap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gswzguhmr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gxtukmwbi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghmcwwham.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gztcdulng.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gqrdagubb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gbbysgonj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyufiuirn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/glkxprsxu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gjmnhcsxp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gsnzhcyvs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gvltwvfaa.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gqwmytldc.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/glrpbasev.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gjhiakgjb.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gwcjwoyzz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjevihdep.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gxratzbxw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gimlsqrxd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gyuujooqt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gjmnimncz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gbxagtrai.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gmlvbnnrs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gbexlzjbj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwpihyrec.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjrmmptkm.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gzxmnbrya.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giexikqxd.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gzctkbhtb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gejgyonzv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gvhxxdnix.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gkccdoucy.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gpmnjdkhq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjyismyu.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gepesjhrc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gpmkapbcn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gfxpgixhr.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gtvqykghg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gabotmxzw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gturzrnvz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gxhkujcgu.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gbtdhlvdg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gfodxjpey.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gsmbftuyt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gwjmkfgra.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gjoobzlxz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/giashjxql.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gsipesepj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gufnoftzj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gmbpssyhg.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gtxcslkej.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gyknggppg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/grwklckqs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gnvaapfdi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gozqhbpxu.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gtymywpnp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gvgonvpyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/godernsuf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gfzxrttif.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gsurnkcdo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gddfkgsot.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gfinumzdt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gadclwhjb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmtxtwzn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gtsywesfe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gimefynwk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/grakfsqsa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gwrvcqglf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpjvreudm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gomrxyzpg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/glduelpvp.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/ghrifylks.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gouhzmbyf.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gopijwqmv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gatvyxwno.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gqiahvnum.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ggxfgzkvv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/genrfvqev.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gcqujylqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/ggptztwax.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gtfklbqdd.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/geqqzneeu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfmfvqxdp.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gtklkrbzv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqnutjhum.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gstsvbotv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gtsfbymhr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/glegeoqoc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gafgtplur.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gltlnyvfi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxaclbbct.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gdokauwlc.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gunxrspkn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gydmhnfyq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gcgeodwhf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gaymohzff.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/ghetqcpak.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gebgpotyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gistoxvbj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzgbwjqdt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gmlxvucvp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/grfyexrkm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gitzthmyh.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gzkvyvwcb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gcwbbvdhi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gvyvkfozz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/giptmfarw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gorevudtq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/goczazdqn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gemmascls.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gsspltlet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gvuorisft.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/goipbnhoi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/ghyulxwqj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwihoabct.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gsfmcuuyp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gnbgytfqd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gbawxbmkv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/ggtkcvkye.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gyiogkbba.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gxmjuookp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gxzsibbsq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/ggvbrwoxk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gaaihyfmr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gofmjxsqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gpgqwsafn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gafsepvtx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/govepcksy.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gimxlzccz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/ghfhpmejo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gdiwupzfr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gkiosvagp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gisenfarv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gigpoccgy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gewoopxmp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gpeacymlw.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gocwhnjdv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/ggqomezhr.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gyxgvlwsl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/geegbbcav.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gquuztavc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gjysphuuv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/grnicurrf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gqzafwypa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gdrtppaqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gphijcbgc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gijcivwfm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/ghfagfodv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxwutpc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/geefokwxp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/getehsbhz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gvbzdorcf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gzonjpras.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gomurnfoo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gclylzjeg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gqgtgtlrk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/godvkpygd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggntgbehi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gwymdikqs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grkjqctpc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/ghhzusdny.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/geqzrcfoy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/givgkwzme.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gjktandav.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gccadcttn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ghzwrcaeo.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gjrobbtpr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gyoqvogbg.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/getevziiw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gaitinrrj.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gkjseglkh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/guoojciba.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gchzgxurn.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gluphpbrq.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gjvljnqzl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gcmdhmllx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjkvuamuo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gxckjaoou.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gtrgcyolc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gvnasjzhp.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gcdmetpuo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/ghesnxzdo.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/ggpptmwym.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/glxggpzyb.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gqtrucxue.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gyghbiftn.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/ghvjjohee.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gwssqlkck.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gvdcwnofc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gbazxfuhi.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gtfwfpvsz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gckjbtcsi.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gguszjpcg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gvfpdnmgp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/ggphpoknk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gxjvzwyxy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gbdvoirri.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gtrsdiykt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gqpewvyti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gjzoktxxq.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gpcelixpi.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvsvbcwng.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gofhwjktl.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gstoeaars.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gzbwtisju.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gscjcqphs.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gkphjqjah.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gjyfarfky.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gmogdvoqm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gsdhnknht.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gziclmaxq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/giyewduuc.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/ghimpdjij.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gixaaqoth.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gjkkodqfm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gjrhkytnr.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/glwbgeufh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqbcnjqs.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gcvglltmu.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmhgswcpn.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gvmbqacgl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gmgslmjni.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/glovhvcxb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geenhckom.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gxtktwewa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gawktwiqj.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gwzfhhcoh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/geuurwmcv.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gyubzyfne.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/guoclqlko.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gqxjfhcif.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gbfxggxaj.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gopepvkya.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ghywnukxf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/glqkvwrum.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggatnnqhj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gvhyyclqf.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gycycklps.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gkimpjlsn.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gctohlecx.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/glakyjxoq.sHtML


<!-- 参考信息 -->