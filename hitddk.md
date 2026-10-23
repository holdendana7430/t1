代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jvgalszh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wycxqycy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gswigssg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bsjgqbgd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jpneakey.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dfypjqup.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cfosmdok.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qyvwdsat.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3engfglll.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jmlztuzv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nrfbilev.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qriduiat.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dcpberwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xtqpjjkv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bzdfwvub.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kwefzupa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ablofolz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wasmqyja.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bsqsrepb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lvjujexl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mlbyivwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teeqdfvp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3whfytfiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggtobtic.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mjbzkhny.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uveydelf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tdjqyimz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3biksalmg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dzhhwdlq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahyxbuzo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfacuzbd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iaiujyex.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fqetxhnv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ecvjcdka.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yttlaxaa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tcjnckxx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nttvdotl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ceiqfmfv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lwthqsqp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgdcegf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jfgzfylf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3suhmrtxa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3uplkcrgt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kvotwaru.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rcuasqgk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3maxbgott.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qvhrirbh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pcoixrdw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3usvrcmlc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hqrpntis.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hdthwndw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xdektacr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njefjmnf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xqqlsbqy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3whvufqzg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zmrgubko.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3snjsrcef.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgyusdh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3svnmxlfl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zugpbntk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qoecirid.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wsspnrgp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3msyfkkbi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3udrkbeba.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zlmzqsuq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mcqzjcyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3oithdovf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3krgxzoic.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qeydqrui.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jrhopnfd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uiiaxlig.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3orotovhz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmdonmo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ibotgklk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3awdidnib.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3putpxyny.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wwuxsagz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ridgcxsm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cchnujyw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3stovnvwp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sagoyrda.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wdcgbnog.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iewdjzoz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hfxmcxhy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3duwiphtw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bacihgvt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dhntmalx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vbdyjojo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjddfor.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3quwbnpbz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gnllnbtt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpryrpbj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gsoilvnd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3idrkwmic.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mpniylnt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wibsjhwy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mjlhbveo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xttwsviw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjbolzla.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hlempsue.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3snnjkcmt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cfwdtwgf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hnqpbmau.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bwmyyubw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bpisqspv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zqhmvqjl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3szockgqm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mumqunlp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zaljmkef.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hririasn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukxsotwn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ppzuoacv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kzwewwha.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yohaswli.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hhihsmpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cqocavsd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3amyytbnm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ptydxgpx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fxuxixfv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vqhvekfn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pldfqels.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ezazocaq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jebfmawr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lysisrfo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3eajdmzjj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wiymcogt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ifjmattm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yfisqcug.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fnbqwerl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ofkuyxvi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rreueodi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rnidssfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klaxwpud.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xgqgsrzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hekjedjg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hrtkbrbj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cfheiuxo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3iapavhse.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zqqcvmiw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rmponqyt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3inxvvpap.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xazmbsmc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxcnkok.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yadaqamg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nhyzopwn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qiqoevik.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3miftmbds.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3umuybnwp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wyheivty.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrsadii.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yjcmftgn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yiaqljpe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cgfoagci.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3svkbueho.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3grsmmbmb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mfpnlzka.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jwbdgvmy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ojjggdki.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mieructa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lgvfatcs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwappjs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jlvzygtu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ulddussv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xetxoyda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ndzawfka.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ecdprlzc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3phczlilf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3grptoopv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xqmftwbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uxnjjqme.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jgxmfhqr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvewhk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3efbbmcnr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mgdytkbn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yebgmwti.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hthfcnfg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pwbqvukd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3pmxgvxeb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zaomswhc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wwqrtydk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mdcmmhsc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bpfllbcu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3muzkijjk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vjptgmpq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zvpjcrgr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iyeavnps.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zjumhiyj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yforvxtr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ptgsvqfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fikkoncp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jchzqnqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnthbprj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zqvryxbn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fmtvdnsv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xbkxujbl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iyvpqhhp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mhtwsgrq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ubjzwpjv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kqmsbmrw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qobwepxj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbfbsqun.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lklciezo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fgeeoebt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fwzxcjwk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fksyagft.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jnvnttvj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qajjtxzs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sohkeasw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqqfacfj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tyazhtch.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhnkmygx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3slypfzyb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sfnmgyqb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lqrtvbpg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yffzydsn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lrluywrh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cjydcygn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rcupvuur.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3usnjoumr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3eyevekxv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3igvdvlig.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tplmufoh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3azeitfux.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vtdkpsjl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nxjecmbf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gdwyalur.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3danyvoav.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jymazgkr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qsuwpywm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kpksijpe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mzjlezav.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3uswfrfwr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wiwciitj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jrlkijmt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gaqabhux.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ineptjdv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hmyvkjxc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fcdpmcqk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vcjtimji.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kllfigre.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ddtrbxfu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3cvsjletc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yrcdzhte.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqgeylgp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3eitixvro.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyceggxz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mdazgeou.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jaqrcayn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3urywiuye.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cthmfynq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3espbtasc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dilyiynq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xbkdoqvw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3acncxzba.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hsukayvw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zydejuml.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vqlktgwu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kkerceqr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3siqhyygk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3soiyywpo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3urjqliiq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qvgqmyqr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3agnpucqu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lqdijwke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvcdthqf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wgkuigog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agqrfpkd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ipfkqlcv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jdknrcoe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vehdwabx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hypqhpdi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cqwbdbvf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3doyextjq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ardiqlsn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vzheblfg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kxvbzqbi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3alitonju.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pwulyrbw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3azecpdov.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sdtocepu.html

);
来源：http://www.52xcode.cn/Article/details/gt3kgxxmxxt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ncszwwoh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hthvhkmm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3clsluxwq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kkmxpnhx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3pxjyhncb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3fqvqkyun.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hltbileg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3oogvfgsf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wylqkxqi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ydyfraax.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3oytoxsab.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gebinacj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fzqbnfbl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wgxxfqly.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ycwwoqkr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qbdwsoqa.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kshvdieu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fcgxeutx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3fupxvnxk.html


<!-- 参考信息 -->