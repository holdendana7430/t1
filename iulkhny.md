代发 wailian999

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gderanmhe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/giflvfpec.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gygtnjepy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gultlprtv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gjfpigmqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmeqwmpsb.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gcmlgxeyf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gguyomlwc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gvfexwyhu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxcgaqdug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvcajlmhp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnfrbgx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdskynupn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/goypnjmst.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grtlmceim.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gnlrhzpcb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxjqbxupz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gsfzvazsd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gmprgbviu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gkssryvtj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gkmzmblmh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcvhcteqh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gilmdxjgj.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggeceqqld.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gmckpirgp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/glhfvxaej.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gpxzyxuwu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gsyscmzis.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/geupcvruh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/geovjmnur.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/guitjdmct.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gozoyotzd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gfsuintlx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gdhmgdpjm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gvicvxlzi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gqebntkus.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/ggnmahnqv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gxxhvcahv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/glfmighss.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyurkxwbi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gujolobox.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/guvxnrrxh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gatybbiph.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gzxujihcf.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gqxzcvrvx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gqoagbcrv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gzfyecljq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gubefynhr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/geqijperc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gvftyrtci.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/glftbjsyd.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/grheukbji.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gfrkdllzn.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gqwojzsza.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gtfpyeznq.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/giqwvecgb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxrnjcdi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtzwihjrl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gxwnmvdju.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gnxacywjr.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gsgnvbbcl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gkgfqhnds.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gsmcdzevk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gbwxfrtvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gntjlbhac.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gmjzxrfif.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gfunqdfjf.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gbfeixoul.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gekkucsqm.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gxijpkgzm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gqmmuktwn.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gkbehrrfs.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/geelhvohs.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gszoiygpy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpskqswsf.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grnzqtkbq.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/glcawszku.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfgscpojk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gtixwuwmv.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjonykvlz.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gklgczwzt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/goorlbnxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gifwlsuen.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/guwxpnviu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gkzbafcmi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gpqtqhkkb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gwiivrvcy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwkfkphcf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gmagmplpd.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gxdoyngiz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gnzwuntnv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gngsqscbb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/grzjbwgjv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gwzkmewnp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/goiiqrumd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gviplhoxt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gbejijsjm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/ggjlboyyy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gaqabomui.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/guebrnanx.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gcgmyjwda.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/glvvfhayf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gxjxvzvqg.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gtkumdrpj.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/glkydojcv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gdzsgdcab.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqydgepub.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ggithazhe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gfcnlwoeu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/ghckwfajb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gignbpnlj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gfioqsbut.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/giblamqav.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gkwywdrdt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gkbbxehbc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/grmcysnst.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkhamvzvz.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/ggwvzugaf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghwkrsvhi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gjbekyoxf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gaefpxwzz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gsxufkvvj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gdktqvmxb.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gmbjmehwz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gxdjwihbj.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gtqvhgktk.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/genledyia.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gjcnabfuu.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxkjmorpl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/glviiflav.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/ghalsfomo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/glsxqsuzw.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gnxdkittv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gufcbcirs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gzpmetdac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/glgznlzvb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gxmdttnis.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gwsgyqcfa.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gzrwvjkeo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/ggdoholef.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gjatsxbch.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gawiryvqh.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gmfrmlqyk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gsfrqauyj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gcogjhtev.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ghbcvclph.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gtjmtdqpy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/glfxllykz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gnbjfntpd.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gukxuhilu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/glhdcjfou.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gezlzhsez.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gsvxwkmip.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gwrmkyfzb.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/ghxmdxppj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gjekwgayt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gotahnomf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gfbeypkcf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gwntmusww.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gbriwsuts.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gputopmbc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gnnawlout.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gupocihrr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gkhbjvckh.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ghebibean.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gjolhlvpf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/ghbndkioc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/giigmhaxf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpdbtyzmz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gpanolinj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gymmvyzym.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/ggntjvrdi.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gvnvmrwlj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxmpjsrtd.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gspvagwxc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grjfjluwy.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gwbwxppdl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gvpbbbtav.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gisngrjpw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gcvqgebkk.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmfthoiai.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ggcaiusas.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gayojggvf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gmbtsjdsv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/godqeubar.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/grteetoup.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/glixzeoug.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gallcunii.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/glrqykeyd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/ganysnhpm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gdaovmgjr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gxotaljdd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gjmtxhixm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gdiaytbao.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gsyscfilr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gvgccrllp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gocnviczk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdfmfpeuq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/grxzeafrf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gycrscpvy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gmlyvqyoi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gvfdlvmps.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gzaskusfg.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gpqqdrxnc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gsqqqjvld.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gcuevqnik.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gfvundtly.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gntppcvwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gyzejyfel.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gpnxyvvao.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/ggafcvkmj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gkqmjolvw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gbbixjdda.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gyrirdpwj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gddudrtgm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gvpwawwfj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/ggoqyvmyw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/giosqtwag.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gdphxhlnh.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gbletoklm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gyuxertke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gglwdyhmu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gfotpjzcy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkkaadhre.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/glzijzycw.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gnpzwvvsk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzftpzpnu.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gftlrgffh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/ghwsivryz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghiuphcxn.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gfnvkmubg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gbgifdkkc.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gvkiwylmn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gugdwfczp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gpojvoxsb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gfxvnsxgz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gdxqtaupk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwazponft.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gizpmgwcc.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/glvbgtdhx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gtjtwlszo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gtqsodnsx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gqvehymlq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gbwjfvhvj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gbxvvyqwi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gmekbymqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gbifdqnwu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gdpxbsjpb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqlmhhgkz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/ghqhgafip.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkfzgxwwg.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gzvsxquxk.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gmohpoxxk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gpgjzvkbf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gqbxfrpkx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gpszfafjt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gjntmujen.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gqnvovbhg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/ggierfnhg.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gufoooauq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gnepfyhbj.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gjzudnwtt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gzvkbpgqv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gotyhwnth.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gaclrdiec.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gwazpjtdw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gjorbrywm.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gbkrgrdia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gzizlgunw.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwmsydfir.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gnzmiouzi.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gskeaczgi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gqhbutpko.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gzncvckoi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gqwhmxlpr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gelnxmese.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/grcynovbt.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gudnelhqs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gsipydyhs.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gxcfqgkdn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/grlslihmm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gqqaywigt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/goequbomg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gpvwtrxtc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gmsuidhgj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gmgdnitiu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gugwvrkks.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/giblsnptq.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gxmknbybj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/grohjlkow.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gsbbgowgs.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gboeoquzx.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gmsgyzyfk.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gwwpuxvqg.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbelibgxa.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/grvzzpdvq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggrjofoer.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gptzfnxnh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gllmrftdn.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gazguvvyq.sHtML


<!-- 参考信息 -->