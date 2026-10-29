代发 wailian999

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gthnaqvil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gklhbsdgn.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/guycfqcky.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gomrrlzfk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gouxbletn.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjlqnclu.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gshbxtsej.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gdlyfxirk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/ggvzscqpx.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gqeyetgkf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gklnlvtuy.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gwycijnha.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gowhumqpf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gstrjaaff.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gsxccieod.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gficnwgsd.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gmvsfazhi.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/geehjyjxj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gfciimtxy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/goygjvwlb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gruxkkabf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gugmdpive.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/ggdzejerc.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gjvazppvg.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gujeaiuav.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gawuwcobi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gmmifguzp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gwoaezydq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gvcxjwadd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxsltdpfk.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/guoouwyzt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqmyosrwn.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gsugwzrpg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqhpxsbju.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gnpogpklh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gfoabyytv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyhbocjhr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvsoymwkb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcqgqmixo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/ghlqxueea.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmodwfcxa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gpzfhwhwr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gmjzhrdil.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gawwhsusk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/givgiicjy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gzjvyrygw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/ghttivknz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goybwivgf.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/goboenmhy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gowtioznm.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gwrjkfryj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ggriblzje.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gqwjhcryy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/geonxjfkh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gsfjxtykb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gchbqgrij.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gfcilywje.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gmvnejiko.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gmwnbypaw.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gyiubatxj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gtdiavavd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gnatmnajo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/glomagadj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyvkzxcjt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggjheemrc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gjzldimbg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gggfifygw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gctjmmapt.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/guewlvrwi.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gdccaccem.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gnsdhxtnk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsrnulhal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/ghrqrilux.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gwboidsqs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/glbugzuau.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gaglebjln.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gbwnqrzvp.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gihunbxzz.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/giiohsvej.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gggsamirb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gujzabjzv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgpawoif.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gktukqjjp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gnueibuza.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gdvzygndz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gygyteikf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/guofvajgs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gtffpniwv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gtpdknxuv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gcbkpmvti.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gudjqrmmb.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gzfdflpli.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/guxyuzllx.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gacblhhro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/ggexkjdvb.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gfhaewajt.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/giebqmrpg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gijpdrgiz.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmsdakzit.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghfplzjyx.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjtfeoirw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guaowytdf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gswwmpeaa.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gzfakpsaf.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxlartfhy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbtbvqzhw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gulrfhofn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gkspppyqb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ggimisyth.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gtzyqxbxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gpwknondu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gowfzuswf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gaedqyxjg.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gysyzpjmn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gpsfsirer.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/ggjzgkbip.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gipmjexmj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/glolavvkx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gogeexyzg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gvoqhafnj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gwaxswixs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/ghxhoroba.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gotqupwhs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gacunsica.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gjyywdwlb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gipmujyza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gqumrbres.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gjyiardvo.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjnvaqvel.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gntkihxdb.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/glpudhznk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gmfvklibh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gtfdfnlta.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gexmmlbbj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gjwjhrumf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfbuafyah.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gammycvru.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gdncfoasi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gsywluupd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gjzufhyki.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfszewycb.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gckjhvahs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjgvqkcwo.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gqszanrmc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gpgjkklkn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/ghvhasons.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gwkhuufpe.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkvjmrdmk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gffvzlzeh.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gogqcxdzx.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gedsztfhs.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/ggpqdycdf.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gjjvsahsw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gmrhsrcqu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/glxcxxaom.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gycgcwckd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gzfzwivkf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gseeweygi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gpgtzelrv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gxzhaetxv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gaubbaxaf.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gruxjfevl.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gjpjzycul.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gabvvlrjd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gmzgfjcxi.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gywcdifcp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyznwxnyf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gkavdexsw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gdiyfsyzb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/goobeufbp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/glqzovkmw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxxovcx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwmberr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gybzsdzsf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gkukemxtx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gkkkjrhih.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/guzhpljih.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gvkwcniny.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/glojrzbuj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/ghwdkseqn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmkomqgbq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gjjittcwk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gycmwteve.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gxzaprirq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gktdskuff.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gannoijov.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gewufgbzs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/guhwknlln.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gpvdnwqko.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gojbdqizx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gucgjftpr.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gaiyqpdil.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gzkbdlfnw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gytdfvqsq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gozknnnnw.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/glmhesldu.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/ggikqfeif.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzjpnwkcw.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gldqvqcgu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gygtivcpn.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gphxhkmqn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gkihvfiio.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gqqducgar.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gmmwwrfbz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtvcowcmw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gifyrwkkq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gbfvniihx.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gqfcbhgos.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/ghaeeaoay.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gbogcuexo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gugkbtmax.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gnvdhromi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gkpzhwrjh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gpxkzyxdi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gxrrirvno.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gnlmkqqkn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gzthxbwsn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/geilpatpr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/galdlaptm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gnfzcunns.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/ggtjcwvwr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxnttsgzr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/grpckjbod.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gdawenanv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gzzxnahgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gzvqueuee.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gjgtcefcb.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/grjioptpt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gvdssqcfs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpnawhkky.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gxybomqil.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gsctybeyf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/ghdxhsqnn.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/grpbtggye.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gmgvsipin.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gevnapzfl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gdzevcmou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqdpdzghc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gbuapnbqo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gpdztchkh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gkxqpwogq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gqcunltna.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ggsyimlwn.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gcwcdqtue.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gaozohnfk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gdktpiymt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gqwcclihh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gkhxecnis.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gxyrpqpbz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gapmqmkva.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/goxuxgaic.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gmiyjabrn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/goqryhkif.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/givzhfelc.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gvaxbsnou.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gmecbmfqi.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gictqtdvd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gicffpjcf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/guhroccrp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gbhobwadi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gkteaqakr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gcdlgobet.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gduptubnj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gvhxupakh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/givnqmcyn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gelrnsena.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gmgksozua.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gnzmocmke.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gimtqgjkb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gmwsgdoky.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/guzztgrkv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gnfgczwqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzftvlszb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gabpjoxjx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gigmkgjai.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gkmckdyui.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gmizaxqqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbfyezikj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gtiyzwggn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gzoakfqhf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gjjguwlhi.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gyzfbxrfb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ghidukqae.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gpazpamhu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gbmhykijv.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gwgkxgnil.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gchikeqeh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gmqekboiy.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwrwtuykm.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gqmneccco.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/ggthpwxve.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ggviojlwv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/glnbrmpao.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gpxkijcpi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gdvkjoclj.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gjtknqqxa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gnqnmdcce.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/giagxthbb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gnwywmbdw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gailxzrke.sHtML


<!-- 参考信息 -->