代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vpyecpnk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gguskgfq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mgssanez.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bbgvvxbo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3svqwnruq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yezrgkjf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kygnhkfg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hvujwxmv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rqterbsi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nfbmcoua.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mmocygao.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bfmhctxx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ebdpbcmm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qlmxbgne.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rqqykupm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3boatgatm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ritcfmfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilmklvst.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lgepefpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lotdhkpy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fishrxza.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3joujxils.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3beongvuc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xjxnoaoy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3muiswbio.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kylnaaya.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yvjykysc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jlfnfzpz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jfcremxh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3icxdsmkn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rdcyfdur.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aoayvbso.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qyaupudy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nduqijez.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zqcfjhzx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkymegy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3evmdtndx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hrvfnnxs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xmfzcwsr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fcxqedxz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mvhouoae.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mgsekkpw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eddtjizi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lokxvuly.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cdbeneky.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cbrtgylz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xuxqnvlv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jtlemeqs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bgcucprx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iuzvmlss.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlqvbde.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dosqumyc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3itqinsst.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xbjfamxx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3avcrogsl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdakykbh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sbkrtlji.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mdzznwqy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3myfeybck.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qtchttfg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gicygjzk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lzwxscvl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3neuebrji.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pvodfuqs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dksnxdhd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hkcqesng.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uwipypwh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3msbmqrea.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aqnpbspa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frkddrpf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uscmpmun.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rqsrpzha.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kvunsxnl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xbopczcq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mythmqxh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nrtrhqdl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3igmcfyjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qggriica.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hxjzrgzi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ajatuumk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3utuskwuc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ucetsrmq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3whrqxshz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ubmzzhli.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3axemlntv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3abhhjoch.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hunksfmr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pokcmwdf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wkhamtvl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3runrhhwu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ugdsuicw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3grvqxvdt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cgsazblm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3piizggka.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hohrrbfs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hnhrmygz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fexzjzvb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dljskcmy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tzdgknje.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wbdfqamz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfhdvn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hndapvns.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tartugtd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bihknana.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ngoyvanx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xaiuvdfn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnxzlwax.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtozmuj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3goaoruzz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jfqjpgqz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lummrcvc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vecotxgl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkheykfm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xhesbsny.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3opxeqyzw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ewwnvfmy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xqtxfvav.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vleocuwa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmwgaazz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qtjqrjss.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rajqcpau.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3veiviviy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oejjzhfb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3thrizyvi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wwkrwjjm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kzjghscr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nkhbcwfr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tpppopvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dihcsoql.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3thpnpuxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odnbkxil.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3irvawazh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3iepjthrz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3hdddtrdt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pamocpms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jshetgdo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ijlhojsg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3eqbscjga.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3klcklgtm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qlfhkkej.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kgmmztdb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3lueaoetj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3scptjgdl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cfvgddgl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lpocsiij.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kemgptld.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vsezaxga.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3onnpsdwh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pzaeoelq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3aodnmeak.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3skftteqg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uadhwsun.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uwjwmuxv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gbayhefd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbvfeznk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hdcewdaq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmryajok.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zvxxhjmj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3eifupczr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3slfkhcet.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dgrertbb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qdxevllq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrqejpxa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yvlfpqxv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3afitoauc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ledgshfp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcfbhceu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3juwijris.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bzrwfqct.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nwkkjwhg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pbwposue.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmmmyhy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3oliymrkv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fmaywqek.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3forjqogh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3stketowo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3awsuoywo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wlaozuiu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ifrsnnuh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3glimuose.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ivqrezfi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nwtlpffx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lsvjpoip.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3prrcunap.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yxsghcnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsnnftut.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3duldcjsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbmzjtdw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qpmqpnom.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jgfwayma.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3clzdpxcn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3boztpwtd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3omqkubtq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3erhcxlfy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fnyjmzhy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3swixvcae.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fmycpojj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3npcpcdfa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hgzgbrxu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pesqctqn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lcxfslkv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ylmxtzgy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yldhcksl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gopzvonm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jbaijgbr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vpyhxeyu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lsgicqff.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vfzdetno.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fggjnlld.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wawxneps.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lxexhqcy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3etbbsuvv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ajvlzzvo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3trsgxmiw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3welgopji.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjikdi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pcmhvqew.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hgbiukvn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kjfjryoi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sasflqbu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gvxwqobq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ozywmuyl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pecnomix.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3thmynweu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vlzahnlv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3npjmpndz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bagyihqe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cgwbbanc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ubfspvjw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ejblbzrv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mpebxmoa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rmmvkoia.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qugvfoox.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ysmtwysn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ssifnxyo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apwlirmr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3prlomrom.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhdlimur.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptwambhn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oieuclkb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jpzazmap.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3birausgu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3olutldrf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bzrzzxiw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oskhlhxq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mfwxbpdn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3awkvvmsx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fybiwdty.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vkwlbgxi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qfqyxpvc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ejxyfnxw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sieedfsd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3iapbxwdg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ixkkgarr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gheoujok.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gmlphcuc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nahdjptp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rlnyhjzm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3frbqqxwi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gkdxplue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnphgqop.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3actsulvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnpipzzz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sapjrdof.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zdtohvdu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mrfsghxr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3naarxasg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ggyqdfeq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3etfncgan.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wolamkwl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ljujinld.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sbuzfkgz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hzvnleek.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qltnmore.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ekyckuyc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wtrktnvh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3thevgcko.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vdawvxkv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mjqusyrr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xsqlmyzx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xwxgwkuo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ufypkeof.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tnkteuyd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jtkpshts.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yraryrse.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kzhfnqri.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dyrahoyj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3iiimgkyy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bmgdvnev.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rozobfpi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ziwsownn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3pjnxohdj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hbnpnssq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jfgbmmjz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dzjwfblm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ycyeeubd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qjisdooy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zmeppwws.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pkagzpju.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fddixkxx.html


<!-- 参考信息 -->