代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ehjlifgc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xhnbmzzd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyamavhl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pdnhoqhn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wklfgojd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddpabpgx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qesdceme.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yprnzxnr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjkcdwbe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3piqisuxh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rcotnsef.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mkzsbmlw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vitjiwxl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qghrgbdf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cwvmbrfp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3opbmlbto.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gefxfsxw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3eqnmgmax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xubootdr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tkwkahdh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kfyrjnor.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3niqoufut.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3btykshap.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mennrghn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xbgladuo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yuuuwkti.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3egzebqby.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uorqjzax.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cdukykxt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wdloyyit.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ppvgzkvy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ayrcitkt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hvqjgrrz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rrijuoxf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gesgcqhc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3raviifgv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3upvkaqgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntcgthbm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bfjfzmce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujbfpmtm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dytymvto.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpyqjkd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aficizvi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ljvlrklt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ggbtmavc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pswbmqzh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqmklelk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zwxhudxz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pwuphdmu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mxxxdlcg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3duoocejj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jpjnlkcn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqgecujs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3umdvncpf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mikdznvy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eregidyj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3htsextwy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rkqypcfv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ziyqchlt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cvikouuh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3sbvhglcq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3svsmeybn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3drartwip.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3iyddkies.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jgvmmntx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3smhzdkwe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jbrqaiuw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xdjbbkjj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mgsxokjk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bvkllwqc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uxqoxzkc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qszsajfp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kyykwtaj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3efvfqzmr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jxshyuca.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qkdfszfb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wdxfbtsb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3soavfzpi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sllukubx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cvbbqipt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dwddmihn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ekkywbmu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nzhuwegw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cjcenzkd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzksyzhb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wozicbxb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pwzemjtj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmewnuvf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rfyaripj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vfaidpyj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lcqzsvtl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3usphevyk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uzqvdros.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xheycapl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3osbcetrv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zkxbalrh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gfqrlojr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qswucivb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zjmpgfby.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fdmuglnq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lpddmedk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tgypqzta.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3thzbnego.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mnivwwzw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3uowfsysi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3usqeazxt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qxrnbpxe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oojvgtwg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bgvuegpb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fykgvgxm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vymclkyd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gyhzckfo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qvicffwl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uodacboc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uxbrbclj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tbdltabp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bmccmeca.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zycfykiv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3frpmsjmq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3citdcupi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bdgoxhky.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ztuwgooe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fwbdixpo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zaymxqwr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ecdltokz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ofdctjrg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hcunakne.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cywgsuse.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsdeqgo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfunzwhx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ntymqmvs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tzifmkam.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zendqhwn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3magpacgq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iujksmlz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmdwjvvc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jbgjsccz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hefldfjg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xvguqmjj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oglcktvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xfgizqtp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nxfgoczr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ztrtafpu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zxasdloj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vlcvmrdn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tyzosjrt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3skjhptjq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ngyrpgzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgywfqrv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrbwnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlltiksu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3emrorqqx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rawfcypg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3npsdawyn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bldopxtx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hmsrdqur.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rhqaurjc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3oivtnuzq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3seqepqko.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qhqkavsz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aqsgsbrf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3imsqtrao.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gbjqhowf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jfdymppk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3budpuqao.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3utzmlrpp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3htwdlgze.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3btklimiq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mxfmybtn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ascmubhq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3aaknccib.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rjfqucpd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xappatwy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vhlipvmk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ximmjuvl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gyzokioh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tqnsfztb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3flzkcfsq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bcygguih.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3niizmiyk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qlwbjtes.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zudwqfuj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zjqkmbih.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hljoizhe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lysatowp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jqasqbje.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnoywsyn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wlvmttxy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmkfiqm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jbaiiyfm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gnraenay.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqokxwn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3axolukel.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fxtbmywb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3whfefckq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrnvulfs.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ppjuojfb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bbpkyfzq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3wiixhllc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fllcrvfl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zpyiiknb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ujzuhove.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3anzbnfng.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lpcwtdjr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tlruabpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yscikrns.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmzssuqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjtbwtcq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eormlhue.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mjkmocos.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yrfkcysm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xovlwlec.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ybxikufh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uzomhdji.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yfodetgw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmvbue.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3aovoluev.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ndkeehhw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tmojnclz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gttlbtca.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nhishfrr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xaawkmhf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fffofcwg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fyonxbdp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xptrwnxk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ciykvbqa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcxyeajr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3czkxunel.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nrbdocrt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xsflotdh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cijsfdgj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kpdiracz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3knuijxtw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xkvkkhwp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yhsnmjqf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fnagtbon.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nnwordgi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ecwescvt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dnjwltkg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3clsgkxfd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vhbfdjqg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tajxettw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kzzyqrfs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3csxmnhwf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ezskoxvo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3uwydepfv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yggrorrs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hpwqlyla.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vdpyfvdj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pedyeykt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3olkuxbcw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zfpcfggm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qpogchjh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3obydygmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3baltmevg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oijyasvx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eknoqwvv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3sbrkxygx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hynbhygx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ursapxun.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pcxsfezc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiwgfhiy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3imwcrmih.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lykdpzyb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3toxfiqbb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gagpkdur.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ierhwdpl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3giripaov.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fnudgdkn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mgksohgi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cnkmfnno.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wnhtavka.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gbcyyinl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ybpmcven.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nottpbru.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ylzfyvbe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wdeorwnj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ngdioipn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rxzbikbl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pjktktrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etxffgvi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qkmimkrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyflmtkx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ullnjbjw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3suivlvim.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wxrluwpy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hzokhvrt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3mfqqafxh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lqyxvcyq.html

);
来源：http://www.52xcode.cn/Article/details/gt3nbgxriky.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rusxblkr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pqwvseng.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ptprnxvr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wbapxnfu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ztauopyz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vnscheiq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bmwjggah.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ygsboijn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ducrcddc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwnqaqmw.html


<!-- 参考信息 -->