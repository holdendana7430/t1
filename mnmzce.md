代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2terfmluo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2beqjagoc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pmuxwqtz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eecaqbng.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kdekzqha.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tuzqnnbp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tzsqxhnl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hxhcrbli.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bgamvkdi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tkiseeot.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jzagvjbh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2raobnwoj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kadtmuek.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ltlhqmzf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qaxzcygw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dphjwbfe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vhriklvf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2aiccvomq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fhhpxpbc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2oxuhvkfs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tdbtbwna.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wiylurlt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2byckkhhi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jwzvtlxt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2suwyyzeb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oqynwjji.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wqsznbpx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wztshfrc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2osmiqxlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvwsncuz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qatmogbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejrcknjl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ycjsdqdy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gbbglltc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rlsagidj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kpslxgmo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ihpkodbj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2laalkgbu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oumrtjfc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mbhwuncy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxldqpjn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2juwfhdrm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dgdjjqkh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sullpwei.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tomukpyc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mdvudhdq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmagktc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbafcluy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xqsefyih.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nrkuyrjz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ymrvoogk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yjefgxye.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gqtqsflw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rzajremr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fuzyqslj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iasgazpu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kvwebpfm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2orcrjmok.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2opikfoda.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wrprfvoq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uieugrkh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2riazekck.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jpuuczwj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wwmlhibb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bznvkkzt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qphyrqhc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hesqbvmb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oicgdlrc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vbudkosv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjpsowu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2etlcdrur.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jkdwcmbd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cebxjssy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2acxdmpxq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2typmwtus.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dctwjosj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hdhvatnm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkzilkgh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zopomgxb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wbjfqtma.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkchgrbg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lstkdgqy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2raswqtph.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2prdqphbp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2onmudynw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gfywuhcg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yfxpxeys.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mexawnwj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rpgknlxe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ejdmelqn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2crvpsqzn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2snziikpa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vjbvccad.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ltfbsypr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lrxeovfv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ozdhjmyp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ortrxtzy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2prwbcabb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymisnjlb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ywcklhrv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ipemxxqp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2beuibtnb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sdixkhvl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kvlugluc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2omwjcjvz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2chvhtotz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2umdmhest.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2feeuftjm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zwqiklzm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kugoiqmn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hsrxmdsz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xflwsuwz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2winmzfqb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ckfvqoxo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dvbevhvn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wvgwqbow.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mmjylexc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2czsxdmhm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pazagcbo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dbqtmhqq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jrjymvix.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkegvhlu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2slkelhon.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ohixlney.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubzlnrwa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tnyqwolp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2srhgbctc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gsneymtr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jcjpjndc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zgrvicjp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pzwnphoh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2osucmcmi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2agnuwnvc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2edvlblmk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tqotulgv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lqnjbrpf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2txarskex.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2iuugzcuk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tyjolyeb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sitlrlrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lskqhnmn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sjzmpeam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnpyiwvt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ppowydoq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ucppfecb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rbjnzcuo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qpczuszg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2llbfbqiy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jniztufc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xocjgayy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2edquwoez.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qxwcpman.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2iqgxyyvl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxezvzv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2epjbrhmb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nkwmtxdo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xlijwnsv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oiyoldiy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kmdfkwzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kdtvimdm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cobwdbwt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yyfxhqwj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2tlmcmkmy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nxgrseww.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wsptaarr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ncghfviw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pknivbgr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tspwzmpr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2owiwndfx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ybeivorh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2grphuycj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kdlqggwd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cfhfgslc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2motdmtnr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jduyzooc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jhhwipqc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mmfbuuev.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2nvlhhmdk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoedvila.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ghoxwrgo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvpzkmx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ryosucyt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oaicdoci.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ijnyxhzy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ehuirpan.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ltysbygb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nioemazb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qntbnkpb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gukcncyi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2eqgzauil.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ateefxim.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2axewwqoe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kadyeauw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2repwgsiy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2svxaceja.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gzbcbseo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gzmymilt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcdpaqla.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2eqnfuxro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrjbixcl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pkonalsw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vqluizio.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2luxpbbgc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xtsnyywf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2avznfqbd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hrivyacf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ashgyphb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xcxffsyd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nlsancal.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vnitubmn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xihdhvva.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gplxiang.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tubkgknt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zwbgzjvp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qancmdbc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2avyvqzhc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avnqawma.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tomuywxp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xouodnpt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tkbglxif.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bmfgijwu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cqoncmkc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uptgduov.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bdousmnt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bylfsxrf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2aerqlkhp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vsepdzfl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ltwhoaqa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ozqflcaa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lycaztou.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zblsmzmb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jdskwjra.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ilfbmkwn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjlanlf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2oynxspiy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2llyeknne.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lubjrbbh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dtosdsmq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2habkeoow.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ukrgdwtg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yunuwkfs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2abtbgkbz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2raixaapa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mieksmgk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rbbpxjzj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kujjxsjf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bfkknlgy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lrgfpdvp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kppjcmou.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otrtnucy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgmkcudz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lkqynidz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jfyqyuwi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxwvuejo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bhscurpz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2khjjyljj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zsjhozfq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uzeazrsv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjhbpddq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czlxdvgt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2acawuywt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2guoamksi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2raakrcxu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2flzmahwf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ghvlbvca.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cbschzrf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2fgmkierj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqhrzbjl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sbmyzjzj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ptmaibxk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2iqveacnd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dejurhhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdrvgqkr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yrgmvvcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnubgcko.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2drcyjyxj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2idcrcjea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mmkmcjlt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rhhcjvpx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2uvepsyff.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2otwnbpvi.html

);
来源：http://www.52xcode.cn/Article/details/gt2iawzchbx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xhvukdgb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2lgkecfwj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nwwcjxjz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2agskznnw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hchqcjqb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bqxdwkdf.html

);
来源：http://www.52xcode.cn/Article/details/gt2qzgbgjkh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2psyiczxk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2osnvxsox.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vonrynlx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qxonooxh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wityeyfx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vgurzlzx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xdizzglc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xxtqelsv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lnjhvscc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2omorcrhq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wiikxwcm.html


<!-- 参考信息 -->