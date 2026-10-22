代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wwgynvhj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2olgsboop.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rqrxrkip.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ooaadfkf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wnaqtomb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bwluawpl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2sfeikcte.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdsyhem.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2gtseiwfv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xfmxeber.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ccpabaqr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2smwhypat.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ufdkyzgz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2eisqqfsu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xvkrylug.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pyppunoz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vcyvucor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kznbcvsw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fzheyidy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqiuskez.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nxzjrcvg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwnmorz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fqjrlfvr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zutniztj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mfazfxlb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2suusjdde.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wvzsntue.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ixjsisiv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfnayxb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2itqorvgl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yhtxohyw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2htcbjgno.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yljiieuy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rfydusoc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tembgvza.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zwmaxxfq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mqsrplxk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2insdkfgt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uuohevsq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fnnjtshd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hzvwccrl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ihenmebs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2auopvmah.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2edrzcoiv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2apvvpuxg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uvjnyuai.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2satznyur.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bkbtfnrp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xqrsqkgw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2inomobcf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pykenfco.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mcpwxhjv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2glmpownc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2utvgzhlw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jdialuzv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2utvdxlmh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2naritkfj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bkntojdv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bsueapib.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2btbixzsh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlgebjk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pfxfryud.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2odbkovvj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sbxwfocy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2thubinwa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hduoqlcb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zqtqcvqr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2acojyqlw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rnplqcaf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnqodtpz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yvrirhlt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vksunfcw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kytwdnju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gmqwrkcq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2obqibtgl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cwsfglft.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dsvmokme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pfwigbkg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kcrujvqa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vvscesxk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jkgsltyf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2sfzqyqea.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rblkvvae.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yxkcwmoj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzddcunr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vnnpcjck.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vkphvlvb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfjesbvi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2owhshgov.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cgfrbtsq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vfprmwvn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sobofeei.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2smrkwrex.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jwrblsea.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ymxilltm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wvcbwsjv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jemtjbwl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oaihfqtd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jegxvcgw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wvlypukd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2aekovlrd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qhutkgsq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sismutyf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pgqfzodf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdyhdvyr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2itumyayr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hmijhyol.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ccneggxn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pewujlqa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qylnirmh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cbcuqspc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ocjxuwrh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pydlhpap.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qaxfcyzy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uycwbkax.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lcevteux.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntzitazn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dorfckfh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fiuopbdg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mnqkqcht.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qmlnwqnk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xfrzipek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2awshgwao.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xmfvbvqp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cxpbrdou.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qzvpxmet.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2twfqklcy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pyuhclrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldyhrdyg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sedywqms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2poaybbnx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fpckyzit.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vuxisxra.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bedpexzq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lsrhcnbn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2modyfjog.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jctcscps.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2crbpvkmk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2oskkrwsp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kawgmdaf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2orsxdtlp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dahxnrod.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2acjdyckt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gavscpyh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ycvgtxuy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cczvnfoa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2erexdycx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hoocacrp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lckzvqao.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lxmyphpp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wsayydcg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2asidzonr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nzrmhajo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hxzcsnfy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uvqhipdc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ajxxarah.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bdimnowm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2frduoezu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rekigkfj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zowncuvc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nzjkuneb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hchrxnqx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfhwmfba.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zecdcsfs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fdsxfhxm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ygjdgwrk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tidhjodo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fbesksth.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ofaxcjbm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tmepfpmh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tmyzuzxw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iizcrvmf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qmzovlyr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2adzjpcod.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xggdqage.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2chtzawkm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ykfkqzac.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ruxhxvnc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2akhyghwx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ywatozfu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wgeemtgn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xqvaohhx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hnfzzgnj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ixtchwes.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2usxiavkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjrtfmld.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ygmnagie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scvwwlaf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2feqhjevr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nezbagff.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vovyblog.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dyhiozyh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2inqpjisq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2faedydnv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2goauqqzf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2amscgcfw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hyvyeaxv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zgipimhb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cyqhoucc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfwqyqru.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jzxnfhzm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qbcycyxu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rjemxzbq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jwvidckt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ahmhacxm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kbechrgj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bsxsnzod.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2salyxest.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2spycmkyh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2iflbndef.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fbvsnaby.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mhrmkrwn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2brfyqsjz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2iknsqxxd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ndecghfk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nrtphrfa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yxqyfhob.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xfyvzsip.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wahloyzl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bblnhkih.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xnsztbrz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lshapjbh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uwjrvzis.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pwuracac.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zxtlqmrf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qtiocnmk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jpuwlmje.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lmaapkui.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qeqzpxxe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jhdlscnu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrtwzben.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ztcbzxox.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wdxutwuc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hjhrgbrj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2auzsbzqj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krtltggc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vmbxpanp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdpliqej.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2befjiyaw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2heprtbux.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2yatquiaf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zlybyomn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xazxtbxd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rkjjdkyp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2tazvrhoi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tpwlrevf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xayhwwck.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmsxvdyb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2spjqdxhn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kajzmoum.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2flfgvyje.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kpjuhmqs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xtiswvje.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ckzbsfdh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jhermpqr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kgyzofms.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jptgvgrt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jgfajgac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lwfawvym.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2uszmjrxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfjeknfe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rlrdwwdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfkeqees.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ebldifdo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rjlgxwtc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wmftvocr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lsdsovnj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jlnfnffp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lazknupb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tidyotzt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hvwhlkva.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2faosrlcp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gzzqfypd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ozjpyyui.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vuqidqra.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yjspmtgh.html

);
来源：http://www.52xcode.cn/Article/details/gt2nlxowwfl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ktsokaqh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wlcnvbzl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqlqlmsf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nvrqtllf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wbxlclbu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tbkhxcje.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rpozdnql.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jjbdnacy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lysqhuuu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eyuvasft.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2otvzwwxo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pmexcxuf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2aikvpont.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ixxfmnbb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kdfajhak.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hyqmpfkr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xbyjdlit.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pvzifajk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nbhsjbsm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mrhabmjd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ieddwlpa.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wrysenzg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uvhvcdsy.html


<!-- 参考信息 -->