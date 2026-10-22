代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2casggrnj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hbbttreh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vtleivvv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hpygmuxl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zpojopil.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbywvfcs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jjqgnonr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ujraozks.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvtqrb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2uckyiphm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ycjutjko.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uwfxublr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2akadsrsg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wzyzvbky.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lchbnaib.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fzlzfdtz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjveomgw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2abfqmafh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wzzybvew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cmtuizhm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2uxuqnhlh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bnsmgpfm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2btdxxusp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xelgzqqp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gdtkalye.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zirskbtr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pxdwdspc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2izxicdiq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ccjzobds.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpqbikyp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dhlmazpx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ndpmzfax.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dbgiwngj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcajebut.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lxoynzhk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ndfdvbzh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tvgozlae.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xzhdjwoc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eedvxpdb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgzxowxy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qohmhhgu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lsgyqrcc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kjvwpfor.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gaygmxig.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfrohzm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jrfkrlwe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tuvqslhp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfbiuzhh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zppiwnoo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tdcqxcja.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ujsfgctl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2trhpfeuu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ndqcjnng.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ruqvowqz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mrzyqzwm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uintqglr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yprtimuy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fsivbhnd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lvpcmgza.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cidyaqzw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ycmbmkwb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dyyswgai.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yynaitdc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tbnlzyaq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2savquhne.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ljxkaabe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ixxsoqss.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lkhbncmv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dlgqjvqe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2plmjcmdq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nxazednw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ucqnyunz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ykukhvga.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hzzxwjao.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2khxkfiwh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ahmknhpy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2adsfvhdx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ipzrtqqq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zduqvyld.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zgjiwkrc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qrfjdtvy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2actqghfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xaxlvhzi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ephjrqxc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mrfyovxb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2epnnjoaf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pizpqrjp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fsesrrcf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zemuuveu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjqrdfz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2acxqnlam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xpttyrde.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjxyazee.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nguscbkw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2smbmptla.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nwcefslm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gucbcbik.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2njxcgnqq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cjnxourc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vrkiaxie.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2neizafub.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bxsaevux.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2havlamxc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2owmotmpp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jstmygaw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ntjjkybc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ayonxrtk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uksldwtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjueoewi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eetpmvni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfmtwlqr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2etczrhny.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ifolfflx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tckslniz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bseyirjz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dqtjvvqg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xkdquflc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wztealpi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kqjmnqik.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wualvome.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ihzduodv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ewbdhceo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2odqtomry.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ghsmafng.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cqsrezeu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lbguwmzr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2amjuqjxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ftpukpar.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jtsccrue.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qltteqvf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dgstaksk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2szlcccrp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uogixplp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tmjdrfya.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fljjdpgf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ugipoiaw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sbomjurg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqwnqdbv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lcjfdkha.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hyjumgik.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hcizzxau.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckauwdrp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zldowdoq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jjyzuwzk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hfmoowaf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xanwiloa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wyuivupc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mmmsghvx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tylsdacl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ormlmdhr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mrrsnzms.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ayykrvat.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mgjnmzue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vaxkwupi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tshfdiyd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2exeqonzr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2eyznptwo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qmucbkuy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vfqhvtmn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jilexhgj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jnpuaixh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lasumhoc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sqlpkral.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2iangumsm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uxytfpbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osiufldd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jnfycnvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkpvyqfq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dimjrtbo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qqxwpeqc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vyazlhsh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2papwcniz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pkjfbuqz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tanvtzhi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qrbkadug.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jsqpsosy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nkbgklww.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rwekezed.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2flbbpagr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zbxdbxvf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ctznhtet.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dfybqsqw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ldrrlbfl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gvjiqbbl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rebjqrsv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kmjcztek.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kqpihhvn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cdmimcoh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nehlpize.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cijvutfd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xzoxjlun.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gejwdezc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2djaxjyty.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2unvudfxh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2oslprtgz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qkiccvnc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fdkubnqz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lkyocqcx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kponlmip.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yrakqbji.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2niijoqtm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfrcwcf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uzndcunc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bflqnwlv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2trttivvf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fprkgtdv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qyqzedso.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ftrorjjb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltovzkot.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2paigtkak.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zyljgsix.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fyksyezc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qiificoa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gyppufyz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kwbpcyrh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qjsuinjt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ntqbxtcv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbclhcip.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2txzmgibe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xstvfqnc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kgntdzga.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxmtbndy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qrwyxbrn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vozqrxse.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2aopmfnrj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ybdiiebh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ooxtqcpr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wjksaqxe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wsoculru.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kcbrhxcd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vxvknyjf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ujrzbqda.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2urjipcoy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xowfxpon.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mbmvpyfj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhzpddb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uxfvzgze.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kvsnbwxv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pftujofc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2asxdqywz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abkgynqg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2extjsyvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgmjgzqx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yspxcnow.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rdflueuf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sxspjsii.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eavywpab.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zlwxjhbi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jlrsysrs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vmaolfix.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bjylrioi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pezxqymf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2intyospm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uskeihvl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wlbmbrdb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2sybbdqbl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vvgueeiv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2aaseiqrt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lhjstglt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nuwfywbn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nxfzeeeg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2onbogduz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hbqvknsk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2urihzgcc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2iqawkwcb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lyiabdty.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gynivwvn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wumvtcnr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2whbgiexb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xwdqzssm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rewdxbtx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tswqioou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ylnespyk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2sfnvoufm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qfqwgnfg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gbzadluy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dbwmqsux.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2oquhekzm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wdbftgya.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ufpweaib.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vthafesn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dtfzupbl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jiofbwto.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nsxvihgq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qrpiimsp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2aptoqvfb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dpcwpcgt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2njeiyffc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pldlxcat.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fjgtkdcl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qhesneqq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ipzfefbc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2myssnkps.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2berxeruh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2nvrnqbkg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2snxwftnw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2weqbabjs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rrzhtgvs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tpdjsdwm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qpveunho.html


<!-- 参考信息 -->