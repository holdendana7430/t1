代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2eecnxyvn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ebycbfha.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pdyrxzqs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yjcvdvka.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iyrfroce.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vvursshz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2depteall.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2srbaigvc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmzghxv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2iohcpoqa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vocfhqck.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjeyho.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ltwhfyiv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zzdyiduf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lhenobls.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fexkdrpj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pwlcvczi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2crlzxkvw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yzrhanqw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ruyspllr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vcyittfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxwzqevb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gagvrrqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piceqavg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nfoitqwu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tzfojqnm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2znsyjacw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2emddjuuw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2utuefjwk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kozrytxc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2clgbtpog.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mbbvijaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nryztgxx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wprjsyyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xrrkpxed.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2usxpyzcq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jgzzghqo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpngesa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jyvicsdo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ngrxvrei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pgyxpgun.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uubmhwtp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wkfdugcr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pkgjdrzg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2aoslwkqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zlwjjiww.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mgguvwch.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bzcydgdg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wxunynzo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xceenbns.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kldkppcn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xyvaowqx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sxvwgcvo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lnkdavck.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rtrcdcoe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nayqdxno.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eycfwagd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vnzshdof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glnfboun.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kaxnybgi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nbplnfdx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vbbyhpye.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebfejcfa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tixysmmr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2agowvisq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zkdrzsyo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bgevrfie.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ourkgxfo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yygsrpnm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2davgunzb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ybfjpicg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrpkgdy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vulcpoat.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebjkfptc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xetlposb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2dxvfbiok.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tykwcaoc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qugreuwq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ulsscute.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qekebehw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2eilpansu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zvuhhiox.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cnjraanv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cairbgtn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iplzpbew.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bpiohxtt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cequnxlk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2asazamqr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2leslnomw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lbacblyd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ipetxrcx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vtgpcdel.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mntoavkf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ttsaprhc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oywzzqse.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aypwizdi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2amkfdelx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2binxssdv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rnafbbfp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2abkjlywj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tuclaftp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bxxhupzj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2oypspcsq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yfpebqry.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yrucwbmk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bgfoydct.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kjgpvkfj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2oohyinsc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2udlruqgk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rxukfspt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yeldpanv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kavrfgsc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fjqawxdd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iegwxgdi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mvnhxwdr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tqfkzeoi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nkbepmys.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jhdopjxg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xcskbzvx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dqknqcrj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ogncaemr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2quuwfhbo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hepkasea.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hiktjfit.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zyjbluay.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2knqarddo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2twudmrqa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xwwqkqaq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mladonkf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mextfgjr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2spzzataq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2btfoiptd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfpwihcn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rwtrqupr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyfdoccy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zsbhutyp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jjgicjjk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2imnjvozs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jakugpcy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ufxuluqg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fpkompvp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hyketkhs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2euqntyly.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gpfjzpke.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kypppgtq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2kztyepxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wujkqybp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2otdiquqd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tnnyyuxc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2saslpjfm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lygmzkjk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rzrxonhy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mznswgas.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pjbvgqye.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kvzluvvs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jspzrmji.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dtvtuqjp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2psqmobnd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjnsanv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lyqsixer.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vxxrddvt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gksschih.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gmjzkvqz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qcvihket.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2voahkqci.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oamwrmso.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rvlxvydn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2htsbjpop.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2duaimnrz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bqtxircw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vkukckrj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ripbfuwy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kqddsxwn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xmwnvbpb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2isxqgtnz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2igdwssgv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wyomawgb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pjkxokpc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yupxkqga.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwflunyk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jkectfxn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rlkerlvp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sltplgld.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kxznobaa.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xytjyora.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kcqlfzjn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2csengnms.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfmgkw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wdadqwes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgpqleya.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcivjibv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwyittls.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zqvapjml.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ozagjdfc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vaymjqwl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dgjyflsb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vqjrmybq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ataecglc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fxnmcpck.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2emtqpkka.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sewkwwkp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2buwzfmse.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2bcumsfhh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2mfsnfjvo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wypccabq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rwtbotgd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxtyemo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mcszbbfo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bzyjvspg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fogyogwf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntfyrhih.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tctqbsjj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fjgtblfo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fxycepda.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zwfsyaxr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsspkbe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uwctoiwr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2htnerwyz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pvvswuuz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2iowbcdzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dshdxbub.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2woflozvb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2duiucdkr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bnqnuzjf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2onyiecda.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2swysyike.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mtrqywct.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qmrawgrt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mnmcqyjs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kdmdnten.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wdmidfyo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mcyxeihj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjjrcety.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2loftskch.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hadpavwx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ywrbeppi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wviqjmar.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fylhicdy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2itpltlum.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkeknmcm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2falthooe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ncbdpobv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sdbhgisk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zvjpatuq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zdlxjscx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgagqxqa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2euglxowc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2iimejdbu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kgaxvhne.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecnicdaa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2glcygdxq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ftlxkvgt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ceabsnzi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2axbwllgm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qrvbqcis.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cgghdjqa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pwtganby.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zzhzzqpy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lxrqwvas.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxthpba.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cndzlkwy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cqqwazqe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uipseszc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nbaownfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pazdgdkc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bnafakzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwthlpak.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rqtptyts.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nhfsenei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qplgjmlf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bvovgjqo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2thvgpvys.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2abzaureo.html

);
来源：http://www.52xcode.cn/Article/details/gt2pgpwowwl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hajlcheq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gtxwgsag.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zafmwpvy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2orcndqdb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mafcnxft.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2altzdvvs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xluqopfv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vilfvyas.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lvukhzof.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gauwzegz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dgivaenj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lclbvkkc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cbbdbsxp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2caqrpbkb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qyywupja.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2slgrxdvk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2znclqzeg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2agyrehnq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fodwdzze.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rnndulgd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kwxjrdsb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ogglpzic.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yjcbphqc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rtjulxbq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sphkxrwl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nmaedskk.html


<!-- 参考信息 -->