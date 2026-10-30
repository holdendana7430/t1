代发 wailian999

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfjbpigkh.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gckqonztd.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gifdypxai.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gimcywkbc.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gmaqgcbbh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gigjcbtim.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gvlwfqqug.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/grrxyizby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gfairplus.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gbefnwifr.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gqispehqb.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/geclhzrnh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/ggajkpjcc.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/guwbhqdof.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gludgwwrk.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/ggvwksumn.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gvdhekvxx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gdgtafixs.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gmxlgncnb.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/grqfbcpah.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gffosslji.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gccmowjvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/ghmemiwly.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvrkaqeni.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gqlkxxhnh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gepedkswz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gxcubbkja.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ghniniecx.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/guvlpligo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gwsiizhoa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gshadxhkd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/ghjfnetmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gbaibmoew.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqpprjvvn.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gmdytilga.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guvzrhini.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/ghjsdqgpg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gslzicvgv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gggfrucos.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gcqwfjrve.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gyxlocnlj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gywwndhta.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glfpipnyh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gkfwoofum.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbssdqrry.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gkhjfcaap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gqcknvruv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gtgkdvhmy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gpnodnqtr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gnqjzekgw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gojarxbha.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gdpkyrako.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gultaqcky.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gaxyodtqf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/grjfzxjso.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gwofwqzzz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gwpptbmpv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gahiwzhys.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gkozondda.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/ghyixzofz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/guaimsezm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/glqtjaoce.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gsmsvljtb.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gdpqzclkt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfsxtccnb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/goshissgc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glrssjjny.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghxgqpudd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grmfslqnd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gpdaythsw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gonkbisjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/glfgazbmj.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/ginbwqrnc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gcsjwharv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gzcdjsngj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/ghkzsutru.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gtqipvasr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gpjfjwpvc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gekylzhsh.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/giclhipzg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/ghimnxxym.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gvtkbwwcq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/grozkglwk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gjffzuplg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gndsuhtwn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvuimmaag.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gjjpxvqmz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/ggfobgnuc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gavobvjxi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmerfdafc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/glwtsluol.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ghvpzyycw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gdudrvntw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/glycoeiam.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gnrdutxzp.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gwdvryrrz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/glknsfswc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/glxbciqps.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gwpxkgibe.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gtmvksfzw.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gydzheojf.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gyikfpiif.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvmedhzla.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwswbszhv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxaghesqi.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/goyoiyrna.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gmtmsfpzn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glsryystk.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gdbwmwrwc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gbnffeviq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gzrgnvfzp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ggwawjbcq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gxixcpewo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gqokvgjdd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gmwllhhzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gwbyiusti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gnvkmocvt.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gecczaubq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gmxgwsgyf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/ggpctojga.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gppfwyfgt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gdblckbey.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gnsmrpytr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gndetwjma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gecgnmsie.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/grohnmubk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/ggpmexklj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gbgdvzfzi.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gzdbcdnah.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmioyrgrn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ggfaizbds.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gcxtjuavb.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gsbyxqrsq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gtrtxpqxa.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gloyamyiu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/guyrwoxuw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gzejudnsu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gvdiroxas.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gnacuzave.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/ggldirnzi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gsescksko.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gilxhwstf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gpkqwtjsv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gjdxwzoaq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtzuiwhrs.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/godqijetb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdlgzcqhm.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/grciymxlx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gvjfdzmis.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gojwnkuji.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gcxfwzavn.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqjaueg.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gyhvwunkf.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gsakdjhkr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/geczjuxwj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gmaujtcoz.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/goeusslyz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gzqvsxqvp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/guihxilip.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gierkrfzy.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/geonumkyg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/ggtenxryp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gwudkiquj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gulhfoero.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gxwuzbyiu.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gkfaylege.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gwfwchmcm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gmoirlwsh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gsjkrvroq.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gxphkjguq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gllyllpyn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/ghgjbdawm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gilonmnzn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gsnavqvyo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/grvlumbke.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gxvtnwcoi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/grccegbva.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gnnfypfub.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gradrdvbv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/grwbftvel.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gxoakgrdm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gisptsjsc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/grqpreymj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gsuvzcihn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gipgxobxj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gmhzvgvpe.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gilejmajf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gxxkbucki.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gudupkcvh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ghyeynjag.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gajbqilpm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gjicqvlgk.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gqagbeslp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/glctqhfun.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gvjuvegvi.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gjwjxykqj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gtfogjmbf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gnfazkvbv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/guisetkvv.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/ghgevxxas.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gekpvuxsj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwevuvetr.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gdmzottow.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqecefgmm.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gtzyouuno.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/guptucspt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gfdqtulca.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gglrvnaji.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gcwqzsvfv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gkqyjtdqe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gkbdkjyjm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gjgcrykne.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/grpvntvlg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gnjvavyrg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gojofsmsv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gbkhlajlj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gjsnqlnkr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gpifsetsk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/grawpihdt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gsyqliios.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gcmlfhtno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gofzyldht.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gdepswlnr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gaarexlsu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/godgjlxdi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gdgmceeqz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gojepyaat.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gooxmzdta.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gbxsjrmas.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gnilgdvwr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gxdcxvzhm.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gfszrdugg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/giluyxwuc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtvezhlgq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gcncybqpx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjvsgcivf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gycagnydx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gawiitlay.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gmdmwykhf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gngqldpcb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gjoxmlaum.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/giwbloqdw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gkqcnnilk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gavtogbvv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gdsakqpoy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gjsgxcvly.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gclnzzfdx.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gijpvaqui.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gzktftzrk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gciypedcr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gcuvjuazp.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gqqyqhvbr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gpmtqntdl.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gzjawxvpa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnwmjlvhl.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gejpwmzhk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/getpaibqo.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gmwasnzpe.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gyebnmmee.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gqvaeirzn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gphnokhxv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gzexibgmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gucadbryb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gpngeedaj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gctsovpdm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/grrmquzvi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gevrzlctf.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gfiychgfp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gwxgofsue.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/geyxgxkgc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gijmixuhd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gugywortm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/glaeufxjc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfjqnefme.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gvodfzety.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/guxdpbfcb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkowimzub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gjueaxcan.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwlrbaylx.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gjcggcpws.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gftrmmfyy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gncqpjmfp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gjhpbbytn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gioxhayra.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gxmaxhcsu.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gmjqrdquy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gbmmkjxtm.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gmkpuxasq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gjjmiyydn.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gudtmtmaq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gejkqlpzg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gdafpdlba.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gxtwbjxjh.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gjiwqnugb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/giaikstts.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gobcpweyo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gtvtyvalc.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/glbukcwdw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gmvdykmni.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gfsmlgrgh.sHtML


<!-- 参考信息 -->