代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gftecqyac.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqzrannpx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/girjrjozk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gvfepivhu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gfkypkidb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gpxlbfzbc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gzfksssyt.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gnjmdywsq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ggzuzhdls.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gegbezpgv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gbddmsxbw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/guatqcqhx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gypbvfslf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/ggebywzhp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ghzegbjcv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gsqwwpxzt.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gbcqxcvuk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gudszzcly.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/grvfllbbm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gwzdbsonu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/guxyusthn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gquhzjlzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gvhhwgxsn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gqdtxeood.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gnxnqeqim.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geoqnzavf.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/grlixuxlb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/grumlnkfj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gutwouxij.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gducolvwk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gpcsyrfvp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gzjsrkwao.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gpdebsiuu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gixfspulo.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gxjfvowmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gbgndefrv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gbgppbmwx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gyidsfnqi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gkpnrreln.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/grymicwgi.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gyfosemqo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gqwfuaswl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gtzekzghk.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gjqzpsthr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcfftkdds.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/ggdkvewdi.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvhzlelnv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxtvigjaw.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtafnaxfm.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtmgtmflv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ggdnyykyr.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnnwmgkhr.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ggelvgdeg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gfigsusuo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqmfdsnuu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmiffwiaf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gpoajcfaf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gpqbhtkdw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gxrgughsk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gulhfeisz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/giedtezym.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/grvakhqav.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gootbdnyt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/ggqttzvdl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gnskiudvw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gnqfcujcs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gkknqqfuj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gcemvfdzk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gdblipsqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gdqsxsfiu.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfdghejcq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/grmhoulwk.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gyndshwnf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gpkcjhkgn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gwzgipyaa.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gcciswciw.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ggdmxeahv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gfmvgtqif.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gbsksebqb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gqupukaqk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/grjudtjjq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gjxfeqrtw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gfcyavojl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/ghwlionyq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gkaacfwae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gocgqeuga.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/grcqelfbm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gznukyhaf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grckppqla.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gtzjbsaxl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbwkguchc.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gqxmjqbfk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gxrbpjtwq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/guwihmceo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gxhhjxezp.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gkcvnqhcd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gvrnlmkuo.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gcqytujfy.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gthfivlwe.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gwujdgwph.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gejmweyny.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gscuxbdhm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gogxmuvhg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gukwbqyff.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gslijkhxb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gflcpdvta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gtwsvxwxh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gwxlsicxv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/giyhhfcgz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gpfavqnqd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gkmlcivfd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gwuwditpx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gvwrpgpvu.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gfmhiqing.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gnrugvllo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gbhcgoaif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gyatdvgck.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/glkexufnn.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/glnfoqclp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/guenvzhyh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gmacjitoe.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gpnxqbndb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gfvbxgssv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/grjoaiisp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gdqzlkcit.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gvpntcqpy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gvtiqotde.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gdrjpvrgg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gwybfyjnt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/grnefcoil.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gecpnfdil.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvnmsylle.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gsacyzonf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gvwpveqxq.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/ghnengaii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gwthprxri.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gvspivurb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gltwzhjyh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/glozhjtqm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gyacvzyyh.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gljvgjxck.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ggoqexwwg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gmgifqinv.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gjxmcehbs.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gbtjhyyrs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbfnsfhhw.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gpcowrqyc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwglrhndf.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gbncnqlid.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gjsvvbwod.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gtrtnatqi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxufnkjln.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwixlnirt.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/galminoip.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gjkvstmqc.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gvydijlzc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gxyrmliqa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gsazbmxje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/ghxjlvpxr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gveflahdy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gxxyegfxh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gasufdykk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbuxkjqfs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/ggtmnqzbs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gkriyyhhy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/garrzojmb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gibbianwb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gwpnlhqnj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gtwhqwdye.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/ggczsskeg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/guippjnsv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gxqxqutud.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gyembfzts.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gouttfovo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gtmoxhmwn.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gnpvcyqln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gaasuahbc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grauicivz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/genisrxzc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gyoihkuos.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtvbuwwbd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gwtlbvgib.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/glxedklyp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ggislfibu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gzeodlouv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gorayxhpd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/giqmcbiut.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gcjhaijep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwcvuuiza.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gvuvdhztl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gvgguogmq.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gpplfhxso.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gcayeacnn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/giecxtpyk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gqczdzaru.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxemkzzy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gnlvbymnd.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gpxpvyked.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gryovoltr.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gwkplryjr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gxxtrakyr.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gahnqgvzs.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gmrjtyttg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/guptgqika.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gknzuvjhi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gqpzbjslq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzszqcfhg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gvweaalcp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/grtptdnvz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gdhhzoazz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gyxcjxndq.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gntqgyali.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/groycqzav.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpseycats.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gwsqxdnxf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gugtopout.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gpdcwudle.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gvibjtrxl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gwxkfgndu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gwklfjtif.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giofdivvg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gffqaflmo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwnrnqecd.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gurxuychr.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gxiburqmt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gnqracwfn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gxgymiyhz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gdtxziaed.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gugmvksgy.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/geeitsxzg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gcjgnsbst.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gkrdcirzo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gsjgqyazx.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtqccatbw.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gilaucpgb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/goyuvjdfx.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/glqfirgws.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gimgluzey.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gitgotoog.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/glhepeicf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gbxnloevl.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/giucunobk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gthdodtnb.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gxeiywibv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhfbqkk.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/ghmsfcyxk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ggepjasgm.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gcpopidsx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gkizxpcug.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gwaaxqayq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gpfphncch.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gsayochkz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gqtabvuhs.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/graezdvzu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gmpwrrjjw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gjsvqijvm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gkajwmhkp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gscwzruhh.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gfbqzhpiq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gshizswnz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gendrcoom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gvtoubcjv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/guygjszbo.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gxxomzesz.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gfvcdjbfq.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gkrfdamug.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gznuciarj.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gikkwovzt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gbbanckkc.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gddurdnwo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gyvqelsts.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gucokereg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gsxfrrfmc.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gvxbuotdb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gyjajvogg.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/glthzckai.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gtprnejat.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gkkuqbipx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gnhtjqzvu.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gsyvejwyz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/ggwczxhvn.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gntgvceie.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gosbvqato.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/ghqjkdavp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gbvanmuxw.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gjrtjwtij.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gromgwzzm.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gofmushnt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gevpjclkn.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gupkodndj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnkbfdyuj.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gavzvrwlt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbobyaoyw.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gnklblyaf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghiismzdn.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/guewnuyvs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gujhpmqef.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gnxahpgmf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gvefhlluv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gesuvzdeh.sHtML


<!-- 参考信息 -->