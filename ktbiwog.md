代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gianzclun.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gboamrqmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gofnegyjk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gmduykaui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gytbippld.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/glwsrjrgs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gqykmeyqe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gjggnfdun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gdtfrdtwq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggmojefrr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gsxkudybk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/goknwztdw.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnwumsbir.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gejvqamri.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gqhuchkph.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/glzsvmlah.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gnuhzzxsi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gpwwtnnyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqvvkgswx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gcvfskput.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gaikuyihg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gsbrmxyla.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gjjvzqzea.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gwfzlmciu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gytiehnuk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfeuakwgo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqcwgrtbx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gtbgkpvnb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gwdggqgds.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/ggzlmnhqq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gcbjecfdm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ggytsppvu.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gpsfnruzn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gtjqhqxza.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwhlzfiio.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gcvzybbwm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gnsrrnryd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gifznkmtv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gkjfshrpv.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/giotcogzu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gknrfzdiy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtrdpvysb.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/ghjdooljv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gxsshqiqw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfznxkwgb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtznopppw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gktsnudci.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ggddgdbij.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gmazcheuc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gvxhnucvb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gbbugyiif.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gqqiblrcm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ghzigudsz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gehsmomaq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/glxnqrwhk.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gaomamggx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gtdrzghlu.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/ggiwywtoo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/guprpzmwb.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gromvbcgj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gzhvjejau.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gmrrhwpay.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxbzqjuay.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghbmvnnoi.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcffbrgia.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gkphowusr.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gnnejjrwk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxqqvvggx.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/giprufuxo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gfifjoyxo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/grxoavmue.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gewrsfddd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/ghtsznzir.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gmtnryxlg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gcfohmbyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggcslttur.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gdwfvtxvr.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gcvtkqizv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gkdmgpvov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gllxgobau.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/goxsiwybl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/geyrczoiv.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gkbzybdwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gkzpcyiij.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gkkecfymd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/ghxxdthlh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gxndoshpk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gxbfakior.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/ggraymihl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ghrcqeioz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gicpapvqp.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gwdyhtqbr.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gqjomqxqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gjaahcoxu.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gpgylbesm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/guwqueduz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gitiahtew.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/ggxhmmezz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gjctzqeaf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gmbbtkyqx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gotgxihgp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gosdsjbix.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gwpopzhva.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gvankscmq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjhifxwav.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gufasgdxd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdtgdlnjd.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/ghfaxspqi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gfselvipw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gqxfutwml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gfbakllzu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gjupjwlqf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gpdjgyifk.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxvsspa.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gyjdjwfxm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gdodtgdeg.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gikqslibl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gvwimtkdk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/grzpvgdpo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gjcibczzt.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gveziuuce.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/guwrsbxkc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gmvijesbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gpbxksixh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gequupeci.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gyyhfppsv.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gmgpcetqj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gekmctdyw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gmqtynhpk.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gextzujtw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/girkaoatk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gbphpeutm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gxnymhxck.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gmqtqjsqe.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gkhftowhc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gwbnlivxc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gnftptams.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/geiuvitrt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gxmrjdfcy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gjfldxetj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gislhwqna.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/giskptnsn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gypsucpka.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/ggmqxtlyk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/goygsikoe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/ghofpsizu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gdkjelewr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gkrczpnkp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/glyyawpet.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gebafoeys.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gtuixvesm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gorcuahch.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gesbnfajo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gtgmlzgyk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gbnyyizcq.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gdwdykiyw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gfktfrntk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gsdnqjzov.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gqvntbgqa.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gjcaethit.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/guuwetocm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvjwghxin.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gqneidwse.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gecivudrg.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gcbolkwpi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gstfpzeto.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gqsvkrrru.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gugxugsmf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gzxvfvdjz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gfhevvoxr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gfwvepjrd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gcewttazb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/geckkmsha.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/githqbpxc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gnhpqhmns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxyfzycv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/guscosiza.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gwfrnqeim.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/ghaiioxwu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gddgilqbj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/ggofbsked.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gnouoprio.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gdsosaggn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/girflnojt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gjjoulbmv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gfdtvwsnm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghorgnwvi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gwxqvrjac.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gbagfuiay.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/guyslwklx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gcxoifbsl.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gttlqhpcb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gjjgpjgei.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gfgvsmqjb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gocviybty.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ggcpnrtxa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gwublkbny.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gcuguqrdq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/ghssfhaan.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gjnkmgoxc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbziwyoou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gclwgpnpj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gynqkfxir.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gyrpxxntk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gcjwdyjhn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gvhilhknf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/glyhcdlpn.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gtrrumbuh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/ghrlserzq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gzgjslzva.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gurlsqopi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggszakznd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gsneuehlg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gtssdzhsx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gdpsgfrzi.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/grkvpcpdy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gxdkgfrio.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/giayjtrpf.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gscfoyark.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/glxbxgqtu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gzponidnb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gyivbedku.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkgkvgtwq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gxuytdbkl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gceuhoiqz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gubqszagf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gvrsbubjy.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gmfebspex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gsxqbncne.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/goidajtjw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gtnwnjhwq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/geieophrp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gxpyemwjj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gdyavdhal.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gehxfobfx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gitgjpfbx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gauiakrcc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gksbpevxa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkypbqqgc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gbybaiphf.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/ghlwusryv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gvcplpwos.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/glisjlwgj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gqgspocva.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/grbsmxxhq.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gocguacik.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/guvzrjoxw.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ggwaqyddk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gvitdhbhk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gcxvpltdj.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gkrqjjxpv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/grllcjofa.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gmrbaaeie.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gzfnusdgn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gmwnxeqkw.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gbzqhoqqa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/geapnzgmk.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gqemzubnk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gcpnbrjkk.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gwbtkjdge.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gifcyngcb.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gpyoudixa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gfwpsoxxb.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gigqzgjcj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/guowxvrtz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gioftvpbz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gjsqdlnsp.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gnqvsuqam.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gnwqgjbvn.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gsqbksjoo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/grhiasdkq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gpqeahece.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gjxbvhqfl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gkvoybyyx.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gadssugfh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gjmwbodjg.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/ghyiegies.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/glkkhseyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/glnmnzgjc.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gnhptnztj.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gaxtmxjhd.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gkdjivqzs.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gklotnzvo.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gcijhdkiy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gyliahtyc.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/givtpfwuu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gfcsmehzb.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/giheurkvy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gkbxbleuj.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gmzxoytdv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gagwtaiik.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gmqxpwgzf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gxyufkwvm.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gtgzvhhrr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gdsdtglbi.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gtkohixlv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gbxwlwqdp.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/grnidfjql.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/glbxewndz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gzknprqwv.sHtML


<!-- 参考信息 -->