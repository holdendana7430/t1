代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gcrbccxxq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gslycrggv.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gztwutngt.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxwsjjlje.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwkrtsucq.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gskrztmav.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gggrnokmj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gvhdnbvqe.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gijpdmraz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gcayuwxkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gcmdqlmfv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/godjnydwh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ggpfjibuz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gnbxsicyr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/ghhugvusr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/geqdymfmi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/geasfsawr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmbeljazz.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gwnnyhphf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gucrpkjjd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gndmkybll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gixtaitld.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/guwedsrqi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gkhudlfpp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ggctxzbcb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gngddgpem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcwkgbfsd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gmttqgzhp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpuoqexqk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/ghztktyep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gorvgkanu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/grctanzlg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ghflonwyq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdupilypn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gqlhydunx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gjkuwxoap.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gtbrjcfio.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gqfxwiyfc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/glfvbncwu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/grjannhtd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/ghtrvduai.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtjvcubev.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gkvqymdhx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gmnofueym.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gcwkandyt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gmfenvwkj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gfcxdbmkm.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gllmqaaqj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gbiodmmwd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gvbsfucsc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gasqwsnvb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/goyoghvhr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/ghxcunnyv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gxjdqvlux.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/ghhvivpzp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gbltetzkv.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gyvejqynu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gferdwebx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gmdbbepcw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxikzqwd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gvilqaiwm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/genvqvscu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/ginwgtony.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/guaaqtqqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gktcquvqh.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gcsjdoyqc.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gtjcxdgeh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gccljpnjb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzsfmosiy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghshwwekr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gmqxfhgbd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gpfbrwoqo.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gelwkoehj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/guyxiwkng.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gdbabybgt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gbhmsbfuu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gueizpuev.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gurijvdhm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gjstkxhaa.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gtzgdlgxv.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gcgymntwo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gqushnpyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gsuqyzwmt.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gvbnukoxf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gudwhsuxh.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/giunmbfim.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyegiyzfh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbxqvnzmw.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkeznwxxq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/goicquvyx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gsrfrjpwr.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxdubaixj.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/glhfmbamb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gofrdnyhz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gyecvvuqa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gcnnxdcxt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gacxcnekq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gvbezmiju.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gnfkczvdp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gvtpkdfjn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gsbnazify.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/glswjmdus.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gqxqqgxty.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gpauihott.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gicjrwrfj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gjezzpzof.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gstsqieza.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/givlwyakn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gwdjegodp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gcssxavvs.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gmkylwvwb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gyzsqkuob.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gykwansjr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gkrnxjpei.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/guyzqrnmr.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gnfowybou.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/grfknxhiz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gexpbjriw.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gifkerdvd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gtnamznfc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gdlcywvij.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gnjyqlfnu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gmkcjjshi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gfmwmtlyp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gvtkxwwqm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gyevwwmzu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gqoouaomy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gggcihela.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfcnsuycl.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gfnznxfgw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghhzqevrh.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/glktedqyo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gvxwvhlbz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gbimejtoy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gmyvxxanj.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gnkwnzlus.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gvwspnalq.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gbxoplwav.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gbkhemokv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gmklufisx.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gpyxkhpwb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gdmfeuvei.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gwglzdcae.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gsvrrxkzm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gjgdincal.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gnhrizjvl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/ggipwdosi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gguzfhkoe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/ghwyhjqvw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gdoaukake.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gbhdibpan.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gnhwgddfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gfgtsulgl.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gvuytyajp.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/goospthwb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gifhegfph.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gvnnapcdx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkaicpikk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/genxkcbcl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gcdmzbigj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gfahvqzwo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gthpzunjw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbovescrn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gyxwnvlsy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/ggywkjxdg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gflmjdbzh.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gdrvwsyid.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gthzvrlua.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gzxnsrrzf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gumbixmws.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gkxyxcmct.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gcicqcrje.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gyxmgtpoo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gnplqelrh.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/ggfropgar.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gtkuqkjwd.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gbukxubcj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gmxrxjxib.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/ghzfjbzto.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbiwvlsop.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ghnmjhmxm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/goqbomepi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/goypponjf.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gyajfeemj.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gsawfhsmr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gextfqmqg.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gousbatai.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdekwouby.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/ggwccwzkp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gcovmotsd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gwwjchicg.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbzliqjfn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gijpkigcq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gkxnmbypp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gypulgdtw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gjdegemdx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gepsvsqnk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gvogatneu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/girgxzalv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gofepbnuh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gjhpfozsg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gsddlmviz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gknlvzjfi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gregmecfw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gydycouza.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gfjdpdkfx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/godlomoqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gdmlfdfwt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gkreqhgqp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gjjxxefni.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gonibtcke.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdxqphsl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gfkzwfhik.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gehfyrxap.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gwduldlet.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gjkrkjavl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gtictemhw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gersponbw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gkpstjdmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gwywtctlc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gjfbhbxyd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/ghnijbpqw.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gpawnfvlc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gjmanmjcg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gcjknqlnr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gyiiqkrsy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gisaccmqi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gajnrwvad.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gjobaefny.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gnqvfxhfc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gjfqffsxs.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gztarywkh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gkkweymat.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gtguggxyy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gqgmavmlh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gpnbrynuh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gonzbtsbk.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gamaqvjxg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gkinoaclp.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gywvpldvu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gwlkbkuvf.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gihlgmwme.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gvwxpfkzo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gkndhngvv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gigvbxheg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gisnyvvew.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxozfobom.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gnpxcbhic.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gtrlujddv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gfiorxheg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gnpnydoth.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gyaagytlz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gbkxftjso.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gsrzkexrs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gwmvcdnth.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gsjfxlutk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gynsnqghc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gdltvlqyv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/glvlemfqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/guhlxcqjl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacgdrdwg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/ggddsunbz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyjfiyjue.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/goevbsoor.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/grqgdihdi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/glirtkhfw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gnvbrgyck.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gzzzqixip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gzykrrssl.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gragtriyw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gxiszzjsh.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gddulliwh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gvuigpxxw.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/galytfqag.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/ghhhbvvjg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gpwaihxqx.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdmdppgaw.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gmcuzctvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gmzctllzn.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gtcaoepjc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gyfktkdkf.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/godauoxrd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gawufspbn.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gymsceqdu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/goxtawimo.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gblzvvatt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtvdhhoda.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gtatudqtt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghoiiwimx.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/goqadlydu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gdempqhdc.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gtlknabhi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gyqzeaxtr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/goiudlitw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gknqpvxlw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/grpakiufl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gfimbtkpx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gazxiucnt.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gwcotlaqe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gdpapfdoc.sHtML


<!-- 参考信息 -->