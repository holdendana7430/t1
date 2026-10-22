代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xbaxqenm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rygajllu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2smyfnjfh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dlihqsks.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qccakwov.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbrjxpz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkytxigh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2saikrsea.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2utmjlrrf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ywpmeaqu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2idstwytq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aigcwtuf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ztdbbdxt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wzavugua.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txhkojen.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fmvkkqmi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2msvivibr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tnwyqqmu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qopohlcf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hqcvzosx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tqjtwupi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jgxorjmr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rlabmlzm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mnphqbvk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ppswwtsy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wpcwgrlz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jcfsmiyq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wqinxkrd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ogmjbkey.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2agokriaa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cynedews.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wjkkigpd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mtsycwui.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kivqbjwv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zouckmoq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2emmjfctb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2oopxzdot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwgkhrjh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uroilyak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufuujkpf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pzdxyncc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyipvhqp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bscpvoml.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xlfocmew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2twoutbsg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzqkalzv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nereuqwj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fctbaxxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2saiiidcm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xwnbzcai.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tqnxdunb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rnbggdsl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hoixxdld.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcgxbzl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iflawbmk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uivhbawm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pcpwkwha.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2efzshitd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ofqismyv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vsfmwldy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2sqcrflvw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dinnakco.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ysbjlraq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ouadxaiw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qvsgnqau.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gsibuvcr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jpdvdpou.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mzczubzq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvpojnh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ogbybfbo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptumgsmo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vapshhtu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxfajvea.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bxikkhsh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lzqvjcjp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nslvzibf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cuefliws.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jfxtxhaf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uhcmfnbn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iozcbbxa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xowjnxzg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ffrmmmhg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2sbzxniyv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ahenropq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gobxbzga.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2abovtwwh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jyjuzmsj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ipwnnigj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nmmapwan.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2spawyaur.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ewpmpuxc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ycxucafr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sqialpsc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cktzpjoy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jzvccyff.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2czykbmst.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rftrdnxm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2llpvudko.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wvtbszam.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2usikcwcl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ffebfmxa.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gyxodlcf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wtjcmmlg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ihgnvejp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qtzhtmhr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yhvvfety.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2palpgdzn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddyogwim.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2laruadrc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tytdauep.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2klowkcnw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wnjsuqwd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2burwryqm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2umhciabj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vzaczyeb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tzgfkggh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hnuhhqms.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wxwwhrin.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pohtgcfw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bpddwonj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2aluhxrpt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zwhyewac.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hcoueptz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdyulyt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yelprtny.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2srvgmees.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fjzjyvhp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cshbtdtw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jfthsszw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yalksjqs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bcoytptn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2eelabeys.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wqtxllal.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oblvhbuo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bxvtzyho.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yrbwohel.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tibbhgua.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qhtnloqx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2egyonlog.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2thzrzohb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2picacsbp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ybgamcqk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jpiiqbfa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vfzaziak.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2prtzosbu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wixcytlm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qoowkwyr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cbwjgsnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nismatjm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gbsguulp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euojeqbc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2twtxyonq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vsezwaqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gitjzjsl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cxsciumw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yqfxyqxk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fglesgqu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dakytxft.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtewsf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ajauojgg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eurwcysb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lfjjuxzb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xrsrfufc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pljlleve.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dvumhaou.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sffvcuse.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2sqkzyjtf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2iqolsszy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ezbbvkkp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xirwodyv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ealvjghl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wzwaxtbd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hnsldjon.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ekhqeapu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yudcguza.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2unmjckdw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cadwfuaw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjqnhsew.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ulkytenv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2psdnuzmm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xvvrkwuu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sasbbvjn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2egaqulst.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qlsudrkg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pvwcfgpw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nricgjtr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yguwvyxc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2tnomkjed.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2aufhjcob.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fraohgwd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fpdpkyvu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ctklwfoo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2klspskow.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bkwyfeeh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2otaxtdak.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2csqsdbbi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2akvlasfa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ojbrhryf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ngiswkyd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2usjunjpv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2syddqxnj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tpinyimb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hbpamkcc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2smbrlqsp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cmnolbou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acmveggy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yuhxbgta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeajmqxe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2krfkvtmi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lsxxwdel.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uaxyjztb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fimmudpv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zdafunow.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mgirpcfo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tbhgmixb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2aumpilky.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dezolgdu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2iiafmgyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lsjcquok.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kgfqqcyr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dkaxmwgn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ynyieyft.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vufvdpzx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2erezjlxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bdasggzr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zkdhmpxe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ygrfulqy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cwwckusr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2plhurodq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gjtsrmxi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nizcqevt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmgkhdnv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zkcqjeyt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ppkhjefl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2iixmaxmu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jqtutuos.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pleijpgo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2velunnjl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pxlofkvv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tepgpkws.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2faiexkja.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2oapxuvcl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2flkofnmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pzklsgaz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bbrysufd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lyfyqhgg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nlcdqzdz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xeretxgs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vtdseqzv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pjuyftip.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hwurkmva.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2qqiixuhe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2avgaesdj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bkyzeeyo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ubkkurgg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgfevujx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kpmzwbil.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rtlshyxc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezwfmjly.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sksiojuf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbxervt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hvtchphy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cvaqrczj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fpgsfwfv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ofprijla.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2offturzi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qmfwfhdc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2csqbdpcp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2sahguuul.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hxtlznph.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ppopzjtp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qzlnovzz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2odmguumj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jiklntze.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hkdcdfcg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2udylhamm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fecarkhp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nlqoqixi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2aqgkejdx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ariatpyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxgrbyce.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gjxcxbbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovlqifqb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nrrjjwjj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2txamusrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zloqtses.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xjnkrmgu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qmdltagm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lukwganf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uagyjort.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lltpskij.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rgawpfbb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ipxqecdb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xhwfoqwh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2jofiqive.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2utgffjcr.html

);
来源：http://www.52xcode.cn/Article/details/gt2ceqkysnn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bpbhpttc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sjdcplsk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2pjnjropc.html


<!-- 参考信息 -->