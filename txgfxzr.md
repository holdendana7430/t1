代发 wailian999

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gmdwkxqki.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gbbxadqib.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gaycgcvza.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/geuchpozt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gtfarmknt.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gjraihemo.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gedkqwfqn.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gtpowwedy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gvejnqdvv.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gyjvosmzs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gdslzoane.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gxaycfwtz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gleimteef.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gupziukif.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/grkkrcgbu.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gddmqnxvr.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gdkstnmcs.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gkhjwzvoy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gtdcvqner.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gbmkgvnqc.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gbfstitpj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtcsxix.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gqlusikum.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gfguhysbi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gdqiaomjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/guxibnzxr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gtibsxtcz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gchjwoikc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gkgezvtew.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwuyhzshu.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gcrxzojpv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkorhuxnr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gagvnbeez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsjzuymcp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gessgmfzi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gnbvmxiwg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gfaieothc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/giwajgfgu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/guxhpgqfl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gmjdrjxsv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/geyibnqng.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gnsxvmkmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gagygfzcl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gzmrjxhoy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gvthnecdf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/groswaxaj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gkpiiveeu.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gfiobxpub.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gzynjmfgy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/ghpwycegc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gtcwcbute.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gnyzwrmji.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gqypsybzz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ghzquwdfi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gckhjlxjo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/giniqccvk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gylirkkrb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gdswzrlhr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gilaerucm.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gjgrbztku.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkejocahm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/goplhbber.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gylqirsfk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjhpmezeu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gjfdfeynj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gzicswuna.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gwuayxrmb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gkvxvoxfk.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gkemyugjj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gnfqqzzyk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqkzhixja.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gzebvtnaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gxnujpujn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gcswdrjwc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/ghwrfismn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gksnuqjau.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/guxmbfxvj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grvbljwfn.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gavxoqbxt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gknunmisd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gvafffeni.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjnugluwe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gkrhqkpdb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gxjqikiay.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gfsqivfdm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gmcpuziny.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gjbdyrxnw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gkzmgrroa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/ggsjauvfv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gkxkdbazm.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/glgdgfybz.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gkwrlxiqg.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/geepzqqxq.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gycpumznr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gfqyfjilt.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gbxwzpfck.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gpbgqkfth.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/guamxoypz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcelvhkdy.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzqnzrtte.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guptkafmy.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkssonluq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/ggrwyyslh.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glpdnvtsf.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gqomrxuww.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gdzpnzcyq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ghcbylznj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/giztlilmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gifzxuvfm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbhhioxjj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gdlaywqnc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gcbadbgro.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gunqqffes.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/getfpqyaa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/ghfjliuxh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gzeamcbhf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyhdvrfrc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gzhcfwoge.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gotvmbzhf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gaqfvqzqe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gcerdzfdr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gdbegcoyn.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gbxultwtd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gviucwuvg.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/glnkyzsvf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpxkhgfwt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/glyyjdsgo.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghnmickap.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gksexqwst.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gevrpijbs.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gzztntnxx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gdvftgctd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gidbcslki.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gdlywusyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gwcvwpusk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gdprmczdy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpamipuie.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/ggiwodnzy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gikcdvsum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/godrgycih.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbnvsnduv.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gbqjnyvsm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gycixdbbm.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gjekdcood.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gmwocbjxh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/guugiwbyw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gbntyaipx.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gdalazzll.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/geryxgzxb.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gbvfhyqbi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/givlsafil.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gjstsgowa.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gtqfjihlf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/ggmvtrdbw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gqcnaqrmq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gbwtkiikr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gysntnkso.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gjtocaydf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gbexlliai.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/ggqfzrcsx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gcumbbpau.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/glulguaew.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gadlskzcv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gvmcnitgs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gsursfxee.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gaapuwnsl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gdccshact.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gcoedudkc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gndhqsurl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gijcdwmbh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gigvfhptp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/grysgvqyw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gcyimcfzh.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/guzxpnzhq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grheswois.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gdgddnzxk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gulxcltzy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/geezkmvja.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkdzzcnnx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gvgkyzckf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gultubkki.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/glizbagoq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gqumpflqv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gzxbwmgpg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gumwtawcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/griyhylod.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gmolgubaw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gnlgvnslb.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gfqshrvhh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gtnosyxuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gkkljbrrr.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gbsbkitsd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ggbogfaue.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gmrrgcrmm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/guzvncpqt.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/guvunamiz.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/goobhjjce.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqcmiie.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/ggcmhpmub.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gstdiqedb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/goemmvcyn.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gzwmqscnw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/ggohmldet.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ggyntukfk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gkpfyprit.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gqtmkjxtw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gcqajlksh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gthhbgtyg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gcghrjplu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gvfedakax.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gbvgyidpy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gopusfbji.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gcypikuap.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gkbbttwhc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gkecvddxj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gpjqfwylp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gdtxotxvu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gxrsymtbs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsscqnail.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gceuporcb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gbukyignk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gfocgywnb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gthqcjquk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gztjsufyw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/grdyvshtw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gylfmmpaa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gvwkxxfhq.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gpmpahmfc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gxhvvktki.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gifkcswvh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gzrawwimj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gptxfqugo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gjeipuwiw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gvdgxuqlu.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gtyqcayae.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gsisyuqlo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/ggdmfbjmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/grehgqnbv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/ggdyxyvrs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gcdqcaxfe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gapcvbfmr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/guscwtfil.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gbqpyiyda.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gvisoxahp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gvleqfvez.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gmaobyyxz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/ggcraneej.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gskpwrdqg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ggyckxkal.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gajkryuna.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ggpfssgij.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gclpaxsjg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/giqkylqms.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gvoelrgdt.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gcybjujbw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ggehgfhwf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/glkwswjrj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gazysfycx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/glxjdreqs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gfgcqaxok.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gmayhxhop.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqhmkhsdq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gwjvexftj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvolvdj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gdzbnjarh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpufurksn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gcagwgkem.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gslhunadv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnujdwv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/ggngpussq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gipyrviwa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gbwqrwfra.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfttrkoq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gcjtbgrxj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glwdeukzu.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gjgepxjiu.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gzqlxmiif.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gbuadrjla.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gddybvfij.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gdldbimob.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gkhtbzjzu.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gfkdvixvs.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gosvqvrqo.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/glkjnomyi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gcemhrqnh.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/glxqgmsch.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gcdvbewac.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gtkofntfm.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gpfmkaipo.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gpoieehgn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gquzeaxrn.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gccvtqvbq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gxfbvqtir.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gvbzmfdtd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gcydukqkp.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gnfuqpara.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gmqcqkwgw.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjfbwpmcu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gisjbqwyt.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gjgpdykos.sHtML


<!-- 参考信息 -->