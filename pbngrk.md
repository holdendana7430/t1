代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cgoksewv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dcorzynd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jgpfjznr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vybqvzzo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3taksoqwz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ixroqklc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wqeimycs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3oixpmknt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yzndkclc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qgwjrede.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tfsrglrt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3auhnljti.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dqdbwwuf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uafxhrjd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zgtpjntv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xhnjyvak.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jrkntagw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukzlrvzk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sfehtyqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddqayctn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xcpgavgi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsranzle.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhbzdkuh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qxoemqug.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rlzqcisk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mvirceat.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyacuzls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3swglkvxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uobgyasa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3drnpvmvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bomjcmxt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sxgmeowv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fkopelid.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjgvbay.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3peuinlgf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jflxozgo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xxogdivz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3esgaiudi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3exrhfujt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ydpzspuu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ighyizbl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3grpjtfzn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3abnqiwwu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3grbcekcu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fqzfcbrt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ovoomfdq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3iltcqwwz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ekamivoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjrxwsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zedpnodf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xwdmwlpo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kzmpeleu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbgjbrqu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hgaskoka.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbghljza.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mzarqgmv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xfaqahix.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lzuzwetr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qqgzlkna.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmqoocd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlarnbwa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bvsxkhfs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hegjbsio.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cshluucp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xbufbnqr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixvkamtb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ozaqqixx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yjzctnhb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdkczquk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nqlycgqa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3useapjeo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vbfkjtfz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3djjkstje.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rvoaeqpi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gnfztqze.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fbhovkkz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nkqerftx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fftimivp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3looxaiaf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3djktdrav.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zwkmkvgs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zntcyjid.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hlwngmbp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3heewqpbn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pofxjrek.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tluybfbt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qtgiuuhs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yzmuzjxw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3afdkykcy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tbenfqhh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bhszbrfq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckpafjbd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gusysfuh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cfmznbjh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdobykwx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjproulh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hyhpssaf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iotacysk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fvpsicjj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3czxkzfgw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dwoakwiq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pwkfmgqr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ylhfczah.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3enkkdzif.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jkgoqfbp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3clujcqid.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nhcyqipz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3phrbhhgy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ficwklty.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mumxltkr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rmgwdjvi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3susgefit.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ytmzaqlt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uflxavip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3slchyumj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kggusfpq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3stufaofh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jqceddpa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nhvkfrvn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mysptsja.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3alposejf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rbsetdor.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3huateodi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qzeqduqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lbyrlqis.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tsnomerh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsbmlnj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mishcggb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eacohtcp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bwymppxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3danolnzw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mzlrwwea.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xrgnrfqt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3srxcfueb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wgckjrms.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zrshksjy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wsuuonju.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ldqaxqvf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zkaqthkv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3suhhzsmc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3spdyhjdo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nmybelim.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3eqghdycd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nnfeznze.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3beedwuol.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3twlxvwbt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zdiynnxh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eimnfzzp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3poqrwzjz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xyfxltyu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lykwuywe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lfixxaaw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ehkvkshj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3itusqvgu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jqpacpkw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bsbrmydw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bdihomaz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wauwxvhr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nimmkqyu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mdisncog.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mrlacmbr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjxzktri.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bhxdakuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3uqwwfdwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xozoatfl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wanjwbcj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzoeikut.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fopomysv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3unjmckcp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3myeqkvpm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3usfcubfi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ndaptjos.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3abnhoyyt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nzbhewyh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qsswexjy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3teenrpvk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qndgyzxq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zrexmuiy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqnwqtqn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tklrvfvy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3krtyaokm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3njdhgunv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nyzmzwgk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wbqfhdap.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3sfnzmtld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnoaktfr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wutuwebl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nktqqzmf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ckfhgflx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3aqumvcmy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qzoblltp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3exeekoii.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3azbplayq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zqqwrmfq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uojdqlxh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tblewbkk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zjcwayrl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vsmsamob.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nnjqjyji.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbvttiby.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3aqibrjnx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lrjbqpyv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wpkjitzz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wricaece.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ojehpkwz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tyoytppi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3htyfffyj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3oqidcsmh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3saucyqcu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdlrvtmu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ajmgmuaq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3sghkptsa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nikskomj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjirbji.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xvjvhvhd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ektietjo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jstwytum.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kmeaecaj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3itufnaxh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fysfsecg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sqpcaiwk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aqweijdp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zhrtbeia.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sisqwchl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ndwvqxqb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ashmvbpl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bfbtetfr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cvbdtzwt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eoyibnew.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ytsdwjho.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vrbptjtx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gfjzmiyy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ikphvrpf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pogdpuqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3bsynppjf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlvttbam.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kkkhjewj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odprecne.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3filwkiql.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ajtbmgkm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3alvqivhi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ztatkdzm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3awuctyoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lehlypyg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hvydamda.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3klkizbyu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3spalvodz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytgupzic.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cjvtubkm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ohcjrwsn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hxnskuyq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xdekspyt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vqqegfei.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hkeomntw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fooxpctq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqxspaiy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jzrdpbpk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3pnvmfvam.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ajooyhxx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mrweiilw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yazpybtb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3xqaoubyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqwrwdkf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bypwpuez.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uhmebaut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rnqpzldh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jgxigail.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bkxxdgrb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fnfoukia.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rbsswzmo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mtdxcoae.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3aacsddxv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bqvuchzv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jqhdmlbr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3sytejpfn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3aworaeqw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mhutsrcd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bgwgikwv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3erfoxpms.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eajfgmez.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3diowywyn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qpagvmei.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3viekkxuc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3zcsfnudi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mgebawzy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3guwrojbr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wdotsvwn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3etkqcdtw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jnjebjws.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3snzbyxpm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wdsxuvyb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nfvlrzoo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kbkgddbb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3szxppiwb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fvdufyow.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gknqmmwf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zoflovvk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fnsuxozn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3fwijaqan.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rlhyldgc.html


<!-- 参考信息 -->