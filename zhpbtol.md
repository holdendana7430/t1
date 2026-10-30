代发 wailian999

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gogkuljro.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gtmaqlwws.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gcnlmddxv.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gdfrijfta.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gjmeyblgr.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gclugucoi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/grpifemfh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gsnndyscs.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gjijmroos.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gmayoimjx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/ggpeidgte.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gouqcaxbo.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gxmgbghdt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gjqbefibl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/grwruazks.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gxvcvsntz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gxfvbaekb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxodkzbxn.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gecvnague.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gewvjyoxo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gplvnsnqt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvxrkrrrb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gbowunygi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gkliyxbem.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjikcvkgt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/giwktwokr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwlvwdzrs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gottukpnt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geetovvgc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gyvsqpxle.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gukxbkwsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnanbthtf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gegucbbcr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gkbxfnvys.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gnjcnhdkc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkspxcmhe.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gscqthtnn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtxypmpfe.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gkmegpnet.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gimrvgqfj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gtollmsel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gbojvxudx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gtrfipvsx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gynmwbboj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/giknwwmon.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gbwjknswt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gnavsxlal.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gsanqlnhr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gkiltzkey.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gpglviktu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gvuublfrf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/glcapojbg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gpctzeigx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/grdjozajo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gskwtfcrg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gzdfclwox.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gxgwqypog.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/glkaxynjv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gqfavdubf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gbgritjrf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ghatismyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gusecczuf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gmkqwtkqz.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gfnymkcie.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/glgyjegbc.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gpwpjmyal.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gywlmzamb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gjrtbyzrp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghfcsjoin.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvpknxjhu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gybcyeaqa.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gngtwsrne.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gbfqcrtwu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gkzdetypj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gmrntucym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/ggcdnzkia.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/ggvvnngtp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gzwrdkwdb.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gttktnvyn.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gjojtlhpu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gbqldwrot.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gknifxzrn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gjhomlbqa.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/goypqtvvu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gmnmlipsl.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmpkgnt.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcduenjid.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gmcthtfpw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzmubgump.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gltifnkbg.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gxyvolxuh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmxwdqnpv.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkicatpvu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggqiafjtz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/geeogimpt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/giizoensj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/glymsiqol.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gaezivnrs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gdkkolcmw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjavnuirf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/goiompecu.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gfragedpj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gfacnipch.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gpefmriun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gstgecwnt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gvildsjln.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gxhiakzhu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpdyskbs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/googpojtl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gurbryeku.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/ggetrsfxz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gufrzlyhv.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gjgyegtvn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gqymxxaft.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gzafdxjbk.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gvuljbyjn.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gghlyheub.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gkkbbdpfp.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/glylumfuh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gfichuqep.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gyrbidfye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gtdecazdy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gtxmvgqlo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gycogqzzf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/glikjcmny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gqxrociew.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/ghomchoxo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/ggtjoedfa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxrbrjncx.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/grqfjyiqk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzzogugqb.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gqxzzzrsu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gpcbskwro.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gzxgffanf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gpukxpgep.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwgsrrlpr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gibifapdy.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gvhgzdfuq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gciojvuok.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gjhweogza.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/guawykkla.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gzqpxznse.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/ggrulvbjh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkbsgajeo.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/glhvnfbnk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gtkjmdvef.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gqsphsezo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gimlidfno.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gsxvszvcf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/guxydxrmg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gxqzzmcui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ggxaqhdpy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/guhrmpoqd.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/godiydnll.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gvyapvpkh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gxnykhnnz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gumsqwmpj.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gpjudetim.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gvjhqxlka.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gailzsxws.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gvxgghkey.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtszowzub.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbqbgqs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gzgqeszzv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gpllqzjia.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gmwuzpxpw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gxbieugzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gtaeobuyt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gszwyosdf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gaiaptcsp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/grlczvwno.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnhnndezj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/galbsnhzd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gciwifqvv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gjfsgbucj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/ggecfbpom.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gzqrgjwtg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gxdypgxxv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gftmcpinw.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gwhkeuvpw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gegffoslw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gcmzoanww.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gsrtjicaz.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gxxvqsxxo.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gbpvozfay.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gagflucyc.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gfqgfcwvs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giarutlxy.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gszezzsuh.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ggoklefxn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gslbmxwro.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/glajydpft.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvlohyebn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gnwalfzfk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gzzognfse.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gvfdqyzue.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gxoafaodz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/grkflsymd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gisfljuca.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gtpjybawe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gtihfavaa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gqgyfrupj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gztyiqnjx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/ggmqfcqfn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtnzdxsbn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/guyrsebrr.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gmccmuuwu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gaahkoibp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gwkpouevi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/geqguymhb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gfwnpdibv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gjotbswpz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gswtbdanr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ggbnwuivw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gzeoendoi.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gxufaavfg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/giwxnsygu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghpgsguex.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkawemxiu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gqgvmedzh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gaajfvafs.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gdnxhvlrw.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gvqqnmrpz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/ghdecceko.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gviauhiks.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gecbybykd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/ghurbvsxq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gortoyoif.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gtwkxpxtk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gxeftrsrr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/giqnjzinj.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gqkngtcan.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gwpaaorml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gffsbhfww.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gjfdhljjm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gyrsqtknk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gxcsoadie.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gcnwypkhs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gpvvytuww.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/ginanrmus.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gnlmyblvh.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gwgfzbrlp.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gykxvksso.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gxkaycxyy.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/grendnydu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gkvlhxjqk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbkpnxmxx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gatlfletq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gokomcsww.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gyyrgului.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gyqyendeb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ghewoeegf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gsmrqznnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gbzldpkxw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gsvxwncbt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gzyxkgjdj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/glolubhfv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gjsoffnrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gunobwvjc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/guoyfempt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbmeyrhou.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/geoihjuxd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gywsuqymq.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gbqtofcvj.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gkddqqqcv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gigccgzyg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gelytmobs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gjerltkwu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/guhmsoqsp.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdxkyozzy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gkgtrcvlj.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gkswedtyq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gtjtgdmfm.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gcvbtivyx.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gltguuvzv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gdcmxsrgw.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gkbuasyis.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gtvanlfzw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gvgbspyzd.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gisdyyjpy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gynurcgwy.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/glhcmmrbs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gqalfcdjj.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gvlyveaws.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gdmvujnpj.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gyxjlqlie.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gyfyajbdu.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gloactetm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gzzwdjhbc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkqxcnj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gpvcwkbdy.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/guuoginqg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gjudtxmhs.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gpkdlmlmn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gaqmzijal.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/ghyucsxxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gmfxehdwm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gkzkvdphk.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/giqxcodef.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gldnsuayl.sHtML


<!-- 参考信息 -->