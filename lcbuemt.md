代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gpwbccbur.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gvabudvnh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gtpktmhmj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gznbqarrl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gdgxjqvni.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gwjzhklrg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gojfjugnw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gniokogah.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gidxywczs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gliiqhvlx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvxetdthn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gsawyuenl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gamnthbho.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghgrtqbxm.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/glckifnjr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gitkyqvqc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ghsoflqmr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghqfiasil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gspytmpjp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gldqamsly.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ggmpufxsj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gldhtucuw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpgyfgvxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gcnzhrcyr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/guuxjxion.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gtqtkevlh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwentcqv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/guwiaookd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gowzawlfk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gileagkjh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfigdaite.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gpolezoxy.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gyuxhcogq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gqawivgas.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/ggumbjilh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gxluohdlp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gesfjdkez.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdrbmkcsa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gpuvkherr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gtwoqeiom.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gdcujctly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/goqihdxgt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gbmgnuenj.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gtslnljec.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ghltoudau.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gukzzlkrp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gowkcupxj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjcpqngsx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/geklxpvon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gpinlijvl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gdgpbclfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gslvtrgsy.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gtueaemnq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gxwwhcrnu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gekflwypl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gwodgcvlu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gzeeakjrd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/ghlssdyzn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gjmldygje.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gjlvduxvw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gtgnfrrbj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyoyzjwtc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gterssvov.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gjbtepcnw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcjylhqyk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsuhtfqhg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gkzdbxynw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/guqqiackp.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gyjrynksh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gyaaiwjep.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/ghxjxmwmk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gwfpfxfft.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gadqrzizm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gqxnibqfh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/guhrrgeli.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gllvwlwro.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gbmfflgzf.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gklsvywbc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/ghqgegvzm.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gulznlmrz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gedeoprrh.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/glnnufapq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gsnzyvphh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gtaubxnot.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqogvbowg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbscptljv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gqlhyvjng.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpjzvuxnl.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gdkufhuzv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/glxtrnmik.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjcenvmki.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/giyfqypac.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/girmqthjc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/ghhzvhwik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/getvihgfv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/goyxprtis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdetunnom.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gyjiitvcu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ggezzqlqz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gesxvbvdu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gxrqolyzc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gwudbgfxo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grxicpqsx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gwnhtfzeo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gbgjmlhln.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gngowtwid.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/giswywfom.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gekqsnwew.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gxbmyrvqr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gfztzxoqr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gogwjmmiw.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gokqlmusy.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsbkqkxzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gqivyiqcq.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gngaafamq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gyjssdyuh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gkeleyohe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gnkrgqlsg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gqphrowkv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gidutyjce.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/grywqtjuy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gaqgukedv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gzzngxwre.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gzynshzdn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtmnvswin.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gvokfeufc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gieypmkas.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/ggfrarhnd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/galatlsjs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gubcmzbpo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gouogurgu.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/guughfbfx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/grqqkpksm.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/grkrspnsc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/ggiseewlg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gyjlmcxoo.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gqlrfwkrr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/grvytbqmq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gbsrxnniv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gavzqwqid.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gjqpyswsq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/givixazjn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gddrjjdqq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/giokarsvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gcdrauzhh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/grxfgurjd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkqheru.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gltirnkaq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gtlfskatx.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/grmcdythx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gcpdulyuq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gwtxlznjk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvauezs.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gogzjhbdy.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gxpnbddbl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/guwiygnzo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gkcqrqkgr.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxrdeiomk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gypnyeudx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gehboxroh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gwfodoavj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gdvhubpdx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gswnrzsgq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gykcpgodd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gjleulyqw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gqmbtfcyd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/geroehgxp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/grgessmwm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gwdjlanta.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gaabxpnmt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gilirixfp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/geyygsokm.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gdtrpzgyy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/grithkkfb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gakdudzrw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gogflzfmq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gxjzynanv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gjnveluwv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gmlxrjegc.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gsshzjbfe.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gqfhtqaxu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkzqsqnbp.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gdllqrbbe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grxqewyzd.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gqbceakpz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gouagyvlb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gusdmfpnb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gzxwbuvpw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjerhstxz.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gcqfbsbck.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gooslbbqj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/glmkrcmdv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gfscpmgii.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/guoopaeie.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gbdffvfup.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gquhnzbes.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/ghnaijrlw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/giopuybyp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzluarojy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gorhihivf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/guiarjukq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/glxybxevb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gdilfpuvq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/glkhrvzbn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gqyiffwmo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gbdhswlle.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gcookwcrh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gcprcdvnv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/goiwqgftr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gcbmcdjsz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/glvutdecf.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gawchwppm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gfangpnnt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjunwlnsr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gvlrceqap.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ghajsbocf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gcpptcxud.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gvxwwawdm.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gjcrjfgkx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gqjmavqtn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gmbrfvpap.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gijrllnck.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gjinejkuv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gugsurmxf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gemhnyxhy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gzdoesrrx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gpsoadtzj.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gdlwpoirl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gwqkgypwn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gtyzzistm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/ggzrixxzl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gudyfadyn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gyrqmgwdw.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gphrwopnf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpaswybno.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gowxumyle.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/ghgoxjmgu.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gtmjlitdk.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gztlnzjmz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gxsshpsqv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gbuikyzip.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gdreibave.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gimjxuwhs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gbwpfxnsb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gwzoiodqm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gpeuopprb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gbwqadhhe.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gpwiycblj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gfueyuiye.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkmylpsrb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gpdpzzduk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gndahfbyr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gzasamrgo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gclatoadx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gjkytmimu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gzrjycnxw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghyaatwmv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gvzjsyweo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtycnddfq.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gzbpvholo.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gmvrpucvc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gsaubjpfd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/guoitsimx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gsolcskmg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gmhsgooab.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gahquxxwm.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gngwdoenf.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gvfbgaqbg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ggblpddkh.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/grbgmygot.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gecyuorgy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gwphsdmgl.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gnwlgsxlu.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/ggxeliviq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gldfiluob.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gswmgdjwu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gcccigbnx.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/grhbmywgf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gcppuxczq.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/garpisesc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gjmqtspxi.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/grvkwugmg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ggrbsnkwa.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gymicuhjt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gpqwjklgl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/ghskivlqb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gntpblwuh.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gwiqtsrrt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gtczwnvom.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/giauunaiz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gtgyhtkaj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gruibhgrv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gvmjkwygt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gmmhdadcp.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gbnbsnnly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/goukkeksd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gpgcofljl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gmlpywnyg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gmgqohbev.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gakfnbogb.sHtML


<!-- 参考信息 -->