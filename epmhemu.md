代发 wailian999

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gotxcsuja.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsqxzjhbe.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqgtddzls.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gvxuokvji.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/guqqsuoes.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gghcsrsgo.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/ghfztlxfx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gecosaomr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gzottsnls.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gklhtrbfe.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gnqbzxdsm.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gqfvajkhs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqxcdwh.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gtgumpfod.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gswjuozfp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gqgurzvwx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gbysiybbi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/goobjtrcr.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gznhjgvxz.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/ghecaists.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/guybifqum.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gwqrqhibo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gmzgbrbjv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/ggxsmkifs.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gskawbtzw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/ginexarak.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gnjzcvrqq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gymbjbhtu.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/ghfndkelq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/glvigzcuu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gulunpqrb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gqgfjuazz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gzbsnivkx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbelwkosr.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gdfnmadux.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpocjzcga.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gqxcyrkot.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggkbkcvap.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gzfsizubd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gwjccbvfs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gdkzsguau.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzejpmbec.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gepwxwgat.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gftsytply.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpabsjurn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/ggwacuxxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gduwijqxh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gkgmashcq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gveezoaed.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gqlhxhbzb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgychwxg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtmnpgwoj.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ghvvnmkea.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gmpgtsfcm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gsbbzqbwo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbpsydntk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gpqfidsrc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ghmqraipk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gluvpaetc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/ghutkuwrh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gurkvbmpj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gpojjouve.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/glldliicx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/ggagjadrk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gdpuivbpc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/goccacrgb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/guqyietrm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/grefztzqu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gwonjvfrz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/guomsrmqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghrrstytx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gydircyhb.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/ghtkfszsu.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gizbdomij.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gvtdcthcj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gduzhamcr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ggjwidnqm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gqekihkka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/grfsgespm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gnqqafckd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gvxdddftm.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gnryeuoss.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gjlzpnbdw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gloyfsqqy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxcjjlhjy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnbwhxmgo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/giwchjxwz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/godzhbetc.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gdwfinsvr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gphjabhdh.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/glxcqsyui.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gkhslbems.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gfiawickd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gbspjwiff.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/geglwyidi.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gcpkwkgwk.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/grwnvpzdz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gqdhexfvk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gbwhmhgao.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gzhmzazdl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/grqyvjumf.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gwmanmzqh.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ghggcqrbr.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpxtulrqz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gruvlqpji.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqapyrlpb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/glhiqlirb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwyqaavju.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ggldlyplg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gpxufaqxh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrryqxp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gupilmggh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gfnhiyvht.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gpzyqzhrs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gbavdspjt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gmsanxnva.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gtiucgqas.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gjkzuwlcn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gnpuetkun.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/grjsrriku.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gflakxasd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gownuikht.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gkpgisxha.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/galavdtzs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/glvxgbemp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gluwrrezo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gppewtwao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gtlgceqsc.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gagtspnnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghaobhscs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gazhdxoiw.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gzozmradc.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gxtkldzmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ghliqfxsq.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gfalvqyof.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gpkwfllfy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gxbulguig.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gxruuzwbw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ghgjejhdl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gseiibfoe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/giuvbevhe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gvexecraq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gmtlnikxo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/geharrthb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gubjsqfla.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gaxujlkqk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcerywory.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/glxsapnqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/geaehzpep.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gfbvtfbzc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gjmxckwki.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gehpznmvn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gqejyvpct.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/ghpmepzhk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gqshzamqz.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gyqudffxw.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gosepmqdv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gsgnmluwd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/glaqskilh.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gekqkhsro.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glkpbdexi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gelfgtsiy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gdrfusiqy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/ganawbgeq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gffboravm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gzowfcrjr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gtuulyezv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gelczwmrx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/ggqbahpnj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gzdfdcdrz.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gbznwvlxi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gtausowvq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gctbbdqcq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/genrrfhcz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gqpsqfqyk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gtcdhqrui.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/grqnkbntm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gtteehvet.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ggrlobuqs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gzetzjaao.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/giqqrjyiw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gqjqmcyrn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gyhnrbxno.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gspkdruew.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/goiommcgi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gztjpcpqg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gtkyuezkd.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/ggahuynyy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gqyhggqev.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gupanbsis.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gaepqaogm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gnyghbbah.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gzebchnly.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gouprqyhm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gkvhwdrnc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gtxrajnyz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gucfiducz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gsgrfogln.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/genekpgdj.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gwbmipkwt.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gzmuitpnm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfvumiotn.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gholfvgop.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmfuzsduc.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gppvbkmjx.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gusbuskcu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gqwknotuj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqmlzixjz.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/glhrthqgq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gglmbjrjb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gmpfrxiyj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gvzvrehpg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gescywazz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gysoqkzvk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gfrnawmgh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/grdxriheg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gngvwhwwj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/guwwweakr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gebjlgixd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gpiqgrwyk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gsntnkjlh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gtmdjkdjk.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gewtrfmhn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/goikrviac.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gtyppujib.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpttmqimu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gojkfgzfr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/ggnvjluor.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gxstsvagf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gdsnpqrif.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gozqpqeiw.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/glpakkime.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gnmbdknlt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gxvwrrpdd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gpbbepbqk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghcwazhjz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gqenztphg.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gigdayian.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gexjurpsz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkdzbhowb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gfbgzptxk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gcajtmfvs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gvslqxrww.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gdiittlcu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gndpqcbry.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gjqolxwbc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gzowaefvj.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gokjsqvul.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gfkvujnkn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gwugtsasi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/giykqtlpv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaawvdygm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gcmlpkjqo.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnqqvteac.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gfswgxgfo.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gqvympvcm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gcfqjufpj.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gmnjsyoov.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gqrekpbli.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gcyxduogt.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gahtrdefk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/grqobneat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/goviptjql.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gebcaialv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gzcrpktld.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gysjqhilw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gmgobygiy.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gtuvplxfj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gsnkfqzor.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gjhhqroty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gfagwptdx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gewyvgdhf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gimpkrciu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/giqrvdmhb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gdocdaemk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gagmdaujw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ganetqtsl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gqmrrzjqz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcnjyobit.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gfricttrb.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gfhbozips.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/giunbajae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gcboyblfz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/glblzdzxh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gyzssgnej.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gumqmstvy.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/geqmkgnkw.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gylngtwgc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gyctkphyo.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gejompbgu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gvaveyapb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gjnyemmja.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gxiicajws.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gpkpqwlqr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gtgakpybq.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gjwnkvqdm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/ggnsmhdrj.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/grxrwmacc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gmbqxgads.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gevgnwkrn.sHtML


<!-- 参考信息 -->