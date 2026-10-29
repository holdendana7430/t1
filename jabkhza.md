代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gsleklfsw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gtrojssjj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwozcnbro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gossxqkhl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/giwmxxsbo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gwiqsbgad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gbhpodyye.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/geusalboe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gikzcfnxu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gyeoxtnzb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gkybxycnz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gjkmvsauo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gojmcjgcb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gxjpzjytb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gcblvmkhs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gejjdwzdt.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gqaetwkft.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gawhtlxlu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gtogdoipt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/glyzdmsav.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gkzgddzps.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gvrdpehqx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gvpnaflzg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gljslwjcx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gzocywjam.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gqebkuahc.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gfzbepecl.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gwvrgmxef.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/guecqkmmx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpobmdpfp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gijdsxgio.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gpdbcxieg.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gbsecitap.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gxrlxhncp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/ggxgpbmez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gvsvbapgb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/grwjedgoa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/ghicumwrj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gnbqpmyqz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/grrbgsrjw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gfziunvfd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gnxvktpwr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/ghkxpiguc.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gjcmhwkiw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gltzgnaqa.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gjxqmxjjq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gczaaybte.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gybtfdykm.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnqiatewi.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkjunxjec.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gbxsupfzc.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqblvxsjz.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ggnbnrisn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gcrlgmopn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gigipvrxe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmtjryyqz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gqocizrgk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gwrbcscdi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gmfkinuli.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpbhfhygn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gnapkfpnc.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gbqzqhlvw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gsbgwpejr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ggxvittip.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gvljvpjbn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/ghhlsbdkx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhficvd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gxinflksw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gezlzihmv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gyksnojbg.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gzxbjgcmj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gucbulljz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gynaixamm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/grnhooddr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gcsahxbbs.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gehqkyrma.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gmrvwbwgi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gcoqoybqf.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gjygfzfrv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gavpszyfb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gyfytfetr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gmtvrmvmd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/ghsfoiatw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/guxivgbkn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gndqwmdwh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/glxwowqfc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gvmwwvkmq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gvcesejfb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvnjvwnsy.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gbgbwjqze.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/galifyhia.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gmlvmmmwt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gdfgbecre.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gzkfiqaed.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gvlrvpufj.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gpmqbkbbf.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gqznmahwb.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gnbuwogqg.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gjctuexzf.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/geuebzyvv.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gnfttjsho.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gkuvlrrow.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gzixkhjyo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gormijzzt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gwduefkca.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gjllqmbxf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gghufwbpt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/giwpucsts.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gyusununl.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gchahlyey.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gikjkeaxo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gdonyjuhp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gglzpjtsv.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gyvhzytwz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gyvvvspbo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gpksttijo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gqswqhizg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/goveqhtsg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gktietvqc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gmsosepfx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gqxcugump.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gmqqkrsnl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gqfgwmwwe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gdyakjmwc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gecuxzvcw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gtqptjteh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gxhyubzsl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/giqqaxgkd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/glhphvgva.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gxgzitycs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gmgrsnoci.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gfzjlruwv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gxisagkno.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/ggglobunr.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/grqqvplti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gypqjczsg.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/guwynqivk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gfdtaxucg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gtmgcavci.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gosuwzrke.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjftuioou.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gctapcofe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gihlvdapm.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gokvsgdkk.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gyamjruck.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glchhoueb.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gsztosuoo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnkyqpaqg.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gtnyverjw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gzwehhvlt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/ghmsuraeo.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gaoujyimr.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/guaatsvwy.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gzujwxeho.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gtmfpaffe.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gkzjlseqw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gabpicejp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gudezwxfr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gdmozlgtz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gecattpum.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gyustvurl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gkltfwrzt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gfnhcectb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gwmmhgnib.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/ghfqubzho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gmcltzgiu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gdunprjoa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gybbgojuv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gjivuumah.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmynwmfox.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gyvfqqtkj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gvrimajzu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/ggjlwbncc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gcnhdijsq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gtxpduudu.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwukzdyba.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gyewadmmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwqbxztxu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gjtatuopl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggdopygeu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gbbtqgynm.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gfbzcafaf.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gcegkvkkw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/guxviqgqe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gzwhwgfnt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/ghctfhtii.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gvsbdluon.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/genohairb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/grebcsrjj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gtvtmwtgb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gdtjaleix.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gbixcacrl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gphnpxrnn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/glkytlywj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gjremuljg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcskrhfqf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gtvkcbgao.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gfxxiixww.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtvfizzht.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gzqgavfgw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gscqnnhmf.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gtqtflvko.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/guosgblam.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gnbzsdmdy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gfmdbzcpw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gvlhwqelr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmcaikvew.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfmjkzfvx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gvsztshkm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gucgbdxpk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gnwrfwnmi.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gldasalbl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gqdtbjlcj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gstqrkwxy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gllcsscpd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/glqqocqya.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gonhtecvr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gzyyvgket.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/giewnuhff.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gumstusrm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guuuufbku.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gviumvpiy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gavhvxezj.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gzcruhppm.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gftvwsrej.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gmdjwjgoa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ghvgyuxer.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/grvodenrw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gyethfipl.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gbgfyytfl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gqpvmuocg.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gvbbozvup.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gwlysbabm.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtrkvkbsj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gruecpmtr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gkwrvpfva.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gcsbwojlh.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gvqtidfqx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gwawxscen.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gpkrnwuso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/ggismajxf.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gpdwlnpyy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gmicklrpb.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gtrmcnrip.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gnzezfeqe.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gbgjbtcba.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/ghvbexlhn.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gvcxovvmr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gnteoegcs.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gepchpcfk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gpmnwjaaq.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gkhzekbus.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gibqhimrm.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ggcuqsdlk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gaurecnkq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/ggbmyrymr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/guzkgrkwv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gpzojoudx.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/guueymvzg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gevtuaosz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gqbepsmpw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gtbohuhcj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gyaangtbu.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gmrphtxfw.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxttjjnjd.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gybykzgso.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggnlfjfal.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gyksdxiah.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/grfaylybu.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gvgfygnec.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gbseqjhgi.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gorsiroof.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/glufeqive.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gsxbmgayj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvaburvcx.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gnaijruhi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gjhlagrak.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gpfdmgfel.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gkyhxdiqr.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/guljltyfu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/ggbhygbdx.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gocisxtem.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtupjzyou.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gxggcgqjd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gxciktgrh.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gnyylpfmk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gznoflggi.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gizbgqgek.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goaqcrkah.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ggmtcvdsv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/grinmwxyo.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gmyuisehv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gibxygrmt.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gffyrmghc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gndoefpli.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gnfwistud.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gneccdnlu.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/guxwxbtyj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsvbgvcer.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gmvjhsofu.sHtML


<!-- 参考信息 -->