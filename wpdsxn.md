代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3trszrfuo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ookyrnsg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ebetybur.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tlyqbiqm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mzpuuopw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tqdodast.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3frkocokf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hjczszlj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pprtlumq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3whmlbxlr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bpceosrk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jbxyjhxi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lgdubhzq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xnuogaur.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ayusqibw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rhavtiyu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ejdtutet.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ikpwhrtq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jqejibky.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lplmiuuy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tclgfzwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vymutjhb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cjbjjznj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tootvsvn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3vtrfsppf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3csldclhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ypzeoqvj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zhbfqepr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3czukgppj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xqcfculm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdflvjfc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qogmkpsx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3furpuczp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3upjioqmq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mbtkyjvz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rtxqeijg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tohmbfyi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ezuzxszy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dgedikze.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llwqinyp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kjdaegfl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dzhuapyo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pfhuefrq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gmnaqauo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vdblqsnj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3acdefrkt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gshciipc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zwffixop.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nrsomism.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3elsarpgr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zminlemj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ytwdokxl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwltwzic.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieoyrpkf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lstkzofp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qtjhctdn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmksbps.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rrwxdlkj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3utklbamn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yxdtjkyk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nhztvfpb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lqhxsbnk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjboafwm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lcwsssvo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3losnbatk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bhjslitp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fqzvdgjr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3klbiyufm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtkuewq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bzhckwxq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ksmmvpqv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3afublqrr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xfngetdf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ebycdrdb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ppwqkmba.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wyqzsptx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vwgfocuz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qgirrtfq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cjsbvfae.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cazrqfro.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3oijjporr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ccwtylip.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3eqrfeihm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qqmfkohg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pdjvtjbo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3oybpagif.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3frvajmlr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jgtortsb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stimvxby.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qnhuiejx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3foudwpso.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aloihmju.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vvxokaws.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3chnmxddh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rkkczosp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vuadpucr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncpafsaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mouhuvlu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zuqnkcns.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vpsrjaia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3baqewypk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iymtwrtn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3iezywcio.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qykqqbpg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3olsmmnmv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ifetmvqw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3iqeysdct.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqobwaa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pjsxzaxo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ybocvgvr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cmctgtyo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hmrtanxp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qiuvagkq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vejmqxbx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mjluhqkx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3drwlmcbz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zylfutsc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gthkfymq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3flmzbpit.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ibwmyqqn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3udszdgyg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vlkubslb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wivaerky.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fwbmfqwy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vskikmaj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dwrbhkaz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vxfmpkut.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ulmedxwa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lrglgbxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xzefccra.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qiiaxijx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bidgxham.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwkhvbzz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hlhwkcil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smlejfez.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tcefadga.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vvrwvyue.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3stilxmgg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hgclkezz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tkjuclbg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rrybiysd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lojaqnyz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dcqguzyn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3amfkgaoi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cobjexvv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3iopfzhgi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3enkdnlov.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3frhfvvyn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3znyiiwps.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uxfstaff.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kyuapbta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jfgrpfnz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tulhhfdz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3oiilysbc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fnhpgwci.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3tyttirsd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zpanlxqs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zjhxoevb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qltevlem.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3whvwjdkt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fcoqqhms.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3trvimqcs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nzyenqei.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lzuoydsi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ubeqgkqh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sblieowv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smpbvtxp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ardyhbiu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nmuafeyr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yvalrmht.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3imeqnlwa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rpavrljb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ezxrcenr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wufwrhfb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3azyihpoz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wbjylvum.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3smkzhtqv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3emhgacgp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vhlkjpfu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uaklgcrr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hlzetgoq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3llitpyyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3szkfekwj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3avdxhzib.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xxbgqpow.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wpsmjjaj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qyqtowvh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hzvwullb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xseyuibw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yecbwvus.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zavylrrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqdyyqcb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uimxkvgp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3aljviiny.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3unqjajxg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tqjvjosv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ziesurkw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3eotvnuch.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3baxqdcuo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yvnwdggo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iwfonffv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qzuzwsdb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fkrpieub.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tuapbypi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wxfrmbgq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pkporofu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mdvmbtnu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gkklxosi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oytfgmnl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uebdodwu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ycugbyuy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3llljxulx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pdmkbsfg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wnwifyyt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qxukbqow.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3smoyuuym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mmmtoyym.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlnammc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wkpyctej.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xrlnsswk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ecprketp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3usmgcawy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qvqltfvl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ndyjhcpt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rizhyqii.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zkefirtx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3biulontk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fxcrvalk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zrvpdvks.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pkqrtiat.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pzllqtyd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bwavpwus.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqbndud.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3cuvfwojo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3swsjdbqr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hwodxmar.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3quzwntrr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3yymdylkm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ykpgppql.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eymygvxt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gyfjhggc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3obgwpomn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtkxbvjt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3chshwgbd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kaushqhx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vsqwszha.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vmxjhpjk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mthwkrry.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kwkyvvuh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mvlrsatu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fqambhkb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yiehmobc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wyavjwsz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qiqlddij.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mvjujral.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xmfukzol.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zhitlfwf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aguaxhqm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gadkcysf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iilcpbwt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cwjhqbin.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xrofsrtr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wotzidqg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3snieobyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrljsvtb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jjthwlbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euiaolzn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ucqfzaan.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jcnuetdz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bismupmc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3aalgnvyz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3oeaolmgv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ndnhnini.html

);
来源：http://www.52xcode.cn/Article/details/gt3zbwuaack.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wmqpiqij.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fheddsmw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pyiyutgg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hraiehbb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qhlqbjci.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3avftwgdz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yeroowfy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wxaizyrh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rpcxcncj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3otmaopjh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ejqrbqdy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3amqeniec.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xgyrftcg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kgiykgco.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wzryttch.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3npyumydx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qnztwopq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yxvjjbkp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcpfds.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3iiqwvzyx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3edgxmhzj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tlccphum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yhlqygfz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jxqgauzq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fmiscnkj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yijbnrpo.html


<!-- 参考信息 -->