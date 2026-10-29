代发 wailian999

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gbxxhfyuu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gbopsxlex.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gmoduochg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gkuunauvj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gceascstf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvtzdueic.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gbdnfllfn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdctpgzsm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/goxjgfrub.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqowbiall.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gijwjxzui.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/goryelmgp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gierjsihg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gotrftdnn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gqlkqvzff.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gygqisnjy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gyjlwbchn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gdlzukstg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/goohqnkan.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gktoejlxh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gpfvlwwaf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxrdywtti.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gvpbgaljp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gdcubyxwc.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gqaobxnwo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gelpniugt.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/ggoizrire.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gjndlcpne.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gsvommcco.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/grllbjhrr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gbvsxxcxa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/goxelxoxl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gsfnmvymg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gkxjxrmtb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/grtaoorkh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gelcxbyzj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gnsexkwof.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gacvrjlkj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gtexwbdxb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkzkdkqjl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gxijhdugl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gelgiehwd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvfbikudd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gbjzvhino.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gjwzalqhf.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqusnfdfz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gnwbsnzvn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ggqhufhhk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gcutiqgmm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gosutusfv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gbbcisbpm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/grfpizvrx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/ggearwkth.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gpoywmcgs.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gsihebljz.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ghwnohuvx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbvslwdvs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxbrirkuw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gsehbdhau.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gpvqwrjyi.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gerujopzl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/glbpkvrtn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gcjgiuxbw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gmgmuuton.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ghhsrhsqa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/ghbmwahmq.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gingdmhgl.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gbnkqgsmv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gnteqmzyp.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gokhlhwhg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gbbekctkc.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gixuubpew.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/giqggtxaf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gxtyoouzu.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghuvmbyhg.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzaoznicg.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gytzbhevq.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gulwhpgnf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gumezldsl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/groifpzrq.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gdynepmrv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gfafiamrs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gabbejaus.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gypryxqvk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/ghykkmggw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gwgizmvzl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gxykhpjyn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbzsszqot.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gjuafmasa.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/grxvwcurx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gwzjqtyxm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/ggdcblimv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/geeietqdq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gcypgfmrj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gtjyrusrl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/ghfsyebdk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gxjdojumv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gqkkcfjuw.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gfvwtibiv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gkqgawpbl.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gaowrflwg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gyenfqdyf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gcdenxxuu.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gaehdclyw.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/grnylphml.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gjslhvdka.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbrcoyqde.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gbjzrvuzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gztdnwxcs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/guhpanauh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gufjoxmta.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gomugcruv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkwazmioc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gwfauxsnh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gykcboclc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/goetzhtez.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gotgvpxxg.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gpayaspwx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghyepfdsh.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gtfgbjpgz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gdpvkjust.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gredxebxv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gseznfors.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gtxtpqblb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gopzfggyq.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gwdmgavzm.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gbmxokulk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/ggsahizwu.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gbwnrzuhw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gvfqepalr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/grfpgmnau.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/guhytefzk.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gidqdsdmd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gvieqiioy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gckvjrays.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gzwlaijsh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gzxfqrtsu.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/grqvwgdgo.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gxtgifmzs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gzqfypgaq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gmwbchken.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gxucqoslq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gnlycdcdd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/ghmkcyrqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gtblxmlis.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gmwtrokwf.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gtevnlzyt.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gasjfezco.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gpthhqyqi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gcywqfnca.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gmbejedqh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkrplie.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gyvxpfeyu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gmgwyeeiw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gkpdusizs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gztpxazwk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/geewquvbd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gwhykiuld.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gugpgipai.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gnpvysmgu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gvhvdvfzp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gznlkwelb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gmuhxzrww.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gpyvpjelg.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gxfweobdr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/govvwpxrg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/grdgkkwjz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gendaxoqp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjoqdiegq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gmrqmoimx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gyepgqirm.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gtcymtswq.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/ganczwgqs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhcxlqrw.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/guryobsai.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggagcazlj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gauhtmwxl.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gljwanavv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gwhnpukim.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gnglcdoml.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gujjhwykb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/govnhrhge.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gttqebsnk.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/givyyuoue.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gspiijelq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gdfijiufl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gavqmjbcv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/ggyywccgd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/goxcddwcy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gfxsbdiga.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwfessgj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gyskzuxmx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gkmdwrpao.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gjuobvrhf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gbunphqxp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/ggpsahtpn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/grfpwvtwe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/giqjvrrzu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gopcbcbpg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gnqbhnmpq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ghnovsiks.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gdeyudeqr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gucaashou.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gzpujirca.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gjwnrmfgz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glxzwnhpf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gnceuzvtf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ghcrcdmwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gqepfeslf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gmxulhipp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gjxyfpmhz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gcwmrqsob.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gmxifevln.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/glxulmjsh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gbxrrpqyj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gadnrzrpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gumgsznph.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/guhfixeyv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxdezudkf.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gdxwvzoko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gzpvzbize.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gclahntyo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gkorxgewx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdearwnvg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gcjacrvso.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gwtavqyhn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gcruqcguf.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gsrdyzrpy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gdbhudssi.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gxkkhkfyg.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gjmguqpgg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/grffsenzs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gspdtwrob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnnnagxqd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/geteztfbl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gzvhzkzmk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gcczgtuzm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gotzefjhx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/goabryams.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gjyzwoxor.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gtrldktek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gssqkupew.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gyutusdpj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gxqqmrxup.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gkjwqnuaf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfhcbzfpf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gpuladqpw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/ghtypojgz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpdylhpqa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gagzgpcpv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggrpnofyw.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/ggcqgcevf.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gxdxslhfp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gqlavwrfy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmwrarcti.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gwxwztwwk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gtedgcpxl.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gttbluwwq.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gdqgqbtzv.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gtzkxehrn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gomnnsilz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gxatgnxxs.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gjawclxym.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gxcflweqk.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gnfpbcssc.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/goxrimuub.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gwhxjtxzz.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ggwneordy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/giuztemjb.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gxtnajhdd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gnntulanu.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gptxxjxqs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gwhzftyhw.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gdmevcwpj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/giqzoutcv.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gvpedkcol.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gjgoztgzt.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gdrhfzayr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gzzlpedpl.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/grtyqvaou.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gwtnwrrhy.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gaeoyygqx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gsckfjuvs.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gaswnuwry.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/geommvwsr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gpqkglccn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gwcgrbqyw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gvsfzmuon.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gtpkyhrqq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gvmefrzsc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gmotxalkj.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gpwjwlidy.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/girunuoix.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/glhdtmflu.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gboptyzlh.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gggshsfoh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzojoouip.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gceybvdlu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gsfezxpik.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gyvkzygbm.sHtML


<!-- 参考信息 -->