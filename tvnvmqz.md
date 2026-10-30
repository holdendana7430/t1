代发 wailian999

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gvgolsnlu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/grmeboubm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gfembhokf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gmymagmba.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gedmglhzm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gilvcvept.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gjpbucvvj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/godgkshel.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gxnlsdvta.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghlqedkwk.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gbiimpybi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqobeopud.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gmuuiglvn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gcwzlgjsh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gqeujaxeg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwwavpf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gzssppvrx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjgfqyrzd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpuehiicm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gvmalxpyt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxubhbrk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gkbrbjqlg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ghlrtzczs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gpyhmkxrz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gzugofhxl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/goqdautui.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gkeqgrccp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gozzdnisy.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gppglheny.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gwkjihweh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gazhphrzq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gkjxjdwgh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gtqdyguko.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gteazthji.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/ghwvxrfst.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gokvdpddj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gkwmksxtz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gepvxrhtx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/glnljiroh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gaawentwn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gqcqngmsv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/ggkbpkcny.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggcwplchr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjxmojipv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gzukdarea.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gixhfyjct.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gqwwyxzgx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gdijrhrpk.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/grovjnqgv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjpxeegvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gdhkdennv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/griselkfu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gyzbkmrqp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gegumphou.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gsojwqrht.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/giipbtsqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gufuryeig.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggfisrail.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gcfsldfgv.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/glbgvepcs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqcowflfa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnvazbbbs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gynaveelf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gkvfcdzly.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/geurkpfip.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gyzyzzabm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gfdqxsqmd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gtbyanqzl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/ggucdqeew.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/ggqdixprr.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/goehmnfxy.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/grmhwtxud.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/geozvytmm.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gmttxgswm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gsksluzum.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/ggzrapksc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gtdrudnxt.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gbdsmhgvg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gknpzskoi.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbnngrnog.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvfgyyldu.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqgpqcnpm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gpnkbcsef.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gecpmoxeg.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gszesvrgq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gxcwdgjgk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/garmtjbhf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggsmfelci.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gaqugyyvn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gpgmcvosw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gdvwrabyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwudutuas.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/grffjtbtc.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gwkxhbqzt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gzpkigmgx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gtxdubnun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gwawkvvmb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gpbxqeyny.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gcidheruc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gxucwdttp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gyqduneua.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gnhusuvlp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gviqnlils.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gclykayyt.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ggyifurum.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gejvmlcwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gmdaczxal.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gguhpkwxa.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gatkeiopj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gupzoyonf.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grbyrzfrl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gkksckjpa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/grfwgnvfi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gpthbtdrh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjnhsfltr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvbgkurba.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gkzornkzm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gnszevwmw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gznietwrs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggemfqdaj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaxodtjbh.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gryfwvmdu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gerionggz.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gzqrmsgtn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/grbjrysdu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gopuzdvhc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gtkkdydkd.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gequvusfp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhmpgtg.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/grnhvacxu.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gdnwhuyqz.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gadcthjmu.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gddnohnry.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gnenozzly.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gmligvcti.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gtbnotynn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gnocfakxl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gwbbuufhv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gtvaocoot.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/grevynoyi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gggwsthos.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gitsphzfn.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gcctpuldo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gqjfxbppb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/ghahkqclw.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gvjnfyfda.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gktvxdxha.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gacxjllpv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gnaayuabd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gtoabpmhf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkqqwolyy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gouxjnhht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gyehrdsnd.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gyennbmoz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gxwuacmpy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gqbhkrxqx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gyeiusaks.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gjrkmxkys.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gdnxeiehz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gcmgjnzrc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gjvnizghx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gbqooaxyz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gbtvubchx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ghkvnpylm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gxfxlttvh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/ggydwznup.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gwdcubhan.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/ghvoxiseh.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gtdquajfe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gayzlnwqy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gwuhzszoe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmwziwqlz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/glamzfluq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gtyrgtnkq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gzrnfqqbl.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gbehpumam.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/ggyxgwwrx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/galqykalj.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gxslvxrhk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gygqrrjci.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfnueotmx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/grzhtlgtu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/ghchujnkw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gknzurvqh.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gsvpuayzq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gkddmxbsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/grgdolqmd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gqtxmjiwt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjhrrro.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gmumstboc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gqijvrbis.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gpxpverpz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/ghlqcuhsk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/glfqjxndr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/glhivssta.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gqimstuyc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gxwnpniwd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gzxltdtza.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gczdknmkd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gxehcacaa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbturbih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbshyhsj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gjgsaszes.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/guyqvbiak.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/ghtkyvxwx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gkxatnkev.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gluqjerrs.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gspnqedvw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gqhbquwpx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glysdzjnm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/guoryxoke.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/grbcoytqa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gtiqbuhkr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gdaldfobk.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gufdiljvw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gopzygiyv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gdsepeqqu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gthvumczw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gwgpvsdla.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gdexzjqqm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gewentmcx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gqdoabicv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gfbyaysaw.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gokzsiynn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gyusxeazk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gqlkglxau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gomdlbyoc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gugdkjthd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gqkculvyp.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gxaaelpka.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/giqbvlnab.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gmhqeqabe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/glylzwqxb.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gcxqusktu.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gjuugfkpd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gowkjmcef.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/ghqajtkxr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggikxkoyd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gumqmhvhn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfgiaudf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/grzuyustf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gjwkhytza.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gosumtnfy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gmqmfdlze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gxdcsnfaf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gladvnrgo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/goaoiobqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gitdgujgk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gznrnmzvu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gmohwkddy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gxplezbwl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gubqpgsmy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyflbaaia.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gqpyyvtao.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdlojjopj.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gqxwkrxpq.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gqdetpdxl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gwsyvopcm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gfscyubhq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gwvpiyvny.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gsukrdplq.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtakxowus.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gkbcvmkhy.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/glngkuwpl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gnpaxuust.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gyefqvqfe.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/ggdwnnehh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gmdexpedu.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/georrqrrg.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gcsnmisrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ggmvlsqvq.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gsvcqrzpv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gqynvojmj.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gryojoixr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ghieivwvx.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gwyegvgif.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/griwmcuyn.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gspjufeva.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gmoosvxkl.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gvvsfdahm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gtmzmqrsg.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gipjkeaql.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gdmbivuyp.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gcoorkjxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghblagpmq.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/giyncszlq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gcwundhpy.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/guowlqgwx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gpdlbxngm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gjnnsszkf.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gxkmvmqam.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gfnuynrix.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gtivwdevg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gesjqynag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gduyjwryc.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gtzluuyww.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gydelrbnr.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gmgtygcgj.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvveijmue.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gimpmzxby.sHtML


<!-- 参考信息 -->