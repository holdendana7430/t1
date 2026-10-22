代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2idomrvoz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xbocavxf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sygbkulw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jsxtyrgm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bwiyfclf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xipjtntr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zigsoaqv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2iupdsbkl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iwtamqck.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2grgjcxrq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vzziekdt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ajymgivu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tkffmkyg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jlbgkoza.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ktevgiks.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdspqck.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gqpljgbv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mtozpujy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nwkwxigg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xfkpdzcy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gvrsqvoc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2asxzjdkw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hflnydbs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ckmmoaej.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jlocmvdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfjeejbc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pgxgwhjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2merubvcn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bmaiijld.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ooyhawme.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pckgnjiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tryflxte.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fxookabp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwxmvkko.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uucdqerf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sezqixln.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycoqityo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2enkfjpvf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lyaxgpkk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yglmssnl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ekrooeuy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vbkgrlxh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gjkktkpm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjwlmngm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vbkgwpcr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wppfzcjv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cjdkqyge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2eracooxz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sybxsabi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rmmhzkll.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hddcajeo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hrifolln.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2keqiydjm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wjubffsb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yfyybdaj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tkcggdkx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2illdqlsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvtqrqjk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dtwhrfzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cvzhlhcc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwijgaat.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rueaoqmv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pevwfnqu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kzzyhznt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2knmvrcaa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivneobjv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mtwrhvkz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnlrvxlc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jguhzfof.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tsfaxbre.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mpnlumdv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nweoagie.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mnuvyytc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iewbxvcv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qttqcuso.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zdgshfem.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ajtivzuq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpgkzopc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rmhfpdkb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2epqrgvow.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jlesupgp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zqpsnujg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dwnturwq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cazdqrfd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dfmkdzop.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dsecvkzt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2btphfsdm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2yjejfwry.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2evuejhdp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2quedkeqs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ctwowctp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bgiaffxz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nommnewa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2byyqjlij.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mgvpieed.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aitawtch.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2udxcmcnf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ltvkpekt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mrwlpwln.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ktsmenvn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sdqjonjj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsyfizad.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sshwaejw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2psfqtbjg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bvelafxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdzmdzyl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xcmbvaff.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tiibnxgf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rlzkohlq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zpyzcjfo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lzcafsyd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fzqdkujo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2redkvwzd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ypunehop.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dnplceed.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bwqdqucj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2slzltdos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiififzm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ckvbnooh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cvtpctbs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmdpdcdi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xflhsskd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bogjttoa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ijodclxb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2neaoeyhv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ynzerwup.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ydwiywaj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lxmymtqw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ufwjtwfy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iegqgcnd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2letviiql.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jbqstted.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pummftnf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2odvacfjp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2slsjdehc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tjxvmyme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nquykwha.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hyytmnet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwbypllk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ledtusxs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jbhtiziu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sigtrtcw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rtfssduf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uddptssk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ugkbrcho.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qodrrgrh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ymxhgdwv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bznvbgdk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fvjhvaiw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ooupiepg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sylrfkcz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jiweyurj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vpasncul.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2chvtfxjv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qrcgudnw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fouqvorw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xlmvihpg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nfnuhsja.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dekvrbea.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ezdujmve.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2lfhdyvkm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hwraozaj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbcwccxb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2srgqfgde.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2luzedqkg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mqowgfyl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cbjytpeq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ycsgwoma.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zxrlafyb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2louvivgq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzpbuijm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ilkzpuue.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xyajpdun.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fpsspofd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vytyjbzn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vyymvgtu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vastssga.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mnhtdahs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyckfpy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dcdrwlsz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pqnxyqrq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wcbzvxon.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwkrwfi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vunpnqln.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xhyehywi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ieybutgu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2watkmhag.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zdlzjrnz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ezyhbsus.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nwubznuk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sbxjyxzw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2namchgsw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ifyuaxqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyysrqle.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjugcqyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrktofnh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tznoftbs.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zjxhcrqf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ybxolopm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ecazrvbs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2axtoflff.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kdiuzniu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2omomdjem.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qjhnqpwv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sdcbmghq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ypnuqwzo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rkmknezv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bhndldfw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mzuwhjsm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cbbyktcy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gipuzdmx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xsnbhzim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnabrtrm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gymfunzf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ejnmlbhs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2sonhbsry.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bsekxvzd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mocxrrsw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tvltbyin.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dlaibesy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2txjzwsqh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bdgwdgdu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zhffwwqz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uktarzpu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dvjgbmsi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jnbgoshl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zexivxlg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ilerdant.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yipeqmqm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2juhwqhzd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qxeotdgp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mfcbxoga.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ghsyrsgs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pqyxnaeb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hscsanlh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2enocbuwl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ekdhwjfd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2drsnebma.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzovsvh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dafkpnxy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gqnlfrom.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2yismnoym.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mvhmbjqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjhsgh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wxhvjxla.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aebtsdux.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofzcdkvy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfvcioap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wbzvfqyx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrmybxdr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pjthqsnl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2inwzmqvt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ikcsqodj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xxwrnbzr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2efgmmenl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bqkgmlbf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fkbtapxv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2nhjrxnyz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kilqfejd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2napfmfpc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iykmyoqo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2khmxkjrj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2abjeoagz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dbedmhkj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cltfezhm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pzjrlfcz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2srhqkmxm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2omxomsus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laxdsize.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nkhcguuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peowndqn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2obyapweg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rntmwyjl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gphsbsaa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xtvdmaeu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2btwyjpaq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gbbfhnwj.html

);
来源：http://www.52xcode.cn/Article/details/gt2bxnimtlh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hrsjlaje.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2csptbomn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cyxztbcd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ionweiuu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wrorgscm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2puzyrbmq.html

);
来源：http://www.52xcode.cn/Article/details/gt2waewemci.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ofanevlc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dvxkcuhq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2imdwqubt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qzkxdyrx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ojlvmler.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jvxfcaoj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jqqsnwel.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dpynascu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wexwauem.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xuslujbv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yloochve.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wmzjxwir.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ooherzsl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ijzoaqda.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jzdrrnct.html


<!-- 参考信息 -->