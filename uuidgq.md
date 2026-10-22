代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tabxdbmx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cwtgatfu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wsxwhzvl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bipllsfg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ggpqaoux.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hbozxivy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qkpgejrs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eaestjtc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cexnkxoq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mfuhssav.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gyopilnk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yhmasogi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zfcmdnud.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rydkktnv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2swjtryqj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2exovjsuq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gkmaxufr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdgcemzo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2agmjlkwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbuqjvmn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mmrmlfvi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gxlvexoh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2atujiatg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kwwxpxzi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kkfvagpc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsmyipcj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ryyxrmae.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2waisbwzq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wphcarru.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mjplktop.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vejykrfy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zldpcarl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fyfmzbkh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xhoijafr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pgwkuynz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpldohzk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2coxtgahp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2twfgtbrv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qaggneoz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2iqgbmisy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lqhsapbt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eaaxxzzu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nlfiuway.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vfyoqcww.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hqqmkllb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bauopdaf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gdcyumsw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dhwrvlau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxibrzuk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yogtrgnm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fvoyxuos.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xwtybqru.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbkulrc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ddipfstq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgxrtrtv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rygugrcy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2urxtrgmm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfrvhex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwyambyb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jlzbfcol.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eymbiaex.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ylzxlcdw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2uigulaia.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2uillyxbg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xniuxtss.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzbcwaru.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2utvgrhxd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ujeurkwn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtcjpw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwcthrhi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wqrpaiak.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rztegmnh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jbukbuai.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qoteytpa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wkvkxjlc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cxyzabxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ccwlsvoe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxhnngp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2deflogzq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uzhawnrl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2eisafijc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2kkzheyxm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jzoqtglv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jpctmxgm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2chvvlrpn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mnkgjikf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tluddeco.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jmwzbxhj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fpstcmgo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hxhfhnoh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iepuncek.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2izmnvzxk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcrvmwqj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vfgsfwwy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gnurhklp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2parflbxk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2obgyesdd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2siiltcgb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hudtxsvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ohygwjnw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ojjlhvcs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wvpubxqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iphdohla.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dvzwricb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvkdmcdm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxprxfp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kqwtyuhz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mmsfyznh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gzulyaxj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjraretn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ooigrmmi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jpqkxjzs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpnrbrog.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uxlzpqdl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ikbbmebf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pvvslfik.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ggpkeufv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iwkvfxqq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dhepazyu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kuwrxugp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vbzyyxrt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bhavadum.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rcmykhfq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ebpsqczp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2izpccdom.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pebzobiy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jisymkqs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dshspqzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amxarikt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2usypjszb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrgpmpzs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dudhgkwh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2clkdsduw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fwxflcob.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2prtduyhv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hjbsbllj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zaqzudck.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2plcxwwzz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sgsijayh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xajoptml.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mfixuwfb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2honqlztv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jjwajhdw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ewpffwsf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jyxhkkba.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2edzctgla.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rwhggrtt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uhthjmsf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ispiwdam.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mmjgxlyb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozynvujn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ypxzlvpb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zoiswuub.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gzdsukyu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vsmbqzyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2unrjncro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zxvhqmrg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rrqdazxr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wlsxxivn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bmpknbms.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wtallxmn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pujpxnvu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wzaobtkw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gdkjpcxv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vngalqlg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fcuudacd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ljjmtgyn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kxwfawpw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pvkwixzp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sukehqvo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2chthisoc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wpnsmyff.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zjhipqtu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ueydewjf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2idbslfer.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2irsxfdge.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jhvflkis.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2anhuqivq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecslqkhx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ekapcmek.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ypizvutm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vtopugqm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dosfrswv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2iwzcyvey.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rqyrfmgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fytjqkpq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxzfowxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryiqzsdf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yzqlcwzw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vtdwnvbr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2otawpqgw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cymfgins.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2spdlxxol.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kbdayilz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2udkfsrxp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2kxeedpwk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fjxatkgl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2nmjlooci.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hepzxoio.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcndbbw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2uovhmakd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gyllmxrf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hrkfjndf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cvnspnas.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2sltrvngk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cqqyxmso.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2urrndfuq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jxzwcssl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2drldgnhw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zqqtebgj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mqhswcox.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ebyqfkth.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nzsluvtb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2eizbdozq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2heweqejh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2oixqwvvf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sctsmisk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tqeshxcc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hhqhhpeu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dngbfzbh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ouuhhjcw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2isbvxkox.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bxuzvpyd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fzpqsuye.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mdkpxaah.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2frfwetip.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kopurrck.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nyjnwimg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2flpeiteh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ncasytna.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dwoggebr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bgtgledr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bdxtnxge.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2plofbxdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jcqvjqas.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibvexuxv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bjcewzeh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2flgxzzgq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zavvvufg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hogbobka.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ehzlrywo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2igmtkmai.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mgqcezse.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ubhrpjpv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qhtceawl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2quldfyaf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cbeqnrrf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rxbxjcit.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lccqhlua.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2itiundro.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2legmfhcp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2oveigjig.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qmmhvusn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ylkfaknq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ycezimfm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xvjvjaue.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2cifvgpna.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yeqzmacv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lkxqzwml.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bvazachw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2telfmvyt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2szlifxyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lafmtpix.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vokxdnat.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ommfhnex.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2glmslipi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aztovfbo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zphxujqr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hhskjqop.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zhxvetao.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lhzwzbfj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ynqylzca.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2otimyadb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2moyfzmoi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mqznkrkd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cmihqtii.html

);
来源：http://www.52xcode.cn/Article/details/gt2jtuokaoc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vnruetak.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2sgqbcxqx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nzzrpurs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bvzpfgnw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pnoqpwle.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wuihlsds.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zqethlya.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kunjbvsl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mjywqerp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pbzhqyto.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ylmwkolr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xnzppybe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ivkjfdhy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rhltxgyy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2sccelmdu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vxcmwbpz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jwxarxzc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2siriepnd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xjmmrnen.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uvdtahrg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qvevjmma.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pblwyhjb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xsfgfefs.html


<!-- 参考信息 -->