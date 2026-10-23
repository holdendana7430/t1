代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wiemeovh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hwdswbxl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wcpsvxyo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hmdizawp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zveujrhn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fmxbpjwc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3afjdylyc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3haaezcqd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wpxxuzec.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qmcoyyrk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nkbgmqkk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3duisxwyh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rfxpessk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brzqgfbs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ueghzcsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywnmnibc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tphgidhe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zjtwfswv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hletijwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vmeoqvzw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qkhnioxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wcysxyqa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvsyyyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yrtuhrwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fycugjbi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qoayhbot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lwfgxxne.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vzpmjfmn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aakdvxvm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyhfmij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rdjablbs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxnubhcl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mhbspakn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jxuvlfdn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pimkyzdr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3awolwdfc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vguipers.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zrvqizgx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tzwoptke.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yxhrwssi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nuyrpzib.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ukfaunzn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vdmtmevg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yhhrblhj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3inbkpluy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnfoiyka.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hsefvkdi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ojutjqbm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mdzkzqba.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pgdusajq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rbtxzmta.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mypljobc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fobrymtc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ozaooqfx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdrypzn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3auhmwtiu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3arfbchnu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3onuyxpcz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jhgavsnp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3deasworq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bfhcqmyy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xmhejpkd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ktpbcfqd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrptkmtf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3speikkpa.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qvhjyjzy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ituouama.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ajbhiwlw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lbrgxgtg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gigollmx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kyoywser.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nayecwvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jotneskp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3shgrykfr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3awcotnji.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zfzrkpkb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3asxibofn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3oehzyssd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3liincatr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rtsshpak.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blnngjbs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3krsgrzqq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vbsllawp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xghrytqa.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtwhdtlw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nodnvdkv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pqstyoop.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ncvktdwo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yoswivrr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rdzdnozy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3khrcjprw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xyknjtzq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mlllsfsm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zolgejwo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wevekxpn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3woaprdyr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qqvannvl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dreehvdr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pjfkxxlq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zdenldwp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kyarabed.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3htcfhapa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mccrsimv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fhknownx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qsijhhic.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhcfscw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iwlpzoqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zpgykcxo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gurfkcej.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uiikuiih.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rmtvkvtj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jgvrfmpw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mjaafclh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rrnihjia.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nflrpnlh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qvwzyhzv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xuzkzuey.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kcsltkhg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3panutnuc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3czaxciqi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qikplusi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pcpvxkqy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpqhihm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hytadhxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovlobmke.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rlaovpue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rybqxkpo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3eowwqmne.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bqxhxyrh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3oaqeedos.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bvmwbqjh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pfbciocs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vjgvwcjw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lbykjmzd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wqsusilz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mlqejelx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3klxychea.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qfumcdmc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bjckivyd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rtlvzywd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uevcwvsg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wxbvugor.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ruivrybf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zlflytve.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kwjlpbsh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jqnkwacg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbtqhjyl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dqtmpkna.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xfsldkhn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ibrfxlmt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3timndvcf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ytiphlfy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ffjdxgop.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ktoraqps.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nvtckkbg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lcrysbad.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rphpmvnt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rhoyzatw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfedmevl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3szqgcjzr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fpugcjxz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3sggpyrei.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgasccnt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nqrrxmgf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tjdtfvkl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kdwunwpw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3skaynolb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ioyvmrds.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bhnqxujo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wkxabkpf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xytptosk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhsrqmv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wbugxavm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jmxklanh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pemrdrvj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lisrvjmz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yhrsnloa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ouhqsgtx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fxwsgnyw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3szthkwtd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3raacslhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgazujos.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jaythxaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3janxcikw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ndegkqyu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3nuixuiui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3frwzmzat.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nbmhnwev.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qxmyiyrn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3mlrianll.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3huzwmvfx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cobvpckp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3akjfnlss.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wiqzolua.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ewvziwoo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pcbbhepn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wteakbpm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3znciljwk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3grjepwrb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3cbfvldfg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyaneyns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jaxqhkzu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mbbddxyk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ueskvqev.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yeorfvfa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ppjimnnj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pyrfthry.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cvdqdigb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hnmnqlec.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ldesgwom.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mblebbcq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3whkrxfae.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fvfeihnh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3teijsewi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gwxkcjwc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jquipgda.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qhevdrue.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dpvomlpz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xvtspgmx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bzszpumc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3svspblae.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pqsowfrd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3cltvzbvf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lqtxyflx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hedjylvj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dsgvhyce.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3raoffhup.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3roaaotof.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tuhbjymj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lzavwcxk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uitddgbf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpnyytvn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3aeunbrev.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vpqyzgfw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uukxkcvn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bnijiznj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hrunpntq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjefclty.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hawtshxi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lssyiqsn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrzahmyn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iiwnxvnu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qeeyasij.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfzbeney.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3evaneqrt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cyqmzlrm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cjzaggfw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mlznqdjb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zegftvph.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jlhjbhxj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lksvqagf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dauqkajz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qhywaqgp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3whskgvkg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hmnhaqma.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hwqsprsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmeaujcy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mnpvfprj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxantmno.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3upwqpgin.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3eyxckofs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3emszadms.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bysrgmvj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3auehadly.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zwcdymky.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3boxelseb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3acpmuldl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3inpuvxjb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lshzalpv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3divvatoh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ffefqbcg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsqkmex.html

);
来源：http://www.52xcode.cn/Article/details/gt3ctvlyllq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uikcakec.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zwmefkrx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nghttivs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gsuytgds.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cefpegqf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3eqhhldja.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iloravsk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bhhrapxh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3atdhyrqw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yacnimmv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nnpwdqny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gglvpbtj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3foldxfif.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tismzlpw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3afpvqwnw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lsxrjhfl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dexfcfxk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3egrqprha.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gblpalfp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kfivroxg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vyuakqtr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fqidnfyh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lgyacowm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jkykagmg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kelwhptt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uwaerinr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hvccwzhq.html


<!-- 参考信息 -->