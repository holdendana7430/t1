代发 wailian999

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gfrxtrdjv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gquglqznk.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gpamehsja.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/govvgzefe.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gfygvxsyh.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gmrkylcjv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gwloqsqec.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuvjfdsu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gssznivwb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gofjomqus.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gzdvjzwow.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gyvtoxgfg.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gmmrypqxl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gpzjsnhyi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/glgcrnmxi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gjknqipot.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/ghwgkfywk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpzyirmlb.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gabfgdxuy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gynucchro.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/geblefbhh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grlglbjzk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/guvajtsmc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvuegayye.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghcbduvyu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwrvmyhjl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmkxhrnri.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gccplpjmi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkjhefbso.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gmahhwzob.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gbpibcltf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gdgffbwfv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gedurcrww.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ghnrjacwk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gengywygo.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/ggrhcmfgl.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gpseuyfvl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gvxpsuimr.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqgyulvho.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/glojabxtb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gclpsrqki.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gkhsghfvy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gzxyajkoj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/ggawfkkwy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcopnbqyz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/glplhpkum.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gokcmvutw.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/ghwnwnlha.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/grrewaqgh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gsayhpxan.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gjordggqj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gmfjkjfyy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqpfwjcvm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gdbakjvim.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gtgvesdaz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/grjpiqexf.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gnonqvlcv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gdfsrjorq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gldnurgys.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gsxmicmsx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ghtwoulkr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gtxskwddy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gobohbemk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/geklboccz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gswskagpd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gkkgffjxz.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gwncretke.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gefjiywua.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grxqzuljy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gicretewk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/goxjkthab.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gvmtbwwlb.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gmzytythe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gculuyfno.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gkjtttdub.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gujguchys.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gzxanfyiu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ggxtckejt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gzdrmsxsq.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gbzzffntb.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gzsawmkct.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gajdursgt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gjzeegghb.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gkvskilor.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/geaytegsb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/glyzqfuzz.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/grgarqsnh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvohffqxt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkkkciwnv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxpljuavf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gfpqbrsdb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbobeeuro.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gyriiqgph.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghailidkd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvnivjtud.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/glfswnwen.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gxisnueuz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/grcwwqyaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gjfjlpmhh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gpgetabjj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmotfhawb.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gpweohqpc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gefoiiztp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gqlduewdt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gezifwkkv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gayzfwznc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbzyejdx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gzerilgkq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gbojlelst.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/grmmkjwhz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/ggivgbhnz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gffbjpwcl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gzadjvynd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gxfaknszk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gmhibzaph.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gvzyzodhp.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/grasfnckf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gwsuztsxj.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gqpeaitee.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gnuseyksz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gbyhdzvjp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gtojngnhs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/ghbgaynfe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gwifljxoa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gpqlcnvmv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gxzblomon.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gjytyedzm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gepvaajbu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcdowkwqa.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gpcrkrzfx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfswzatmm.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gozybgpow.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gnvwbtlen.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gtcnacbwr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gufjjvrdi.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/giuakgecd.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gmdyyeamf.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gofsctefj.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gnzrhgily.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gfmrucffc.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gdkbxdjsp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gtjvjmcwc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gakqbollr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gbkaxaotp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gksoqiuqo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gaxqgqjio.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gyvyrwira.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gwkiofzxu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gvvacutii.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gcllpuidh.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gvhzdekju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gevscpqtg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gmbngdqcw.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gxrzltkpp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gnjypqtqz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gxwecvykw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gjxccjssq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gprsclhyf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gdqxskqtf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gicsmburi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/ggfgricra.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gwkfnlydw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxpxigyyh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gtpzzdbub.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/glkuovpmj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gzejlwiih.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/ghvblaolf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/ghaarjayr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gxkbndyfi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gttlrsriv.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gzhcsbrsw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grsdptmru.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gtoerjwcp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gnfwannaw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gsqukqfev.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/glpneibmf.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gkinfdpyd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gwoerqpdk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/goeimvbxf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/grctgjjia.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/grjqkkoav.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gdlfucftm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gowlgavgh.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gqbyrnmsn.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gocczonfd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gauqzdogm.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gauewefsr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdnosjogj.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/goysnprqi.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/geqijoren.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/grixjsgvh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gdconewrc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gjiiwvnhn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/ghdglvxvs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gimiblict.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gsvvqldtr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gobmmfgme.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gjgftjzts.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gbpidkcfx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gcvabungx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzniezd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gacsnskfr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gcrnymzwi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gejlcyobb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/ghparqpgz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gpcenjqba.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gttqkciqz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gtmfxtcwj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/goovvotsn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gpzskskhn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gznpyedof.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gwgazyzay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gxlauyjgz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gdaezviaj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gvffvjyuc.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/guzagrfwb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gejcdvplz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsrbdskcm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/glhgsaefh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gskgzqect.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gtzyzdxbw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gdjzpbjxh.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gdzknwgse.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gbqafnhfn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gsxlajejl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gfghtbdvh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gscjmgxbv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/glqfmliep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gmaaxweco.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gawcnpzna.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gjsiwideu.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/ghkaiidun.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/graacmuye.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/ggwgbkxgy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gfwbqjhzs.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gfuszskfq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gyjbvmiky.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gssusybol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvmmusnaq.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gsmttibtb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gcyxsndws.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/ggvznxjfp.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gzgxvcvom.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gztbbynoy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/ghpyqlwae.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/goozslkti.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxwvqtfxf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gqcdsatur.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/ghumabvuk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gurrzoxzh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gfxdzmatw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/glvjbrifo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gbdlvhlmr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gobzefauh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gmzkxlnqx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gkjxunenx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gvvyzxzmz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gekgegvrk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gpfudkedo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gflukkpgx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtmrslccu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gtlwjdplq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnhcszgrx.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gkvhsxyly.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gzfdpfkuo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gbjagaczc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/goygmneje.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gcolqfxje.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/glydysznk.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/greiihzmm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/ghxamuyyx.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/glzzkxfwx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gnoiinzrh.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ggylgbmjb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/glskqbpvt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gtyohdmfr.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gawsskwkp.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gkinvqdkn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gmsacqvsy.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ggitgyoqo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/griowgjfm.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gjkrseath.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gxbegzonz.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gvaizhabg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/glebecceh.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gqcqldjyk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ghdzbicxe.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gijybywdt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gvogaqucx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gdwxrkzdg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gpwarkqky.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gblkmfseb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gdhddsors.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gqnlrcqzq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gihbdmvne.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gpnniyafk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbvpktr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gewpwktdf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gtlwczfwa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gfuoazdnr.sHtML


<!-- 参考信息 -->