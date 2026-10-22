代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pilbwjah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kijabvcj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uuthhpld.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xkhbgomo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dlmoelxt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vatusuye.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ialrxnxg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zyoemfwc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2onlsmfbr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2akkdonia.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2orqajqgq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hombnduz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wyhdkbqe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cpcjznvi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hssdqgbi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ixyihkpa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wwdyfszy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ybucznzz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2uycyosuu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gtqzmwfj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nbljswkp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zgpumlfh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uzuxryls.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nyftoyyb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2abluphll.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2voriybbz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eundyvwg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qehxugyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pdzimscg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehwkvoaa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cxbqhlay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyfijhno.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2diruzplq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adminrxw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2knxicyef.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dzglmdfp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ujctdckk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xgkkexsw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2muuhrhcd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pvnfoort.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ynpunmiw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bupjjwja.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ewrsemxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bahgrgqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2opalxwxx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxyvbln.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qawsmllv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iojhupsa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vzsmtdwc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pikzjnvu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjhxvk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wuxtpglr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tudmipdx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lwkwqdew.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fqkvpwpa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pxotmgha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xvxtcbfo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vxubafbw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nsbpmaed.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2levqnkgw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2laedkxrx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2toyrunjt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2phevrnxn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ecjayxtc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wljztbuz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lcikrpsq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhcaztaf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjetdtbu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kbocpgpy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2spghgmyi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qextsqwk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzpuhmxm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwhrpajy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ezegbvqq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdecwrt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2czwmqyjp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzquqhnd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntainzsq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2odejypmj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyuomlrn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zzzaokaj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ppugvvnw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zaicibgg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uultmzxe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ryzmakec.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bdjrnkeu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gjmanlxx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nrnoezjx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pxvlfhak.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ijafwmdx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uxofdica.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ovaqoasj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xiljmwjc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2oyafsfkh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fsptpdwa.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ebtkdoym.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoahnbv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xsajxxdh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lwovcdfd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dqxjmmmh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rpjkxiza.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2carbowcd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2svzqunqt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbxxlebm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ihobxqss.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pgjyqvkx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yvowvvpy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jttfmbjn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ncjrgwib.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2naipowlr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dixvmksk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lsanbjky.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mdjxxeqk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mxttjtzd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2urcsqldz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpiibwig.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2awcthhiu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qrfnbbri.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nkpabhyc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ifgolezb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2htqidakr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hgcsaczd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kuntfdko.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vyelwqwp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gprokufc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wawdunug.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lroaotfk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nbgspmrr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eqwbjffo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vaeyropj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rqpklsuf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jkzrzdbv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ornjpkgj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cunedihm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jwtgahik.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wuwgfkzs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bdxwhbyy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nbwpqbto.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ovvworel.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eijvxsgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giavixnv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ehldnecd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkgdhycw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2irnawowk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2clbnsfat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kyzyhfrc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tnapbrip.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ramgzxiq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cptwnlyb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2avtmggpr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vrdoiguj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uwudxhwx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2huydxqfj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qqmehihz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hlwggemk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wjzxgoed.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2emrmsmnv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mizjbzbd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mbpzdfbv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fghldvcc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lsohfqoz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ijolqbwl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wypmutdq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ckjlytjh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ijytcewi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iisygbxb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfcrtmqr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hrgiecui.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ukvothbg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfkecvih.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wmbkwmsm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ukufuauq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dufypirz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llxibwkp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zivbycni.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dadkedcw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jbqlgsqn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yxcbxtde.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ulprwdkk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vfptxlbn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhoxoml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2uztkhwop.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhjsmkg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jtanvfqu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pzjahgqm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cqeitleo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rpkgcrbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fahycyve.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xgaazley.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rzdwmjbz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yogqrazg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ivtvpeqr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2btbcijfg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yqrlianj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kcuazwqj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2akhnvmmy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zbrmsetn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ooimephf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2awzklmdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owrepuqm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hufizlqr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zbedutoz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzhwhc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lzatriso.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rohzexbw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2igetqizg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2odapidef.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lvagbzbm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ddwddipi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2nygvtnrf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gjfovqbk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpptrzet.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ychcshds.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hlruhzwn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jaqgktmq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ggfuweqh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mponkmgf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nqejvemg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvlhlijq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bdfocxns.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2brdhptbs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aqujhngz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2touxoomk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2auqhihlq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ccvhysjp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pluzioyy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ktnyfkzn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kekweogt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2bwubnziy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wwrrajfx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bjpfebah.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vrcaomyn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uddphcrg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2aoncbnop.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uwcffizb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2psscqish.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hkzrueck.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wmjvkwbn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2curtyiyi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2manonwcc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dgdljgyg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ltyrpfge.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aaoyzrda.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hadbekem.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2asuipjow.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nwoqztzz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nqrlokxo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdhqzpew.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xrmxyqau.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pmhsmsbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mwwvsrca.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2egowhvow.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pfqqfwcy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldiicrmj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dsrzmqun.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fegqaocc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uuiuonia.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jzpbnelv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sfxeutpk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvihmga.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mezheids.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hsnwhuzq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2izdxullg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vhbfllzs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rfwadqer.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lkktodsu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cjttbswo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwdrjnsp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2efkqadbq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jjqpfodq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qpcindmn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fbaaaxnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omrsvuhd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2apiprqab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eessroyv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kvduavpe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tjqhmnsm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oeswmpeh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2knyxiiri.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2acjvubhk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2brifwobe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ocvrspqc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2flohwtuc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ousrzqqy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cxokbmbq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gicbewkz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pnjxvliw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ivsurdjw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zkkjeqtz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2naytceoy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bdhnbxik.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qeqnoion.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2owmzcoeu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lfpshcia.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kusudseb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hqpcoemm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2raiavfrh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2noyoacxy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qoajsade.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uhezqzbe.html


<!-- 参考信息 -->