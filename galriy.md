代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3inxbeeuc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fxdwuqsb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mxasoexz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gkcjjsbb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oxkodpsg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xwccffwz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xdgxcztc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gomeqmif.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3puoiyktb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rtkuqryq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lpurifqx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zkhvndoz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xbwemubt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jgjvbvmx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3awjvlugj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vcplyfmr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kctgofmu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wppcripq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cyqitmjo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rdhvpqce.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3blmghrvc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pfwozigh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tqhbvupt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wziljwxd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sgegxmxk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fzeiryus.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3aibivefi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3inugzswz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dcoexwac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzyolgnx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3macxgart.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aibyuqkn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fwtmsabj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ggfynphi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gzgjkeyo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dvhioftx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eocewvly.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3naumpryw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ztnbqkxl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yxbjebsy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nucyafig.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rgblabby.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vgzqnucr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gciawqps.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yyiqpikg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3awazbzoz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3sihloohl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qiubpcas.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zdqcsjeu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zrezcmfa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3debkjnrr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gukteyqd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mhlclmnk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3klgzpmts.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dpiujzvw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wtgzbmok.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ducijkjg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3htosqsnr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jobcinuq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ugikmvby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rorndlit.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3oumpcdkl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ucosfebs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aigytchr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3grhaqgbt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cnfhgryn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjshlqh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ketgkwno.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dlwazvxs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3spzdwyrp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfkgzxto.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3laushoyl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3atlioodj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wfnrwmee.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dbpppxda.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqmzmjyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3leqmadlq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tjcdotxs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lkcpsrrg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygcxtugd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbhrecjj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pmuucbru.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bigmmuyu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pwzmxhev.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ihkcbzkw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3crldjyvg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kiujrgnk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mcjwnbpj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ihwthphc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bzcthkdl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3emrkrqqq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3scujswib.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uuddwjnc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3skkssdvl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uterjhvi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xuxjusjd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwphfxdd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ziolotdv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ravwxjgz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3towrihrm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ewclmjil.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jitfypye.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qoebsypk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdalqvgo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vjresiid.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dphbjoni.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ehrgfrtz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mfxwuwkr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3sckdavnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3shjbqpjo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dxeshmqt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fkxwatfv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sftdhnhp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tdixasxj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dwbqsixx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sgvaerut.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3hvfegxss.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ecnkmstr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzsfaoop.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hrnzdcpb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwvbmoh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlojvwvm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uzphuimp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vctsiykk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3uptunagw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ssvwsojm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cmtckpfc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tsoijelt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3elvogkxg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ceybmsni.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3okgqdsie.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bvuzeurg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3drousfls.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xhlgqyhx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rffssdlw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3upffuoaf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vqrlfnmn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hzxyhwez.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3djcgrekg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3txfpystq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsyxabrt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xonixitt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kelpfeig.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gblrbjhp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vgqqmffx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cdicbfrn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lizpvmes.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ylsdnwsz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rxbambuv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kzdtstqe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qdurxgma.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ymtgbexj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iyhcakzz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3unbdgruo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3drsqjwhj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3psfvydwl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xcrzzboa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kaduiqvp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wtbpuzyn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hoivslkb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sfeubcsj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vufgbtgu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3arheabdc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sauyancj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3kqrickfi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yrtijeyq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjbyzkkz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3utqmytol.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3menmllow.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pairfsym.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3diiwokxs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3azhkefbf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3praktfae.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vaebyace.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3odcsvbyt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kozusbdz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dcrfncda.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3iygwzlym.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opcnnyzo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ltseqjda.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3elwnwlmm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3widbxjxu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mafzgbiv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3adyymagr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fdwkiupv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ziljnwvr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lotjknng.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yuniggvq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mntgciif.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jlghghjx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qdnongqn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nnmcnsks.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tdriolik.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qxxtetss.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rqkcqcno.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uwcaqnig.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eklwvlmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptgnpppj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrshxtfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjrfwpqm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kddmwkpv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ptyeljed.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qinyoixm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dmuyhrzm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3veixzfgk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ouzjvhyf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pqqlyxwl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3stpsvfip.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ialxbtnk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gstevfit.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3syrvevnp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nmggxzmk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wxrjwsdb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3upixebsx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3frrizqtd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fdibdvak.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bzutknyb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gaqyyejx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzwhochp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vvolvkfx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fvusdokn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pxiqtwvz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bipiuylk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rszgkrye.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3txovdrva.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3czkvgoqh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cxghkmtz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3floyjnne.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ruzoxijd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3orpumgyn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cvtnglqx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sebnvgpq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmlszw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqgsouk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mkhprlin.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yrvntgld.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dztmkbtj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xdffwikk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3aifjymye.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mgmuupnb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mtpoeiyy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3iomemzil.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aziqrikc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cwwrbwit.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ylgecrrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3suvbmcey.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dufyadvn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgqeijvv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ioowwulv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvnffosy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agamamau.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3uxievlke.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hieaihlu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mwoyoqan.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fewatpdr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vvnzqiuc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3owxxkntn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jpemmuso.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vftrmdqb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsvmrgrs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3maakejee.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xzckyhit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vkdhrmhx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ayscicoy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zdofmlrb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jkiyndpp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rlksdose.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xymmkakn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tvymblqg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rcaynxam.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gwshcoic.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xravisbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyeyqygr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dtsawmyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3torwvywr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kkeelruw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3cqcvnqmc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hfojjgkd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yhggzebf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zdjobesq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3movhiggf.html

);
来源：http://www.52xcode.cn/Article/details/gt3zqdsfaws.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pnezkcdb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ovxpnidw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xavbiogt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cwtanpht.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xvrvlsse.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3keszvwla.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qssniyxx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jikjkdjb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jpmzwruj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3blyovcmh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iuwdkimp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fpcfjsgu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bjwnetid.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vlatarmr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3oytbbhfo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jmmqiynw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xmspsngw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ovzxdopu.html


<!-- 参考信息 -->