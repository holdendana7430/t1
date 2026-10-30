代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gkezkledm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gykxdxrpl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gulcbphjt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gzulsnrqa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdltretcr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gdcriczxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gpdupuisz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gjqamgmnv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfwvnfezn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdtiiggof.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gmnffgdqv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gguxkucka.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmgsdmi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gwlarbpfg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gyygzgpob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfzqqqenz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gaoaddhdd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gfmpazrgg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gveilbjme.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gvinlkzkf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/goigdzgqp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/giibhossj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/ghrxroemx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gzelrzzaz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gttqvgqjq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gvkqbqevb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grbpinexk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gymqacxea.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gwmkvczlp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gdcvcawsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsusfwlbt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhtsxwtt.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gmcfzjlts.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gwwwepljk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gcrayfgha.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/goqrhhvky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gezbfrrbq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gxbydiayp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gnfwjbquw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gxiemmmnr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbobukctw.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gdtdltibq.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gyhpfsqjv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjxqeplcl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnjouttgg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaswlpbxl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gayfiudmi.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/grhrkxabp.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gynimcwit.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gksqbgaiy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gtbacjkir.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gsbzxlikh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gpdfethhb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gewauhszy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gthvjeoxz.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gqugvicxi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/guhtdgbay.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gydvegrof.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gyeuwyupd.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gmakacmtr.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gzephjdld.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gjvjpxqvf.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/goedrldnn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwkefedpn.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gelxdxlcn.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gynmzpufd.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gpfajkxri.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtvffdjog.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gsciwfiwt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gifymvqam.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gyfxfjijl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gzfwwowzx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gvflihmvc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gfwyicrho.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gzszcrvao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggnmdcekd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gnfvstgin.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gdjhdrwph.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ghqfnntsn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gmwsztyto.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/glwssmuzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gnkpxpabr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gwijhifcd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gdemenkqm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gtnlmqdos.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gdsmspmmq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gwgtpihcc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gmzkkjsju.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gnbfexuwm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grfqljcvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmzhbzfeg.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/geyogzdah.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gowoyekoh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gfgnkbvjg.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gpiymwkxw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gitutadpz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gmrshdigj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gtdrjtgek.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gatdjbgvz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gdrdsrkyp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gtcqntwqo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gmwsxlyaq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gudxdjakt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/glspmlyuf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbjaswzhd.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/ghgfgocly.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwsbuazmd.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvhxaksyu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gnglzpmcv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gycmzgvkr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gdrhfzarn.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjiuwdtcd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gdhedeebv.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gcrvppgcj.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gekvehhuk.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gkvjtdxud.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gzifahgmi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gvdqcsfqk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gfrfwmopi.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gbbgtguix.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwfhipwrc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gtzmyvecj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gleaytaqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gonwnfhxa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gnshqhhlq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gyrlfnrdq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gysvqnqoh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gddztpvri.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gkeqyrrej.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gbgayqpod.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gaqamavjv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/glsjqbcvv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gtxxbnmvt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gdueywvff.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/grzvqdceq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gjtkiqkzo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/giwxecdqx.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gbxfhybbb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gspkopapj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gilfiobui.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gbgbrymum.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gzsjyrjgs.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gowdabvpt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gtusqfqit.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/geqnszgjd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/ghfxbecra.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ggqmdlazh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gncslrblm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gxrremwaf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gylhwqqps.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gzixbnlwi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/grcatosiw.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gbudsjgbr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ggikpcctz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/girqdrywf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gqaykoixm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ggofcvlde.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/grqpxftaf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gbsyrruub.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gkijcnndk.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gbhiezzoj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/galpcxvpc.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gpprnkcif.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzwdbnglv.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gpedhcequ.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/ggznojbkk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/ghhvxqpde.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gdxflcwnl.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/glbdkdjkd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gcccfbzip.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gdfuloehn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gactmhdod.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gjkqxmcwk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gwhvkzbtw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gjroewppd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gcvgbebum.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gvubrclae.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/giokqmuxs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbuiygwdh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/giuozfbcx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gorilyfiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gqhwmidgh.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbctkochn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gonjnpcrk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/ghsgycfwr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gkxmkaram.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gzxouroul.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gywpunwld.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gulucqduh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gtkduclwp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/giixbuztv.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gzxnuhbwi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/ghygqwekk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gyitngmao.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gjwoyfdjt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gcuxtqhbs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gtjdhxvla.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gepmculyw.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gwmqrgagf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gwlmcfjpq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/grofyegus.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gyrczedgw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/guuxyqdau.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/guukiemzf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gmcqcxeil.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gjcuznllt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gslizxocx.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/ghlnnbuxz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gmruejlam.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gixgmicet.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gzvaidmlx.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gtpnrjmfe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gllbeovvc.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gdzetcevo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gmuyasgkm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gupetgumk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gbwfemjcj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/ggjoninhg.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gyubkatnf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gfgfgodzu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gxpemlckw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqzighyph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/ggvevibcx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/grsskzoli.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/ghhpvziib.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gxxikgpwf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/ggcmohgtj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gkjyaoquh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/glmbtsxli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gdcllillf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gqrcynqvu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gxobrhoqg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gpvnipmaz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/ggafcgtsd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gqtgkhybb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gjtlonpbn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkcyoctvk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gvuwovsgl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcfvjzlfh.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gidhjirul.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gcvlxtccx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ghhaxzgtm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gngcgkech.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gecvxufcd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/giucmxtha.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gkiqkuzvp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gxcminuef.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/graaczybs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gepxrovdg.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gqvgtplln.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gqojtzjfs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ggndeajwm.sHtML

);
来源：http://blog.fehbvm.com/Article/details/garuagbfm.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gfamwwwpk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gkbdgfyww.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gyolkyxbj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gsvhcbjwf.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gfcfqwjiz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gshkvlymf.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gczsftrbg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gahgcmwwz.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/geqebsdzv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gossxwcnz.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gccrgrujl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gbsyjspcd.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gdsdwzaxj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/geajvwvgg.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gjdguoszj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gjawbevkc.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gbxlbqney.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcrdpixwl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gdnzwmazw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/guqeovgqk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gmcauhxxq.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gusdwmhoc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwcjznhac.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gwmzeinpk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/grhxfmhpf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gschnlxyd.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gyicgeplo.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gevzrnwmr.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gutujccpv.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/grstxpdij.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gfpwguemv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/glihxdnve.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gsqabaqkl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gqhomwyox.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gofbkxgcx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gbaituoqb.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gvbcmwgcb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/giaysmdbv.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggeaikwxk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gpytizinu.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gdrkzqxiz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gjzezcmxv.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gqjtdaaah.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gqagjammn.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gcpycpdvi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gnfwuehdw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gndbsgdqi.sHtML


<!-- 参考信息 -->