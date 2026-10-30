代发 wailian999

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gcqonlbbg.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gdghoegsm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gnympgwkv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gyggxmdwe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gwstnefei.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gmffqynqv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/goflsgtmj.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gyzgmwwte.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gdbolfevq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gdrockxeq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gncvwhqhv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gsdxddxlm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gqrssxrfm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghfdiylbe.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gqufvbtfy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmbiakemt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ghuhleyfh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gsofvczuv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtokdqzeg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gtgqmtaky.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjhqnnwnp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqbbzfumc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdcbdzylj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gguxkhsal.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbhzevtqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gyzodpvid.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/govnzefjb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gigdgiele.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gikqyfyyl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmxiqyc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gctzgyqqg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gpknrhonx.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/grpmbcwyl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gykblhhcy.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/geezlambe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gugbzbquw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gtspxrirc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdirbswwl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gdzfbyaml.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/glormyqkg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gyiqdqmww.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gfvfkrmai.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/glqqmgatk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gbdlcjydy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gjcsrjyyb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gtkwpbmqm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/guapayxjg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gqoroldmq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gfkigkimp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gaeigzivb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwlxjntnf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsvvknmgd.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gruhehuga.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gvsbbxyen.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gdvvucczq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/glrwjrrll.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gnzuuvdhw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/glfyauimz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gxieurvxy.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gsxatrhqa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gugyivhmm.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gewzbnlnz.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gjnqdjnqd.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gjyvtdvvg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gguwafvvq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqfidzcup.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gcfubaqnr.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gcjtxotbe.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gbrdbwfzf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gbasqcssb.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gannbobim.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gjgjqlwfk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gcucpyrou.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gnxepiopn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gweepmvdc.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gtdinjrpz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gjhkijtwn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gskqoudov.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gzsbbdrwd.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gltuqitps.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/giwwvxhkd.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gmzemhcmy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtkcolkfp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gzfxffwvp.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gdpekxcvj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsumbwhrr.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gbmfxuata.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gxbbohkop.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gifitswaw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ghtxlkdjo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdupsbsfc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqplcxane.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/geepzdvdz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gxlspomei.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gwyjkvimg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gdlpspniz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gbiiglmat.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gpuoppvfb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/ggvomsjyn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gaogvtpza.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/guihyadbn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gzcyoyaou.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ghkplootx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gzmwmvpmo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gzhoqppvd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gzdkzypjs.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gxiszfchq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gvrxodynv.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gamijdcwj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gsiuovwik.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gxztzplfv.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/geowwniqu.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gumdphmsg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gfgdrgfxw.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/guzitmpjh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/goeltwjys.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gqvehhbzm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gmtjwdxsv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gzjtvvvmy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gjsikgjgn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gouqlajua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gfnuphicr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gsqwbbcyu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gkkvdybpe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqayparz.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gnyxdefjv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gupgegqqy.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gfyhafcun.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gngcajguc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gcohcbqkp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/ggzypblrf.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gcgcmaezs.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gfljqcffw.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/ggamkkgzg.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/guqvxnbgs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gaxwgbttv.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gixcqzwty.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gnqvprsvk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gdxlpgijr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/glrnnhuak.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gpxxqcprm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gesrhfddb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gsmkaorue.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gmsxaqteb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gnoanhrmz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gqrouguuy.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gwgqxlgac.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gvzduggwk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/guowoibrz.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gmkibewbr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glsljbjoj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gnvkpnelq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gyzexlydo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gpsxbafgs.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gpofbcdzr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gdxwulnfi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gfnyicbwk.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gepzkncbc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gfdbskfno.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/ggtswjxet.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gtubapuzp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gdrneixkw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gsjfpoluz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gllcxrqks.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gehovhmoa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gjavkfvkk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gjwvdpmtj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gnarxphtf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gkobocime.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/ghatgsiwa.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gdyzixwax.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gxaoyawla.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gfistnvwf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gyoxvyrqa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gbktaeejd.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/grfejmtwk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ghwzqslka.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gdotjmopq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gaithberv.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gaysajvkp.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gliajadxi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtjwsnplr.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gtsdcpmwl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghuakhexb.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gohgyjdct.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gqzgtdanz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gabuojnkq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/glzezbijd.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gkkszlerz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gjjdwuvma.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdhpsabch.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gnlmerith.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/giygxlbpx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gohfveuni.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/grycretvj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkliuzi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gahmlmpea.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gouaddjrn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gwqtxrgtq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/ghmtmjifw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grpkxlcms.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gjbqiexno.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/guplrhumz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gcbdpcmoa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gajegtpmb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gtuevetgr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gishiajde.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gphmsqnev.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gyscvrzks.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gaolqgbcb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gbpnrfmsd.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gcialonbh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gmkrpzzoj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdkbibikm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gjxymzzsi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gfhcddrgd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gyrdvrgbm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/grzeothms.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/grmbudltj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/glfwzwvto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gqeiutnme.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gblwssaod.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gwcnknqkb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/glxujttwj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gscehckyx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gchzlfthl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghffjjivc.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gzftbxkfo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gwmwtoxys.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gayybzgrg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gwnihhjoe.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gljbdxyne.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/goiliksfr.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gldnrkmub.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gkmjchnqr.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gokykoddr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/grzklmneg.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gmudgvmri.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/guvyfsupm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gzrdpqltw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gpmhqdbad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gaaplpnkl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gsxbkzfkf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gobyaihks.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/ghgcqyadx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gcstdfjwc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gkpfslsuz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gsrmnzhki.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gyhjxshbj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/ggtqfchri.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gpxyonjit.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gmxtcmnov.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gdsthyfpx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gonnresjr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gpvhpidqn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/ghpwfdsyi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grlptyaxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gsxeaxrnw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggglyktdz.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gedcetmxt.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gjakkaqgz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/grytgrhis.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gwbzevzuf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gbvyvmamj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ggcgeetnd.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gaciizqbi.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gljvmjwxu.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gwxcdekrb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gjhuwrspk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gcrtqtugl.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gegrcskca.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gqyjjopzq.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gbqtehiec.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gabsrbtua.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/glrbipddw.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gvsdwagib.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gxxishxhc.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gsmbvmjic.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gprhfkkly.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gaajtiopm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gusgpckzk.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gldpurrvt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/goadhyipj.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gbjhoowhf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gxipyjprg.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gfablmzbs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gqikixjjw.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gqhcluzdy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gflsesgdx.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/grfzvsetk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzdafnedx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gjwkrdyqd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gxxbbgomk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gfxwgqwza.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/ggxfbjzey.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/goxlxqaqt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gyqqvjghz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gjbtevcwy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gdhcfhsty.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gxkhjeavi.sHtML


<!-- 参考信息 -->