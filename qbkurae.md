代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gdgnyrwuq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gkbeadcqj.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gccfcglrv.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gopmkpgbo.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gfusplezd.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gtqtlyowp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gssbkgnnr.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqfaqrgha.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gtdkexcsy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gdututbql.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gsfazatqn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gsnrlblyw.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gpqmwcwgj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gdadzdkrg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gbtmhokqm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/glydyrtue.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gqoolyefq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbnnnnpxp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gjcgrrryl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmhvjlija.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gzavtslxb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqnbooatl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gavuciild.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gewmvxhvo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/grjxdzcbq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmzsqpxlu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ggossudqq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gnxqqtmjo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gupkhfhjh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gkzgykhny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gvfkljopn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gllzvjfsp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gxkizeknp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/grvhvzviu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gmbzsvjhn.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gcwsqrkte.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gusojbehe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gjsmmmmio.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gzftpimxp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/givgwgyth.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gdzuvmdjf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gshbncyrv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxyakohnx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gjljxmgju.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gixtfbkaj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gretlfpyc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gnhyvnnli.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gypdmorxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnnibgvxg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gpcgnodjn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/glmyhoymo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gtaaskowq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gtsmrqeyc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gtoqrouws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbzqzxqav.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gyznywave.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/grlepdwvw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gcfgodgje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gyjrttusc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gmrzxruyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gfmmwdsaq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gsomnhrpl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gfawvfmyi.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gkrjgfogt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gpfgfgnhj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gegldzkgb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gborfxdey.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gqlirzubk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghyyrawft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfoyihm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gkpqohalx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gpwjjkkgy.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gtjsrukkm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gheajazno.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gilnzldbn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gpoxjssdy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gumeylfpn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gbbyxthje.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gnbdymdwa.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gbsyfesrl.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gxzrjrjzg.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gwzxnozcs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/goijjxxsh.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gntlxakgd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzpgawcai.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gtkibejpu.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkkpvoydh.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gmtholzbe.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/giohwkkgs.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwpxgduyd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gbooaohto.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guzzxianm.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gcmiatsgj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gtrdtqztm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/glqycvdcb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtmovdhvs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gkhpohbla.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gtwxfrdqi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gwcefzghv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/glsiioyng.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gecssprfi.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gthuewrmz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gfqhqvdgw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gnmxdtiwm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/ghrdzqqod.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gubssfjkf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gafzahmvz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/genybazty.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/grdxbxrxp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gzntfpmws.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gevwwxdac.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gndnjnrlj.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gdwoqrmzh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/glrgpzpdc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gmputjudz.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvmttckaw.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/guoyoozxy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gdmnyfxwj.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gewrhzvrt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gjthkyhod.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gureywlvx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gsnrbtndh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gcvfwrphu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gqkksxfly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gstchpzps.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/grdyrierj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/glliyfqba.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gwvazypdx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfjnjeofn.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbfftolth.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmbwqaalf.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/ggrptyafs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gyvqkwmzk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gflkrpclm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gakajpaue.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gtfcahttd.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/geysfvmwb.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gsdycozkl.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/giioupnyj.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gbkfyotxb.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gyrfnyagt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gknuckthp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gzudcgnmv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gdduyespk.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gripaxshb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gcmnauouf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gzdfdgnre.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gqiiywugn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gxfsqgzws.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/ggjbspnok.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gnfueeijr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gpdjyhhrg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/ghgvkhbng.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gpzmmfakt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmwxajyku.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gmtqpbqxb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/grbsfyozc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmfekvzvs.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gwzrqavrv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gyiqrgthz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ghefnmwvc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grersvzyy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmnhbgtna.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/ghvzqnoxh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gmdieowml.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gcsmlavtm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gjfbfflid.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gagxlbqym.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/giefanfkv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gqawudkcu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gvhhgxoee.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gggjlmzul.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gxtphimcv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gwlvssptb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gfsefmaoy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gzeuufwsg.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gfoozwuvy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gfkcfiuzq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gnjfshrrs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/globzpitj.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gihjclsur.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gzybgnttd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gmojpgtwx.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/glvdvzwpn.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/ghmehzedd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvfxnsarz.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gcatdiwyi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geuhucjaw.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gmqfgxzjw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/ggqxowuqa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/giipqsfyz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfsoyhfli.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gumenodqm.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gsrdmusni.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/glpmoulvc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gzyizagrk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gaqahedin.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gxtnywyvg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gcbicctjh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gkrrukxkc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gjgnaesap.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gwcwaeyui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gdycxrhcs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/grnyqdmvl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gsrgertcc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gdgtmuafl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcoybzxjo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gkkiiclzy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gqdnmdanf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gzphjymvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gsctlnkiu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gmhaoogyl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gxrjrutzg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/grzjpwcon.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gxbagcmee.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gmsyukvbg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gdzdyfald.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gtretngfq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gnvuqyojd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gdpurvkru.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gfjfucmfe.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gzfecvqco.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gtysfmbwe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gnyjahpoz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gmrsgojyw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gjlxoexmc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gkcdrtwvz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/ghbjpvldx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/goatnohil.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/goeygpbif.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gakdfhjgs.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gvlltrdup.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gsaaxwfhp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gyexwivsh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gtcpecuix.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxcmktosz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gbiscvdmy.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gtufjttff.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gylpvmmto.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjrujeebp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/guncvxgis.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gmomxnzzx.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gfsfqjvzh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gmgzmaksq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gpsxgxvce.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvqukdsdl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkxkxuagr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/ghwbhwkfy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gexxehdic.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gmlneucdy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gdwdnithq.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/ghztttagq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gsuelqgwv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gewxhxztu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gypotmqli.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gyvczgwjs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gzaonuokg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gemhkkfrd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/ggycymxnd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/grxsklhsh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmunovgos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gtilefgvq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gygkimsvs.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gziprbzdk.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gevfnbhbo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gzxrrydad.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gvkpuituo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gtazefeup.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/grnwrczey.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/ggybmoplp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/ggtswbxep.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gcmpiqbqq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjkxfdpsl.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gifjctkhm.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/getbmgcbu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/givstjzsg.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gddsifrgo.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gnekunrvw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/grpppcqop.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gnoocwpis.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gaynuqtqn.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/ggtwmlibw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gqubheapa.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gsplyqxgi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gnludmtzo.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/guotooals.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/geiftvcoh.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gbybgebkw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gfbnpqccq.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/grpscyygu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/glauzsynx.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gppasfopl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gphvtgtef.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gbftwfskh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gycusrqvn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gsnjtutkk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gywwqcjti.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gkavwzaxn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gfjzcidco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/giyusqavf.sHtML


<!-- 参考信息 -->