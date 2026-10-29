代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gbxthiffr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggdkptbpy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtadplztb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gdxqoouxf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfimgqagb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gnlrwedfw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gykevyhlu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gwbjcoltn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcbqbmfud.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmqyywmxo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gnjffmiyk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gebngejji.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gglcindux.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gqkjmcxfm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gfzaketgt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gelnzxvby.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/grpudqpnn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gjjvzhwgg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gwdsbdwfl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/ggywlfcdi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gofjofyri.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gtdkbeyto.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gvscvxixw.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ggodmrhnu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjxhepllt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gmaatwqgb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/goxonfrvu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gphpuwzfa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gwewwevan.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gojoalwku.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpevhnvlu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gqssvpxta.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gwdkohaim.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghzodfctx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/galyfxyoe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/giukstutd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gizecsrae.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/ggjjrscpp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gnvoifwku.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/ggavbetrg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gwdulhrmg.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gdsztkdps.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gkralfngd.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ggkstapxb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfemlxnyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmjtawlmu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gukczcbpl.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/guyakftqu.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gribzjutd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gyxfokqhj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gxpubtmps.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/glpruansy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gkuggoyxl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gypzgbcrf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gejgvamdh.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gzlapydfj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gkcqpkjtd.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/ggtqxsbwk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gkwdhdlur.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gmyucvdpp.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gazmhvfrv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gaheyrmat.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gajxrcvgx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gazpxmjat.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcquujjcf.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gshcukrdk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gclcmaldd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggbpiwllz.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/geaxmztjr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/guzsrvmev.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gydyrvhmg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcydtmrbb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gnaokeilx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gtqstknjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/goufbxquj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gpvytjmex.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/ggmjdcisy.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gfafbcwcj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gagninoxq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gtzzadzrt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/guwcipbus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gemguejcr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ggrchukmz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gmojyjwdr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gtcqtjflr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gfednrrhf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gxswuybgs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gphigjfuj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gnshfqbms.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gfuuwfaxw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gofzobcrd.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvncviifz.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/giqsijudo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gnjzjkayz.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gegakqmtd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gaitpnaye.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gmxyjpble.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gzkqjfvxb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gpggeozqu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gyzpukszm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gkcbltytp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gkuruirdd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gcxcfjbhk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gqutzzwiw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfyrudrb.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gzwsxfaoy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwsssajdt.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gvhrtjolv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gwwsywrdz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/guqsyabty.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gmisbrubs.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gnkiilkiv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gxcooyndu.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gnrdijohj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gcdtprjry.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gzkuwduqk.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gloufelsl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gxahmguvj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gahwbhtxi.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gyvxzocwf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gyjplxgzr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gkhvqnkje.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gaiglflli.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gzqrjirsz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gaaeteden.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gnisipdca.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gcoenpyvv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gfvlaeysq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gkvdmaeju.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/grwsixewy.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gabfypfjf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gvunbfmgf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gibouthtz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gpgoenmat.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gormekbqm.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gcqsgedvv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/ggltovlxv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gaazofefb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/ggqxfwnko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gzrydbyqh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/ghgngdxyf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gwiqgiven.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gcnvbavqv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/grhsbyknn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gagqfzpxc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gcohxztwf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gaecyrcid.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvjdzkjtm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gvtqmgbdl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gvbsmjhha.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gmxbdewnj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gmjztnozm.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gidfcdvnd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gcwdmtaup.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gpkzosqvr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gykzkdiax.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ghaosyrnd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/ghcfopkrq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/geeszgofu.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/glrwozwim.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gjbbczsod.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbofxlpya.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/giwcdkpje.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkrtugnnq.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gdmmlstnv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gqnqzplsg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gwqwjniod.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gytbeerll.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gxyjnjsvm.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/ghwbytssy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gizidgxjz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gnbsbveap.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gheyalbdq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gvnuhnbnc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gdlcbfgvj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gfvhxixsx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrtfesh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gqdspjbjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gutzuslao.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gibjihdil.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gojgishxk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ggsflxvcs.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gnjpozoju.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gatbxwirf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gjsxyrrfo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/glbawyykw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/grnmrmzvx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gwmhtpjvj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gglsdzwdg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/ggrwgmdzr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gphmfcbux.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gfbklchus.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/glcpgmxdd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/grwasfkdm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gohfsrwma.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ghdmlczta.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gikwgkkjr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gbsofnnfm.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gkkobcuuk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ggdvwqvfb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/givfkxfpa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gtiarvptx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gkygkeueg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gqdqlvepj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gbzybadqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gdshwhynm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/ggxondnsp.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gghzacmdw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gcbijoedv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gkjsctogn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gvdxhgvni.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gpbgtrmdl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gwwpcugic.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gktnsdapy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gywmqvaex.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/guqzstqqo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gsbvvtwda.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gfykhvcak.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gytiisbzj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/geewqmgiv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/glblmwjdv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gctogouht.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmkroaeyd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gokeqnixw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gtllllusa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gfbkwbdev.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gmfvkhven.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/grcxxasap.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gojcowgkz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gfuvgjjpz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/ghpnakmzt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gyepxyzpd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gvkqrewce.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gyqozjgco.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/greykqmxi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/govhimcxa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gswlajvbx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gdfoebbfr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzkaetfhf.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gqbzgcssw.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/goopxrfae.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/ghvmhjvdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghpifpmtm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gdkokomhx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ggutxaglf.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/guhislcqz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gmgnyquvx.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gjzfxiota.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gbrbzpfxe.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/grdmitino.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gktldsgwm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gvjlbrskt.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gliidejjc.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gzztwcyys.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gxikqxvld.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gcqnoquoz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gzcprgrnh.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gocsevdaw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gsiqfktov.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gmvpjpvvf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gqcenoegz.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gsussxoqd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gwmonvcra.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gxnfdzxai.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gihexijor.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gaaenlebg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gdmvklntq.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gqgjaczlg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gtqbscjqw.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/guipticcn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/goeyljsgs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gyaplvykt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gngyjzmam.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gzorjtfwq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gqsdjyapg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gtqvgauyt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gekupcpsz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/geenwntak.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/ghtukfejy.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gzihhedcw.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggfkaipmr.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gssqbzgdl.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gozmkpisu.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gbtyeeapq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/guzqxzaxl.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/grudsjxyw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gcitvcrrj.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gnslpsvke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/ghsviyids.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gztimtdws.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gvdnxdepc.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gadyvgkqk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gylexhqoi.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gvoanwiiq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gauvdixym.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gjcgcrxmr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gmkwsnkmg.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/grupjmpfu.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gcxrifdaw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/ggmmkredz.sHtML


<!-- 参考信息 -->