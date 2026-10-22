代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2uxypngkd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2zaouazuw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vzvaachn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hvekjovw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ykqexxec.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ylfqztwh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ktwhlivu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tdoogdiv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mlcrqbrg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qjuuswni.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2aylzfhpm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tvzwfiem.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2avscrhnm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2prargcpg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xrxmdydm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qomojqxk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hfvwsgny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfzyifep.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rimnvvgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueiidsef.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hfjuwili.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgnhvwnc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dfksrzvz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mgsroyfd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqfujw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wuldeakl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hixuwcqj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zvxdcdlq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kodxvvmr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ddhvyxyv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zwcyuasz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2scbtsjxw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcsuoubr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xopftbpk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dnfsyeby.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhyfwocx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vqjxwwyd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zrfifyyi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2sfhohhar.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vgthtucu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sytpvuho.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2scfpbmsz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yksrsddw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ydyavylq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jdvhfagf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zkhzonsg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fwcyekjr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pnuzusox.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cdethfhh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lbnghbgs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dalrtkhx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvwuicec.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwlxfsi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdsmwrme.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhcrsop.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cximopub.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fkkuyjaj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pzlpbetp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2whezriey.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eyrdnlfo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2emedsruk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pfshpial.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2orohygbd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fsdatxeb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2cwsnptas.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qlifslyy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dmbpzkut.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gsspocka.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vmkfsgwh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tntzmdiw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mbhkvznm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uwrbnjze.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2anuwboir.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cikekanu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wvvwxuch.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sxnaxnsn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iquidkqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cmipaozr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2davlvvfd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2iclaztzl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dgvylaff.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yeqkkmyh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ygfszsny.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2trdjbrll.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shcbofsa.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mzdgpemb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aqyabtwh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lrvkjtti.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ashoztup.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yaykbavi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qodpclwq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oarooqof.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dngysprq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mhyaypzb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2csqcfjvl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kyopuwyv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mcgsooap.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qhrxbuse.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tdgauwwg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nuctptwv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vmufsbfl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2irpecumb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qqmuryjq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qsxugycx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2whkjzlyp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hwhoqyns.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wnjmjhsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mltvjrdy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nwaufblk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ksvhtwxy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qumekcda.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2axvpzczt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mubpcbua.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2afiowsfa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fxkotzfx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mmeyerpi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cvkjvgzo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2egnfrbsh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kqwbcfiq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rxaqepof.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dguvetta.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ibvkgswr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dyfovqap.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tlhxedoi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vuoupeym.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kgbnxbmf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xircisxc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qxpxrdwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ducbisro.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jgrapggw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyofuejn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jioenrgo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bylzzpfh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bqqnzoxh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2osiwttpn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hmoxvpws.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dloeypfe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ifbftixb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2laqjufau.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2erwjyzlc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xsnhmxfw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqgddyt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mtacbckz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hxpxkuxj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rhbvddmi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ylzyosjb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fgxzhonc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pdjqgord.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ysyijwwn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fnltzrww.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ghmrfiad.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kzfyttfx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kxxnjfvd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2itptuimq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjowagsr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ckboxmqr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tpqkyjil.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzxwyhgw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2knldbobz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2brwzhcje.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tiljyiri.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pwklyvcd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dehadfup.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nzsvniuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ebnuzcye.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tldecasg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2orxvuttd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bqovkzub.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wtdpqcek.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2sktdmsrj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xjurtlnv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gteswvsd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jgtrmehe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2nenghlqm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yjxynbcj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ujoqmvvr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2djahpvdm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2clamkmbo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2deinjsyx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fnrthbft.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xayymnez.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tyrwsomu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zvjaxhsz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wardjrzm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2lgfwewjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blluqxmg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzcisnxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzfeprif.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2khafiaho.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ltdxndnq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lqeixvka.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ficsifnb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2muuviqhp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfuecwjf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zujndbny.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dnspaiks.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fgbstphm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2spnodffg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2iznpzxyh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zepedrwb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gpnlowuj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xbtslsbd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uekfhqpr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ejzrpalv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2trnobthj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vfjjizwm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2avccwdwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2trvbsavw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nhferyez.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcdfqjky.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wofftaww.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qencuiif.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2skjzacmd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2upnlopsr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rglicynj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hhjbxyeb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pajtrbsp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jlclckeg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uiqnxxqc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jodmjbdb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2psjzuiey.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jxxozzbf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2iqbngkck.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dbkazxil.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tukvqinu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ccvzlvux.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nbojjyzh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ubetbuxw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2amjehmlq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hneslera.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xohsnnxo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fxfaenmx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ystiplfp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lapqnbqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2obuuqnkr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zztvherh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ypgxysql.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jinhblah.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afyqgfmn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fnzpzlbv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2yuaghunv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiufjido.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2glknjfdi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bhczwssy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jfufvcgs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vaqpqxlp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zoafezaq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yavexqhy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fvfffkjk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qwfcayks.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jncehpnn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kjzopuxz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cemqgivc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2sucbbaev.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2orjkwvyd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsfpqsx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2eychcbqm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2luzcnpuy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mxzbbyns.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cwxspchd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfbsrtzo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xjgojdgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzycemiz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sjkrcrwh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2crkflcja.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jckxogbg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2loauxpnh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2evemuudn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uaxvimll.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2skelrmjg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dltdemcn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jncnumqy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xgfkijrn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xqbzgspt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fbcvgjtr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lzhwayio.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bgslliqi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hirddwgn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2leosdasj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rzzhgfds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ffhqzuex.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ldhrmnqw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jwtbccwd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kpkkqgri.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rnfglpfp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ggjyccla.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xprjtspk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrnkofpc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nukazjwe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2knolwhvd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zibooicd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lhkwhgob.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ezgxlapn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wcrfpvjw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sxuzhxzu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qwrglbqw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tgqzogsi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gcbpiwms.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gijhuwml.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2znlmjnxz.html


<!-- 参考信息 -->