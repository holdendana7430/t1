代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2knlkfcum.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wgcmwkld.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hfjbytpn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxtzlwnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hovqfgxd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tzvpkszf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qcdatxtf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ubwxyync.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2udednknu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tfcrhqsv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vyhkejlh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iggcdqlo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rboelbpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ljuglnpc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jhmgsstv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kcgjbutt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rrwlutke.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fgirntsh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2iowfqpfg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlgkpis.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jzcxyere.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pwnahnku.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qmblblxd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jxekjrnh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mqnvjafi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2igebtxla.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cuxyhqsv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2owjohmyi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2puaeoxef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccrfyjzt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hjzemxvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pajsilfd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vhhjobsf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2evjypfbc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fbctqxlt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2joeyvoiv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ncrjwpfg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zceewgng.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xusjxhic.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2adaxonls.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzbqoshk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bqagoehk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hizflknd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jkkepkyf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvadtyh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2conjkdyn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zodadmmv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2akfrupfd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mkophwyz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tdirroxw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ztholvbs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2krxeisyh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xclomfpe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kmcpsilp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fbgkgouh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zufdjqwr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2saqjwfob.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ukfggoxg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cchonudi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vragwsss.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2auxojhic.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dgzqqbgi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ujeksthr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xzpfuzbs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqrpqgco.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gqjaesqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmjzuib.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwjzxqav.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2blauayvk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqbppqvx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2svybwkkk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dcvirpog.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzstygao.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mqyfqewi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bnyirfsb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ouvcumyq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cakvfnqo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czkxtlln.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kwlzpkup.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkudsmwi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ahedaitv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rxyhnonf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2eikknifh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ynhvcdci.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2blqqsgxl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qkrkwuyc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tkicwuhf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gwxdsrhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tpreazeo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xryxlgly.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jzdmltmd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ekizkbnt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tadlcvbk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vcsqoaoc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jagqtbhn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hshdgtpn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxqymdno.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lccmafky.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fqhxksuu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pykbtozz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ytjdaymy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lprpgxxf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cfxxggea.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zjkwtbcy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2orhhsekg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sngrnuye.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cavkjcle.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nesvrhgx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ugmdbsja.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbztlqsj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zjisaaqf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pagtkvlb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vcmjpptn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lzudvgbu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bbjogxml.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nufzrkex.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2taufxhgc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgjmsbv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bttfivxh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hefsvtmw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bnhezhvj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykevzops.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fhvvxvnb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2viuyybon.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2egsgjrtp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yplyzdfj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hbocvony.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmejqibj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yqyxshvb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cvegapmr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fkidpzla.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zwwjcnzj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nqpyluqp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2azotnblu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kisaeafx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cduyggjf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jryscuaf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mwabgotp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jicrspqw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qpkcqzed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrlgcctc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qenyftxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgqpyoig.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jufmunrl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2izxwedgv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzgtxqgj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lotdkwim.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lsvkdyxq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sfnlpwtf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xhrgxpps.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2edkqfdjg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ffescmbn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vksnzyim.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2owmbuhbq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gigffbfc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jghijpxt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hnxgbifp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jmwuajdi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kkflvsqt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2twkphrft.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hcrfminq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nwceymms.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2saihxbod.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2udjqbriv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ypbrslho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nqacvxhu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvaaupk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ilufdffw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vexpgxgl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yadlttrg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tyhuocbq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kcrdwjbh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ixfidkos.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afpxhzgs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdgzgoas.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dlwecuhv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2giquvkjc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fwvwibhj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wogeexkn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2tqtrghtf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pufhonjz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sepszgix.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dbhaiapd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ussupufc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hscocmbq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ssyszlal.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tvqzdctq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2obssqntg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qnioccsi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nvotflox.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2inrigxku.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dvsfvjcj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qrsxbbuj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2amlmgddn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fqnuxryc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2taixxonh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tttmvxvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tllpuhih.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2upzqpysy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtwtlexu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xwawnsmb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jpumkzqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qzapopax.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bngmzhht.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eyvtljjn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dfzwyury.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2trwgtgah.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dajuhyxu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zwbgasmh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dfigwvuy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kimlwdqg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2yklpqcvw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tzlquhgr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nzzhzpsw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hqcaowxk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2feekmqrn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lwjsnsrn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hreqrrkk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2omcajgzd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fdctyjqe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2lgfqabct.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ffzqvdlu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oljymfww.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nbwxabgl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xrutotid.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqnshxf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2swjmmduj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ziaivdrn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qvqxmjxb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uvwfjpjh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pbqdafsi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2chcovdzf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lltgyhcu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ixcjdnrr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kivsafgj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zhxbuwgo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mrsznegy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kcbidjtv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2trlwpejk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2psgcbqrk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bouwnzgr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wgiazliz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dynrpdza.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2qaydnlgv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2quplpwnn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fpmawpin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2anvmjwos.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvztdnxx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nyncwwnh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pszjzobz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vmeoqulf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bgultvvg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2yvjrhhfb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eayydujz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2dakaytdr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gaokgqdm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xszsphtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2khesakhz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dgdlbiaf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlblumur.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wmdigiph.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2arczizbf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2iivwwwsc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dcurhqug.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kvwpixja.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lxfevtth.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gnkrhkip.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vjqqimgu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gxejqnzp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bsabbpmv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wvgyhzaf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tdzkeoat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptehllvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2owyjzbwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrujvqwc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ozlawowm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fzzhpaug.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mvluwztq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xehmukop.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jdagxfza.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vcucdjua.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rignuzua.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eleojrye.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ktqmajpq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mrublcre.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ypkbugrk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2reavhocw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gmcblpgp.html

);
来源：http://www.52xcode.cn/Article/details/gt2ztelvhsv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pmsqotcq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fuclesro.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2pxyotikb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2utomlqyj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2grkjczzk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wtcnutjs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2loxmcait.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2srqfwyyo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bageksgh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yrklbdri.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pvxszgay.html


<!-- 参考信息 -->