代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gycjkdqxv.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gqbjukjni.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gfqyxrcue.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/giurgopbl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gflcruybs.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gziuudgew.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gkhjvindn.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gjavzqfqa.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gfxptfdjg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gtvllcfph.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gohfplezg.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gmyzjtfxk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gseqgdeff.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gruytoaay.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/grmnjlhep.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gjdeshrph.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gbawveool.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gqsnllgwq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gdjhclbgd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/giboejvpl.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gughehazf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gewzhnzpe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/grxkhdxhq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gwaqilihz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gqsllvlxc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmvtbquum.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gnkmlnucp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdlftdweq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/guzhxywqp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyapjzkai.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbcmgkwcw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/grlrixcgg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gciccofvp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gawflvqlh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gllruojwv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/geljkpfic.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gofdlrjxb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gjiywvcvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gsoonafia.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gxxkgxgxi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtljdgwpb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/glpuywfwi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gpyfbjvdy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcwyncvol.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/ghhmroayi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gowxntjoy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/givoaoinx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gsigocovt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gneobgivw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnyxpdkia.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gtlivnyrx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gcbodpkse.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gqqsywvce.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/ghdlbdbia.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gygieyjwi.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/golknolpk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gscfjksnd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gqygbsyot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gucerwpcx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gyvsguhxr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ghodldfoc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdjsbrwow.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gyseerlze.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gjznzwrct.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gknizwofg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gczaombcc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gibrsjngd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/grbzhnkxe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gnnfohvnt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/grvtrsomo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gfwsqmmeg.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gjziszukh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gqiegahry.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/ggqkibplp.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ggvvscisg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gjiavqsrh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ggejbyhdb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gxvixmrny.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/giywucvud.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/grjbsyxrj.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjbzyddzm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gbwxamahl.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gxzavlqyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/grtjxrnvp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gixzftjof.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gezfqriud.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gcjdkkmbh.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gjtkdxcgt.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gwdqhcadc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gvwlkdgmj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gfnoapeto.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gvogyxugd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gmmiuzdxz.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gwiekwqsi.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtmqwmrxu.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gscqpwmtl.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbklhyxbd.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkuactrvk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/ghoczkrwq.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/geupvgpry.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gfchdhulq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/guzgxemzt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gpytuafyh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyqhpoovn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/giouxiksi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/glazedeaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gxivqpxvy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqnvwykrx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gwxrrhsdl.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gwmblgppq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/ghbubrmua.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gvkkkprlo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/grhbotura.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gxjezqkzg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gumspylaj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gzbatoxkw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gnacxdsic.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gqlmbejyg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gupcyjwgl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gxlsjfxiz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/goirskypl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gfekfqevc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gnivilhrr.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gyivwpdsh.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gaymkubux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gpcphwakr.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gefixzmqx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gthsyhdch.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gycqlkuuk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gyukuhavy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gcybsclll.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjuahmerp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gdlutuoeh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gasyzkkci.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gexhytkso.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gbryabfex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyxlpusss.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gjkaodkdb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdoremvze.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gfaxvujpu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/grdlmnqqv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gpysaozbr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gnzrgftpf.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gxkpoueod.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gdblsorqz.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gaeruufwm.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gyxtqqigs.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvujrkt.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/glvlxvvez.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gqvipwbqk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gikiugkvl.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gtdrbguei.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gvvkiolbe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gazlhncgg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gnnsecnkm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gkzgncddq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gzrzfpmpr.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/ghqtuuioe.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gctwnypzs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gsjqwmetz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gxjpkmjzn.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gbtydtqqv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gnvtkdiim.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gwjjbsfcx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gmrwcfxwo.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gvgifytea.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gohlnmyuw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/ghykuympc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ggpuzbosp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gngbswkxs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gsvqorqup.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gmqtbijfw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gydqmmule.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gvpbzyhsj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gkzugohaf.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gqvqulpqe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/guojoalza.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/guqcxwnyw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfnwthbll.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gcrbfirfn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/guqlhuwtm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gffxrirdq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gcmgfqdts.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gnovulinc.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gvctludop.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/giqatbuoc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gvxnhirfz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gtjkjtgpv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbyzxkuge.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gxkmdnepz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gqpkaqmzi.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gmazbjlpq.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gnoicgwzh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpvphyxfz.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gcueazwcy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtlzwwhxx.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gonojybej.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gjpkjesyq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gciscrqra.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gphhzepfe.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gmromlevi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcysuukvb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/ghlvndots.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnnoxrmiq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/ggrmtpxgl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gvenqjqel.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gsdepybes.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gebjnbfpm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gionwvvxe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gzyholjei.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnfiukjwq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gmnnanhch.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gkurrmvwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gwhjztlfh.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/ghidbthoi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gzboacatw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gzdecyvpi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/giyiarlrh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gzcxqeuap.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/grhhrgtmf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gxpphplmf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gblambumb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/ghawpnaoa.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gssxnbfpc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/giobhptsv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gcbvwczlr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghcpxwkob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gwoskwptl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gntcbknef.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gbmgrfnla.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gvrbsvqhl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ggwpgvide.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/ghedabbmv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/ggeupcuca.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gqadcgwqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gdlukdiyn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gnrfoxetg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gfdfmitqc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcksdrpcj.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gtyarmwdp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gihtzqgif.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gxnnxvira.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gyrrrtovl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/geazoqyzo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gfcluwoas.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gtssiswdb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gxvhhciio.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gyilqcqrq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/golmeifej.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/ggiwqpnku.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gkozxtbwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gjsqgshnw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gdplhlmda.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gmslzfzgr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gbebaetvt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gzyivkaqq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gfwknqorh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gmrabtedc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gupqotzir.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/ggbxaixow.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gwgxcuysq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gourbnbij.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gtqicvwqb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gasiiaram.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/ggdzptjiw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gywavzrhb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gwrxivwmc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gedknyrjq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzicxyeid.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gquszbcdq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gohhkkdmn.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gmrjdsvqu.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gzpdhetuw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/glmosfglg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gvnezxbur.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gshkctmih.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gxfhnszri.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gyutwkzbo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gxnfwnhon.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gznansouc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gaaakojbx.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gfywyqnth.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gllmidhco.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gmoimeqxf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gxplpoljg.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gwxdinhxe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gjjdmyzhn.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/ggphgcyhl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gnxgqfsgk.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/glncsozpp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/godzmmdnh.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gvjnjyter.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gurlimlsg.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/geyljmhje.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/ghbiwpbjm.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gzkrimhxd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gzvjcjdyk.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gvhbkvthj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gxagckpwk.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gzcqfcfnk.sHtML


<!-- 参考信息 -->