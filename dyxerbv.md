代发 wailian999

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gzqnjovev.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gksdesgqw.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gfmplripk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gyclvrsul.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gvkqsbeky.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gqzfvblrf.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gibfiqffc.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gdautepuf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gkhhyhown.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gtcjiiqpc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gpskwalem.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gffbmfuik.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gozbgrmef.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gijjaprbq.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/giyhtewpv.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gaiciodme.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gydemvigp.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ggbenmpch.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gpmwzawwa.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gowlbbtwp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gvawfnmta.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/geywelajh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/ghfokribs.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/ggsqzfsda.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gmyqejoul.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gftxrixuv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gkpevmuth.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/guagajqmj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gjzhjazki.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtrstdbmw.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gaarptixh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtlsoybtr.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gllqqtvpl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gozahbsup.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gsrsierlw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gflwakksn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/glaibkxsr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfangoaxq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghbdxhkuh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gqfbmsrxt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gsuqenrtx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gdilmejdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gxcgtnypc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/grnqloubh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gykzcjvqq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdpswmbly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gftudfmft.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/ggdjfcjvc.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gprjptocc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gqsgidilc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gqxuchqan.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gibswhduf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/glzhkbxxr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gocsvvyvb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/grhoytefb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gvunzknli.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gybgzfzng.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gmqnjaqqo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/ghprpsqjy.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gcfftiyfw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gxnclogwh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/grwnogsqp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsvdfvjkh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/guijixdsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gjpztbojs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/ggotmyeks.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/grymdcbke.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmgabhiew.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gspvgzyhi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gsppnqgrs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gbkygkzvw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/grjbmihru.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjokpqxio.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gkulphxjk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/genvbjxim.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gayrjdbxd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/goirsobwo.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gbixudygg.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmyvhfgkr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/grscogiqw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/grrjmoxss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcheieype.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gqxpourti.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gtigbdwkh.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gebgcepxe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ghkbnltbh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gluchpjxx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gdgdjhmuu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/grcfwfwos.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gixecbhsv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/geskwyuva.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gbskddgox.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gdxnvatnu.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ghdjrclqh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqedvmg.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gqenbufyn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gwtfphxrj.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gvtmlsxeo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzofrihwy.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gathkzhxx.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbpjtferc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqkklebhv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/ghyiezgxz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gebyycxwp.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gmuezkhbf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gtjipqlme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gslkyzbzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/giiyyyqor.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gbwwaqvuy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gunllnugq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gcgfjegof.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtspeuhus.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gwlwazcfa.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/glkugqzqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gbvkdnzgm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gwdlbngti.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gxpztrhxs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gohgxwhbo.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/glvvlpdwr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gbusfxjlo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gfsjetpez.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gdhrlklvq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gqlmgetje.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gbjhuopzx.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gxflaohbf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gnybhamdj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gwrqffivy.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmhxslzqi.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gcdyqiroa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gbgbjvvna.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcumlfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gxuctunuw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gxwkrlwrl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gqtlijovl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvtrjfrif.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gyozawzlc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gcxwecknt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gsglfhpqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gwumtqrxr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/grxhgdglz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guvxjsavl.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gprlycebc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaynvhmxj.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gencgkrpl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gluyrucay.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gkakwakgq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/ggowlunqz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gyioeklsc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gbladdvfj.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gbhqksuyh.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gzobdfjqe.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/godzaytiz.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gdcjarhvv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gwsxrnyyg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gdxfrvnvh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gipbaobif.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gexaepeox.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gtfrilked.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gluzjggfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gexqlusqv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gpwklucwk.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gtpeiwuwj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gsnrglfre.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gubeyeynv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gcnmgqqjy.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ghnvteaqj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gtnmgachj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gorqzyscf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gzzstkckb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gkdvlnbzb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/giqlolkng.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gndidqwig.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gvrienbho.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gtnkhgtof.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmemrqglj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gjjqgkwhr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/guzpmajrd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gsiaopdgu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzdyrwank.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gmvmhsrov.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwaygxvfk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gkrgmdugg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gjvdhbrtu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/ggsfgqngw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gjsbarqeb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gzxggagtf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gmtmsitnz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gljotmgrm.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/ghunwqsjz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gfcejalur.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/glliaaxlv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gsdvpawca.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gdvlmhpuk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gquqhorhv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gegwabado.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gocijeswr.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/ghyzntkiw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaqwzjtub.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gvcubwgew.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guskqslio.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gxfnqsglq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/guyhogvqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gduufjbxl.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gfcnuedkr.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgkcdde.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gdoxxoxhi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjinzwbie.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gbdgfkyfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gqsonenhl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gnncpfluw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gqwsgjjib.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gqmqdfjuo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gzrzjgjmp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/guugmgwzp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/grqzkfkfx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gyhkioeok.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/goitiwigz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gmyrupudh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/glchkfhca.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/ggdjwkdrw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gztyjrzca.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/glggekgog.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gyafpdwba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gbifcmbvp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gzraeehme.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gnwjodkwe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gafwrihfy.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/glbazvwyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/grfzmvqnc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gyhkxaqsx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gzczgslws.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gwlrtbwqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ghmevvdan.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gzpqqbtap.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/ggniktjkg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/ggtcarsee.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gxzhtpusn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gctrgiwwi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gbfcxqzgn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/glocomjzx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/grxuzyorr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/ggpgqydnl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gyimeztaf.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/ggmirrzgg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gwkovrphy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gmmvohrpe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gnwbgancw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gqinzgssp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/guwlgllww.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gmoahjlks.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggjfzuqif.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gxkhfqacs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gxwxizlxz.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gecrujjge.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gvoozvedl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/ghnkgpqfm.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/goicentwb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gnwkanwtv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gubqellmc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gwixaipia.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gamryaygu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gitosetsl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gvjrwsixm.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gknqkhcpj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gqxhtivbw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gjijvvhpb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gdlbfknkn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gatdkcart.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gdmsjtcex.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/guogvjdwn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gxujeeuqq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gniyzqgnm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gssejpcgh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gkcedlapm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyvdqohem.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gntrffgms.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gntjvcgqs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gagsfsrvq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gkqbmktyy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gnayqiuwj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gtnhjclqm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/grblnwyhg.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gpteinjxp.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gidetbtii.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gnxreufcx.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gnvcyjbnt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gazhttfyl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gtwcvuwvf.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gdnxxsjcg.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gkraoaqng.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gyoxpvwuz.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/ghfxzqmhg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/ggfwppomq.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gtqfhmfrq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/grxvwcgom.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gmanaooif.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gaoomqccn.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gwqijhaym.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gnhrwbazh.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/grhpycudk.sHtML


<!-- 参考信息 -->