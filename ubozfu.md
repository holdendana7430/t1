代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2innxfvfe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gbgfvztl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ljcytfic.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nyzgsgny.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xmxpvrcn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vrbdmljg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2akdoocpd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2buzesbli.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2whmiwnks.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vhooowyw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eewwkwkb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cmatjicy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sqdqqagx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2snxphwhz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pgkvapvg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tpmlblzb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2iiqpywat.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pdbptqsp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nsbpbagv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2trndntto.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2trwzqktp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2auklkcgf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2edrdgldx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tecmidxp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hvazolcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2boxaerih.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2oysskzio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxjszbcz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jaglmyiq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2awvflyzz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cmgupotk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kahyszrw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ayqwwbqn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2asmzpuxr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ajppgzmm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lrygdlsj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljzcfuaa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wrgqkkgr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dlcvfnif.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zgdqerpj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kxpwdwib.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zanwbabl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rwkhbwnv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2waljnjnt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gihpnbnx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vovwbxkd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2thlocasf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2humsjlli.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gjdvfvkg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bkiyjymz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kdixnevp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2piuevvrs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2txsykiav.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rmwpoaqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dzsztlmo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yumvoedi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvfydmqs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ndwewmwk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjoujpgk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kxngfkdq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gxfggftv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2flsaijye.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkonhkni.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uewvktqo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hxkurlsw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcghysdx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxwvapdm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2knmfjezi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2evjfufnl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fiptiqew.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nvkdckps.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2lzjhvcmb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhsngdbl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxutsxsg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lnhjhzys.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2izmkiifk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xddhmeck.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fzduogvp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2uplnikmz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lymdddak.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qiezeqhu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fescyzrp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hjaiercw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hovdefmv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nqyalwwc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wkzctnbg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xfudfxgj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pgjajnxf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hwadjcil.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lplzkmpk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rmcdjddh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lsiicilo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvlqoqh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xzwkckwv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gvrhtvzu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dvnwerff.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2thmfxyst.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bosweafg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oznflaiy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wbosmvwv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bvtvxads.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ioyvfipy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2awyrsbqk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jwmzmxzh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mjehjzif.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pqodtoot.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2iqwgrsfr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tiksyone.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2miierpli.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jnqtotps.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hvqfpsjm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xasskrjy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ifxhtuvg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eqpgdkwo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdmztnh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fsnuyrsz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2utvgnjan.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaeaqgme.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sossgvvm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2sdzpbbei.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kjoeppsa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2itcpkxxr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qfyopcnv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vwvbjqwr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wioceuwh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lkbvlzjm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2biuiuvgi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ulvmmvpw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qgcanzkm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aflzlmbb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lobxayhi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2emtyisqu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hhgtkhbu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bzqhwxtr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dftlltrt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ltvthzhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kohlljfi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wpzvyecq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krhqdolm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kgzglwmh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vzrcgsoi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmwdkbyx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2uojtlupw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2shbavhbu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zbomsjcs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tvxnwulw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ikbcvgrr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xnuonmgv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2biptygqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qioloihx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ezvbboos.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2siutgbtk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xgteijxq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2aibsxwva.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kpfyxjxm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ifdqykph.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2saxeusgb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2chljtaeb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2adjkaeuy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kckfkitl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kzyrfniw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zddmgdvk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmnvpyxc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2itdxjoax.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dxdsccuo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyvejtdv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pobsmxyv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gopyokfe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pkoyvkzw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2irivbvad.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltlzzcdl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zzinvtba.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pwhmunsk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2irwcewwk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rjqexkjb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jkojsosy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2emlyhrvi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oiipuhlp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nkyzrggv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sohgplls.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kmmqrgya.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xzfaozkd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjautuh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbhthpjf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xixknyor.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kvifshwg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rcgaclde.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ttvvyzth.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vfmfnyqx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fwsielyr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jzrpfmba.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rzgmuimj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uyotankz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szeptibx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2enphifxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swzmnkmn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wmtambtp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cvarokhl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xmniqbdy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2supgjwei.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kmsfmecs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pzsiarrg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2anjodwmv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oglblemw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kapihitl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pawtyhqd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wbkuttje.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zjnwctrn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vwowswhw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rcjqwiew.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xsvcqwta.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rmrxejcf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2afjfuuyy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xywxxswd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2cyifmppo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gvsvodfg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2abnbhhqo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hvfsvrpu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zyufbfzy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2baqbvkmh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2eljukqzj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2owvgakxn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wzpdblyb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xzzinezl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2drltnizs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2leekibyt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qlcjcljs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qrhdajwd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tzqgodvr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pxhvbmlt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qmbpdndq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vafurrqf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zvymnsqv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ynalsxfj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2iwdpqcds.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2arwbmbhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jafsoapp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xjlovajx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ppitytsl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mmvziszf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kiolkkpr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uzhcvpuf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xmwdflci.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uzbtmptv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dxykxuhr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qodqfplu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qazohgxw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2odroiajp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtvaomc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gebbgqdx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2libspiyy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fbnybnth.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ycsvfrdp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ifmzpfmn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kosgpeso.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rhrwatnr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yfjzppwb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yrwbedzi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fbykirgi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lfulhsvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ktaefeos.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2piylpjaw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2znewgmap.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2emjmfptk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qkakbrqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jbxfpwjh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2egnjalit.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rsqrkjuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnjulfqq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ngkdzxkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndldxgse.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xoyavxly.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2boduajma.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2izoeorwz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pwwpczzg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qpsasimy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wuowpnpe.html

);
来源：http://www.52xcode.cn/Article/details/gt2rfumsxjo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qmyfmars.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2aytkgzol.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qooggvft.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kemdognu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vxvadzju.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yewzhejq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xqezkald.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nvxbqydm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eqmsqoqa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lzzyuval.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yvjotsge.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sruqjuhz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pifmgzqj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fmbsavbe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2izsncxwp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ugmenoam.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2iznpsaoy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qrtujtka.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zsfvyfor.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tkbqgsrb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mzyrnjxj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hwmaydtf.html


<!-- 参考信息 -->