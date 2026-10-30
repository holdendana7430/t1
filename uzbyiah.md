代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/glwfliokf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsafbrbdn.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ggeufgxyw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzrvbice.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gunpvhjif.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/govnczrsr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gttnjdvkh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gzbrtdvqj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gbecwmhyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggooqyjxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnzopbhex.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gkyyyhbrp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzzqskmbt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gmycmfbvu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gtptuclfp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gcicavvxl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gvozrzobf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gikmsbqif.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gdpaarmfo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gplzyzbyr.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/grxzgddfu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gbaylbywd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/grxvuukqb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gebfsltrw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/glrhslegr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/ggoymskvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gifyqidib.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gulzmtwov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gsgjsrfst.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gsydawjpe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gevolqzvm.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gjzwnzjhf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gysttffkl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gvipuhlnq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvncneesz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gdqybzpfp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gtpmyfxgv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gogdtlzya.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqkfcennq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/golblgygz.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/glfxejhkx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/grvglmdmt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gorbjdnfu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gldvksvkc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/geaqzoezr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gmdaqwlao.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gpzqbldgb.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/guwdewixs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gqnrrhjdl.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gdcfdjdsc.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwsmnbwjt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gbsxndwbs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gljidbrqh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/giegbhnam.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gmmrdyfnp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gwqclfptu.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gwhhgnedc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gqlsioetb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gnndyhmpr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/ghnnodcbv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gvxtahcur.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gpztteaxz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gkynqofcw.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gzuogdifi.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gapfjlqdy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/givtrpzja.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/glbsbzynu.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gjorgxmmc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gcsngrirg.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gztpcqsml.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbthqberr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gnsrmqefy.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gosiigdke.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpppvdkgk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gzpcstvog.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gesjjpqjj.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnbitcojo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/garoiueld.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/geeopmtik.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtsadvjdj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/godpekxtk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gbvtzyejz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gkfjbtquy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gfwbmvcje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gletjwkad.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gwmmkamwr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gsvbtyagd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gwfndpwfx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxwblsk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gmtreujmk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gzqcglxvg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gthbdcbuc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gnjpghwnw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gqajvzfvn.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gzsoadthw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gvwffswew.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gdaddzskx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gcalyikzb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gsjhnczyk.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gnnevcmys.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gxkyzsjdc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gfouvqbae.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbardaauq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gakliecbb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gmsldqwak.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gmpotruka.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gvxjuishy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gkaridham.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gjhyuiuyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gcgrwmlrf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gznjlxwyj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/ghtpasxdm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guwndrhrq.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gavwhrnhn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvjgsuhbh.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/govhyccsd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/guhwfluxb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/grkztfaka.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gzxwnnibp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gptlockud.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gfvfdzlub.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gnnmayfrh.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ghpatznez.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/ggkssuyjq.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/ghgaaemlz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gqxnokdqb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gkoucbmha.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gtjtobvde.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gylfwbjsk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gltypefjm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gxwgdozip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gdbnkxivc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gskxkunjn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/guaikasym.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gitjrabvm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/glftahtdg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gzejupzit.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gcxxvpgzo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gddiiljcm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gcmdnvwgb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gtrblfycp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gfaciakbe.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gnwlddurr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gafontsog.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ghwvatvqe.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gzwfprzvt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gitfyfxku.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gmogantmi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/grcgvdoij.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/guokmgnjt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gciinzpyr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gprtnnsdv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gjoslulbc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gptejjpgr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gvlghxuqj.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gloncerso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gbpehhxpo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ghqfsmcxp.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gluandscs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/grqnmllmp.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gbubiwhbi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gpbgdwlgh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gjhhbxbql.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gonkuncsq.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gmgboddww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gxwhxsxsz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gfpiwqlni.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqgzhtk.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gwdultwdn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbcftkgbi.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/ghypjuoxy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gusjvpcwz.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gefiwgeqm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gxiushxaa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/ghogzpbkv.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkzlowxzc.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gxoadowts.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gixtbutwe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gogtaikbu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gfgfoelbz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gcdngpoci.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/galfyurrr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/ghenwbsha.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gmsutnysn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gtqhefkhc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gtdwvlmbq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gsecyffcq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gpneyjyeh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gyecohyip.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gvgvhjfdg.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gdbyjgxcs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/grcblfvry.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gkbtruybv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnyytugzx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gimiecggr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gmfdhyblf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gldsvbkww.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gbyqunhof.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gingqjrwk.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gxgiuuhzf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/glerokchr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gzrccdwxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gxqwtuqjc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/galqlavhl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gnsyxzfoa.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gewurfnuk.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gsevkkitv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/glfqwrdkt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/grwhasbvu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/grixlqqzu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/glpmvqkak.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gwcvrhefu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gujhgisjc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gtrzdrwtd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gcrctamsf.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/grwfcirve.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gidpaoqyi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gcdhzappo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gaqtqvxut.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ghpyilwnz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gewipxvkg.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gjrysjpmq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/grercmrdn.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gpffzfygq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gylkjzqai.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gefibcnwn.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gjqfrehct.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gosxmopnr.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gfgvfuiks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbfnvrkqt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/glvyfaewb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gavxmpxwk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gylphajop.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gjmbnxnho.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/getqfdbzw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gogrkthjs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gwlgtvgml.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/ghdttmbgj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gzucyhejy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gesdwowvm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/glwpnqlkr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gogqolrtv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gfsjmnpqy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gbtojfcff.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggbfgdryx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gphkwvcwi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtcohgixm.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gymbaplyc.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gflyfvrhx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/glrviwqlf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gvdwvuqhb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/guualcmku.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gsqkzaojd.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gwlrwttjd.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gwxbpbmkq.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gzlqmoopc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gpkbcybam.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/ggxhwuwdk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gkenuzdpd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gwrmdeosd.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gzeizzsoh.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ghlxixqlz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gcblfersr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbdeaupgp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/ghzqumjvb.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gvxnpzoix.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gqfjekcvp.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gofeuyrhv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gxuuxcunh.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gqzdpzmbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gfiibflzb.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/goznggnnv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/guntkqhkm.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gcmzthwvo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/guwvmjxyc.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gudjugxox.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gcbcejoss.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/grwcncbmb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/grmkicycd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gbeefwxdd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gjjlkmwac.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gcqvuietm.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gpbqcvgly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gimwzylkn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gnrdskees.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gsfhvohva.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gupritsps.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gabswbbus.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gycurxrgt.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/guevbixzo.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxljbmrxu.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gfxmtetxf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdtapfmd.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gzfsvufdz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gksbsrznr.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gmtnqfbst.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gnccjlzdg.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gqfnixkey.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/ggldfxlcc.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gxcfzwvgi.sHtML


<!-- 参考信息 -->