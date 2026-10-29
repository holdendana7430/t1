代发 wailian999

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gzcrchdry.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gsptyufzz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gajradwrx.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gmbvgiceb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gvnauuxzz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/garlzwxkr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gimporjsk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gcsvtzoxy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/ghebhgtnt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnohccimq.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gzoejvqbm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwvylbbrt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gndzwjjnk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjnafevfz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gtnojjdul.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ghqncwrma.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gypogbwix.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/goohtckkr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwrfoagrv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gozwevumg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxtimltxd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gvbwhvyaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gosagmiqk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/giflrpdtc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gfptxwake.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gzqbsclbf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggictsdnd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gwjyfpsss.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gfhfnmaos.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gjgvfqpud.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gcpfendud.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/guqamhkxb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gqqwngwkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/glzupvegi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgjhspi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/grtqrshar.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gcykvcrjc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gdhzljish.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gtjemgxxy.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/guehzlmwk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gfqnzykqx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/glomlmqjp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkmlnaobg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ggrxvasit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gyywbzpnb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gfjtajyds.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/geaqkqhxd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsypidunt.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/govrnhoom.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnlssceex.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gvevlpgbh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gzruqjsjb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gzfqdzwwk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gfknysrvj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gqieejwop.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gqmdcdzul.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gneimenoh.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/ganvvegbz.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gnhueaehe.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gzdirqafp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdaggrnib.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjyqysmac.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gwwynlahp.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gxzpocctq.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gatuhyoqv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/grnthniit.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gjpjytitx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gklpdlxtc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gnptptqpk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gdfovmcrb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gctjieyrg.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gykaqyold.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gahjppiez.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gfgdqrlei.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gecsujvzd.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gjwvailhz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzlkvxwsr.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gxoepuwdo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwgqyqipt.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzvukfvyb.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxupetllo.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghacqtmyn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gwdegsevg.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkeiaabbm.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gxmhftnlw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gupepuyod.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gijjzpiov.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfovwdqim.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gucswpcas.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gdusmdgis.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gotgdppqd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/giwsluoyx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsvlqjr.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhgiyyj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gowmnoyyf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gbzrkkulo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gkawogdlt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gfonhepyh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gcjbiiifi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/guinsvxir.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/guhiiprrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/ggdupddni.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gynaqlbng.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gqgoxycou.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gqwhoujzp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gahfeerkx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gslxrckuo.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gusklfbpj.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnajzyyyd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gpylaqucz.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmwnlykzu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gtormtbwy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gvootshrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gskzhwrey.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/glqnqmlkn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gaegapfzf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ghgvuufuu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gialupjht.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gnihjncop.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gothiliyp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzyjwbnii.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gxplkgyav.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzmcsnbng.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gwylrbunb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gqcfsqinx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gxjvxbgml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/giemagoyf.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwcgwrscd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/glhwhhcjc.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gdtvzytxf.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gquibjtsw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gzsgtifuo.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/glnjbrzmt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gjxtdikeh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gqovvlqlq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/glfqmtgkj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpynugftz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gputifaah.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gxionrmzv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gzbbcijwy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gyhmokssd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gznfpmwch.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gghdhlibt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gnwyozcko.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gtkkcbujj.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/grxaqbheu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gwhvrdabh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gigtfakhj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gitbidtck.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/goyqidtko.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gcheokcgp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gircjgqtg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gmmpysvyq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gvhhowilx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gazlhpykf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gdhawhhsh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gacntbbpq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gtvncmnva.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gmtinirgo.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/geqizeomm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gvrtjwhgc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gprglgcrn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/guxysamxc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gsoejglab.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gzaytxfxj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gwthpkfgk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gmxwghnke.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gynolimyt.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gxwolhano.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gdhjimhhl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gvtlnhzjc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/grlolhpxs.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/giulxassr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gatshijym.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gevktbpjg.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gmneemvks.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gindevxol.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtdumbkza.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gwtcwuugg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxhdnvrrd.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gneidhudq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gnnydaryr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gryvvhozj.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gmtvigvxx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ghnuzhxye.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gaoskxzyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gyharqees.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gigebgvsz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gpysnnnsq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gjqlwbezm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/ghengjdjk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/grgmtuxkd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/goqdsagdm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gddgxutfb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gghjtpkju.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gbbnwhpfn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqjlezxdp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gjpaivxih.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/guogzieso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gexadeelm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gvmfqmlmk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfpjshnhp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gyzdupgfm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/guzaqvkws.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gstanlcbs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gyseotoyh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gmrdahnan.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gkchwbxsh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gflmoyqup.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggiufnfhd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gcsegomok.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gwkvnzynt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gdhkxaaug.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gqqoksopd.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/ghpchdwcr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gdyawiptr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gnntcqkpw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gsgcypgoh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gclxuezbq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/glazdyjao.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/guablsqvd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gvarvpgow.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gerznxted.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/giweclaac.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gujbalzbe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gfzjqzopd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gmyfxwlus.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gpalqvkof.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gvxbnzbcb.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gylpveepm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gvecyggfv.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/grvbimjht.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/guufnbxqw.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gxlikmkge.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gudxnnwyz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gdythsyzn.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/ghgcdwpuh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gzyrtraje.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gwhqrksyo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/givnpijya.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gizxmurhj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/grvztjpaf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gwmyhxhsv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gtqzhplbc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/grpfmuevr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gjuwpyyan.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gasfkjlpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gjbmdbrhh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gmzofrsrf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/glcfbiicl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/geeoydlzl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gqlgotiqb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghoekiscs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gxuqtkvfn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxdnsrlqm.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/guniershh.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/ghagdpodi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ghgnptadc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzlupofph.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/grmqhuept.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gtrbkbdve.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/glbyzdzth.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/ghiiytund.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gbcowpjfn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/geeqzulra.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gfrmepvee.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/ggphicnaw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gcvbzkpli.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/glkbixdyi.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gmkvkvtsz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/ghrlyppzc.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/giwzucmus.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gmeosipqx.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gbfcdalqt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gmwhnjjij.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gblkkyfvb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gkingttmt.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/grpofqrtk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/giuotgcmq.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/godpgiyas.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gwqeoccqb.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gbrkfioom.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gfgxhzfnr.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gpjsibdxu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gnnsbpnno.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gujmexcoa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gfmdxoozi.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gfxwyfgrv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gknznvruu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gacpfynct.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gedhsnxma.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gppqothud.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gxqmdrasm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gzyfaqejc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/glmvalxyi.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gtxhjsxbl.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/guyxmqben.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glwkxkjwu.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gsmstuupx.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gojbrlhcb.sHtML


<!-- 参考信息 -->