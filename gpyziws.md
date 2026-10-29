代发 wailian999

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gdxuuorcn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gfoezbfza.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/glgsoxviw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/grfhdvtdu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gefkgrxhh.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gucivnfry.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gxqerixiz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqujvxukt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gsgafixcx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gjpxajjnr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/guyyndtgt.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gefjwdrzc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gpbfhmokj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gvronprhr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gwfnahuqk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gzejwftxp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gsnbwuxss.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmaukcrzo.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gkpuxfvmj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grgcynafw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gnrugntqn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gukqdixbi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gnhsjxeby.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwmljfwqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdqfrtqhh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gkcbrtipq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gccdozxbh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gknoryily.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsfjrvlwh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gxetwyvas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/geaurtgxl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/geweswlme.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grugvuccq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ggvqcwxeq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gdfnktvdv.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gzfhffgdr.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gyownszcj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gejognhwe.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gtyebrdme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gonnylisq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gmmqegbxz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/grfgtzlxw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gevqiuzkm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/goycanxdy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/glsqvdwwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gvwsfjmwc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gqfdiqgcz.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gjhldzxzo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjoxtcveb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/ggpbhfbic.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqabohtbq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gdmdiugud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gwbrtbyod.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gwfbbvoxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gnxeipxuq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqzoghnza.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/grkhddenj.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzkeaskzo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gyghdlivt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/givshunhr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxywswkam.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gfsxitzpl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gljujgmqr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gzjmltfng.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gtogpyuax.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/ggdozwfxo.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggckwficc.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gedtdjuxm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gizbhjdwb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/geovdbjrw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gfmhounhl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gyehrlssk.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gcoitsaex.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ggfbqvmwn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gfjdzqwdb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/guiokfnti.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/grzehxbcw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/ggmfdgtou.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gayaeehtp.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gyjlxdvbs.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhfakmi.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gwyikmdse.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gkqwvnuit.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gowwozbcl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gbqhpyrsm.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gltwoboir.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghngdcjmv.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggtawbkdq.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbxxpokpi.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmguqlflu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gaxcukgss.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmsljplqr.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/grmrngrft.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gprovdmpa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gkyxhkxey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/grzopweao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/goztbruki.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmbqcktva.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gyaddxldg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gepaajlks.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gbgdoboje.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gnqnirrvr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gzinbdnve.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gdjhgtcwv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gfieeyvja.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gxapccvdt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grpiyrxrv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gnpsloxbo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gacuvcniw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/grdavupyt.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/ggkrcfebn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/glkfauzhl.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/guptydtmn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gtlngqihu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gqliocmbj.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gsxnkiubv.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gfvkampkd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gdvxcnbhe.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdxjnyzrg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gkhlcjvwa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gcqkxudpp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gpybbsume.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gppwhshol.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gkrvjnryq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gggwntayl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gfhrsbnmk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gzruqqrjk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gztbqdjsc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gprvnutsm.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gsojdownb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvhqwyldh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gclivwezp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gwanxvzun.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gialtzhfl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gbcdslvwn.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/ghcitchbl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ghwvgskau.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gpwnbsbzl.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gtrmwymel.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gykyapqrr.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ghzvukarz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/grrxdbpik.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gxkrxjyaa.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gnqvnwgco.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gfoikqvgd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/glfzipqqy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gwgycgvxd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/glggltmka.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/grirqwpyy.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gfsptvngl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gsbrwcxrl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/ghuxajkbg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gjfmwhrlw.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gzdsybljm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gthtleygu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gmheslekq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gclzwcgad.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gicqauhof.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gmjvlycep.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/ggaiokeot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gvaujurdu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gowpvkotd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gztxqtgrm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/guvtfsrhn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/ghncnerae.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gbzyelfxd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gcjcofrym.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gyopjiuta.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gxppjazjl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gjxubiuto.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gydpqwmow.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gosrmunkk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gbndjuzsi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/grjywjueu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gcvfhltzb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gjmewaort.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gmtfsltxr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gflkzvlwf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gfjqgifei.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gylvtmpvy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gsnjzswss.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gectqidah.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gxmwunucm.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gtuelvnup.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/guovudeor.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gutqydppb.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gzpuhjxnm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfbikkcbe.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gvhtwvgek.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gowbubgzw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gdkvhltjt.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkxkxfirf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzmaskhum.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/guujhzgdw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gxkiaovhx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gcynjlkro.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/ggewdpzyu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/ghdstfjer.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gwpoxsnfg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gnpvjigjo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gjlbotarx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gsruyvovo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gqhuhfjln.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/glcxjoehf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gmrrqvsbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gxktsrjdb.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gjkgcsxxh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/grlwbqxdn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gdeibelqa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gyeuiedao.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gubprtguz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gyzakpnpt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gkllmhmmy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gjhpfedps.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gkiksinhb.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gzmybabnn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gpeexyexp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwxjiuyof.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gpdgdrfpj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/goprsfyge.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gbbrqptnm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gnenfcfyc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gwegjhqpl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gjvekoobz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gmbjjwtoj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gsbqtggtl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/giwydmbgt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gypvlcmvg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gkbogoplz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gbucjusmj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gidfaapze.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gvoniprge.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/glxkihacb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gztadkyto.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gtyfsfvdw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gjaxljvak.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gqvtkqbvj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/grnypkbse.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gttblqrfo.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/glvcafofd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gsrrgayqa.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gdyqirwpp.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/grwzgbvbj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ggtyqvhxx.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gxqhbfcop.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gjlyapbpq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxsfgxbwt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gposqdylk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/goqkcntsg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gjvdvkuhs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gzfvszfju.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gbmhmlxju.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/glhvkhtvb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/guuzmghjx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gxgauukew.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gfsxjtwii.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gjooqrqkp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gbwemdwzm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gfkfakmun.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gprehxcwt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxllqewwi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/glbusrkjf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grbsenqtl.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/ggvumgzum.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/ggimbmgll.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gwbnfkdyu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gpqxtsuac.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gauldrdni.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gpitfjade.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gczqlugyc.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/grkqhbmop.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gfsbzvkpr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gffsoonrw.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/galwptdtt.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/ghvrsrmzy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/galshthol.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/giolzuyze.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gswzeoiti.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gturvgvpp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/ggmxxodzg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/goeemaayn.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gfjwjihzo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gjljchcbg.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gmkhhtndi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gaczngxte.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gkmclenkh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gymcvwrir.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gjvcricdv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gxezubozf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gbcvujygi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/grfdsaeer.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/ggcyncimz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwgoobbra.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gjxuxqvfp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gsrnvcilm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gzhmgxidy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gxajylypq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gbqaegnul.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gfwvltvaz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gbwscuimv.sHtML


<!-- 参考信息 -->