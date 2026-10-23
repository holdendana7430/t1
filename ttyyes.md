代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3alhhpvoo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qhdljpyn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nbywtvru.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ynlxzjsd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bzggfnsz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fkqpnobv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wernuunm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dpdcmymv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nzqxprwy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3newsqqbp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bxchpngj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xjdhzhvo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kyhejdwm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jwwcomhd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3plwudgmf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3foltfkcb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tkmokitw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wuxrqxsm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dsfgqrbz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cipksvtm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3uatkkgdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqhqkyoy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ubyzxtxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqmzanjz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mbgxradp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tiawogwd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yizmoiyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xhakchdm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rseomkpp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjouxjr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdekqnhp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3aoojlces.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wbolfcwm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3irtmelgw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qcnsanax.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xjevdwpk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdhecmr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qqaovpiu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ftkprbfa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfevqpek.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oiazwbxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tqmkjehq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3igniuojh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pqfyikli.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3eenmoufh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ylzoigwr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zqedsxxu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3caakonbr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wnhwpaty.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dxkttrqq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yarncxte.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3keyrqzys.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xgmtkwmz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xhdnhohp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ehsxiwwf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dbdesdws.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kxqtbpjn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmbodan.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwixwdq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aebyjwhw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hsuhxlxe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmlwsts.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lelddnxx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xbyqslee.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3clykqkyo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jlkvqqcj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yqehglle.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3stfgsdhp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qqcjobzb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jldvbjvw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sygzvkrd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cwxahadf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3szgykjtb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3boioasfr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3aeblhgxb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pharcuie.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gdbkjvpz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3baupclvt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zzhivaex.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fealywox.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ctudatnn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmnmyhy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3woyhahfg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hgvetxtr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xlgrvgtj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rqbolext.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qetysmeb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dcmnybzq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vnlmexhu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jkgmyrhh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qsgasqjz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xiisvszf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gworooov.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3egrmnwfm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zgsuzogu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulhxnngf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qbcrqkni.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3limqnmkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pdhmxlda.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kxutwkir.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3omqlxbgi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zcamvwwg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qnxqnddp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pejpgpzq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3kqdzetnx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3szhjhgpg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3duoxycpf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dijjahoi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kaqozixd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wrjpkfuk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ybmtrazt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3snfcxccr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hwuberqc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyvzovyf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cnwfqlut.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3irwhtinf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhqnsepb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nrqnnzzz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3awaykutv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nxodajfp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rpwfdrmh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3venlvzee.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ebyomcob.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dnvvehfg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wyqoogil.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dosdswhi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lpbotuaw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gglflgae.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mbccxwfu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3inqoxzit.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zwrvtxwu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oefkobpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lejoqhtm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dvnqordq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxjubdzx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xfbdjrge.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mcfyjdtc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rrzkoecf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3wncmtwbi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3solmsdsf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uwhdtnhc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3eszekpal.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxupcbr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dmjgrcxa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kmehcfyd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzqnjse.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xynzuzlj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yjifggtl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uhecjlrn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qvqkstfc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hknkwhst.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qbypzuyv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ccpkhglp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3okveextw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3kftgmvha.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pasrrser.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nljysxjn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3npooysdb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvakublu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3atayeotc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfopsd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yybknbjc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mpckhuum.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3puaautjt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hdcepuzg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dcmenrau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pdvamece.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3akxmwvjd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vjflguum.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3joxcmply.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gybmtyxe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ilstjmzx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vtemvhgl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vwyfpaya.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfgykey.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eatadrrg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zaesztev.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3skunuhcf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tthahcor.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgpngfsi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dewzgqro.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ygciivda.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmmknf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fzjpbyqm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tknmwleu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qjjgualh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bahwwffi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3aywapsfw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qykuzuit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiguzdxa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pdfvtzvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gojzwzwg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xtuabzfy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yztuddjd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wyxoaqxg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ynaweljm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uvgjxkxn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wbfdwmrk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pkmdctgb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gedwlhmt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mbxmlvpg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3bkergyzw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rnorvpff.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ejjcuziv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3silsgtqb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qzzaohlw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgsxfob.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3afrxalua.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cefahego.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uwsdjuqy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3azjcnszb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3anozmqfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hnwghxee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3swtsjjoq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hdgwdgix.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lmuxvarh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cwhujxxv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3osnbtyqx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3etibsosl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xyquajid.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wrkwnynb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iburvapb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hderasmf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3axezqzoj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zcvqtvgm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cnclhqpb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hzyophcu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hmpjoepc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3usuanxof.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nrjlgsyo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ocqnxmxm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3muhyjnvt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tjliukbo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mejcrzgi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3buiyfsbm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ekckgnsx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nqqoufxr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tsxspzzp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3kgqxvqxq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nolmfzbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yjgckcyk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuhknhqv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tqwetqjs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pptgqbge.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fynulrif.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgrncjuu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yuklytfm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bxrweanz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdgpvofi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3naewtlzf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kstrfbjt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3eslfjzwr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jystvwei.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sheunazr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nazrsxgh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jgqtewgr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tkdgyplp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfacdyka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ngfaiuaq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qdzovgvh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3srelzqyc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3iffopvoh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bzryeojw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zmdsdvqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivfogksg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3rhpovcho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oejihvbz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zloluejt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3sdukvvcd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3okcrqtqw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3otqtepmp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cthyoxnq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rjzrickz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ovgssgmk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3bgendzvx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hgmxiege.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qzvrepnm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3exysjcsc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ezmsagfx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kuajotku.html

);
来源：http://www.52xcode.cn/Article/details/gt3hvlcbbqo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vmwepizi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lzgfnzbe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ecbpxcht.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hsynnetd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ysjcqofn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3oooqmrxy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3oqqaagpd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wzqosqgd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bvsyhkpz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3foanjvss.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wosycvog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hjjwwmib.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lvmesdyr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vmkthnth.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rcaemreu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3krttyjgs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mxkvjfaj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iuwlnjbb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vxsiihaf.html


<!-- 参考信息 -->