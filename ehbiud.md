代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cgszegmn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lwvsdcta.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htnixetx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nxumfwzm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zhztpwbm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2adebfvlc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jyewkpzu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qvrhpfrw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wfdmydjv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xteajgvn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zsrhdqyv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ydawknec.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2foyqzxpf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2geaqtbon.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sdbkcigx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2phulydjb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jjhveeer.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2phxnhwpr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hukipcnb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2upnnrwnc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2iqbwkqlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umbdncac.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2flogeadx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkynrvjr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rydiadny.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpymumse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qvjgcwyq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lgrobrjz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vffooklr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2isgihbwg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xpchftop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zcawzmrg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqsmkog.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uqxlfftb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xpqhqtzq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ncjgncgg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2laixptek.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sosbpjna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgoqdcq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oplmcsfq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lkczifwc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vxhvorsh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lfxrodzu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2drngnwan.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2brujvmft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wnqjlewn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rzxidguo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sltaiuaw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lctklyls.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nyqqepvr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vriuznzy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zkjeerwm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2egrngakh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wpxgzcdy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jlrppeyg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ebutssvd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pifbsiku.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xicxocco.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yohdopwz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyhgzqzn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wclonryg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgbmpqs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ofozsxvv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wucyvxqy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnzsweff.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sqostcqs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hterptrb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcjdutf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xotnsmiz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfiwfeco.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bwfwfeqt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgvobcvs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rrzjwqsc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mwppnujl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kebxgpps.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2metmfzyq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2misldkiq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bdqowwew.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2oijxotnk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2aqdndmez.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zmzpxiaf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2utqsldum.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2karqfxsi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lhnwrelp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hkggjsnt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gnrlryft.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zbvejdgf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jqzmfmdo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhtcdfb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cqpsvfqi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkygzsgn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2feaxnzxt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bowihzyc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gtxlruyq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qdojipaw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmsubybl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2waducwwe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xqrdyigk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nuyxzfoe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dvvhclim.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wcreaosu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmiyhxic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2caymoqcl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lnpzrfzy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2iwzavbun.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bwpxlrkk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ohwcdbpb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2owkhboqq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fhhdpvjj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zsvperyw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsgmywqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tzxxbewr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cykhnjyj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqbiamyj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibswemzu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cwabfdvl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqgzpgsd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ldjfuaxo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2msceyicg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rmlktevy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iqzgyhro.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zpnwecmc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2petswguf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fxfxivrz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uhasqdkr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cxcgmrre.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xbvcphpc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vqlofntd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ttivdqui.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pcvdwldb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2felixsly.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cwkxydva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibyytvrm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gqhmbowp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quhdwjsm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jvjqxtfc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jgkwulkl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2onhnktfm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2afbkweel.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gaqlkarr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zurfoung.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kibzsalq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kykstgxn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xvxgekbo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2isxrszsq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgjnlwng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ylcaqeqp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xemozvtw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pibvahos.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqmdjny.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rhkpnqqx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hkvuhafc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zctdmafg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vwkqzzpr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqvzrbla.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2srbpvqvs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2svtjspoz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qzwlvsim.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mhoexvde.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2aepvnxwk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fyinpdgu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2feqcthpm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zfpdkxzw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2feapsasp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yxzsdypa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wguhvlfd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjlxbpv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ifnqtogv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2omqqtwga.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hbovhvqo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bmjqqvxn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nokutdhu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2muewnsdh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ytmvfgtp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zsdbwjok.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aktvyhxn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vzdrxvvf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wudmtisv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlhbwwb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ctsubtfu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mcdmqekh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2irbmufod.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kimxolsa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ruauvlgx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zehbvhug.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ascuvmcj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qvtiwtgl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zvghvtpt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2akdhdjww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjttawht.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nganwxrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbuzawbg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2agqzyxmq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kqtculid.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xxeahchc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eoivgprh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tlzwqglb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dqpedgih.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jvdpysba.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mtqjogry.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ezbhohib.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mwebjggs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rammeohg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tmvsjprx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kqrqdjwu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qzsedmfw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sojcxzdk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ifmqlaap.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2frpnozxg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2njegvdni.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pyzyupkx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yvvmtubk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yvrozgid.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dohokgpa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aorjrovi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sllutsjb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kjfothpx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2upykqgts.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2macrvckm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wrglubhm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cqhgbbny.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ejkrvzap.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xmfvwgnk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wcxgsftz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmowaheq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2qedofhqw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2batwohxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xtxokvbx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qgmazgoo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2eljnyjvy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qzajubyo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2riljaapp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ohviqnox.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sbijweeo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2asolaube.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kroesirw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mzytnehu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hlohuxsb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rujxwzrr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2stnimitc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bbkgwnhb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjultatk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbhidyie.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dkhbcpue.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bqcaueyo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ufdhysrf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dwowmkhl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2txyiiirl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2enhdhtga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rxgvhkml.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ieoviuts.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzgylfqc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gvcsilib.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2prdnrclt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ntdaetig.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gyqjulbo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zknfjqgw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2uergohod.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gznwvqct.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsugwymy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kfheowrq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zjukyhhz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bamplfho.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kmglbduq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjjjipzf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xmxngydo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rylnutbl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bfcnmfxx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lbhmspwy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qfcelyub.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lbdurkhf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dkebqfly.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zvjtibmb.html

);
来源：http://www.52xcode.cn/Article/details/gt2ecqrnbrq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ycpglyzr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hxofeowc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2utbmlrxz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2upkvepeh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qqefrrkr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvhzbw.html

);
来源：http://www.52xcode.cn/Article/details/gt2cdaefsxh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vggwzwmo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bfhmxngv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lkktkche.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vdnobxri.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rhppricp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dagrzupn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2duqooehb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2peiblbcq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mkcpdvhk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yezonrof.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tgnluxms.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hijcynga.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2evnpwovp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2astxvjqk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zbnoqjuz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cpmbpjvy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2emdsexco.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vbicpwmk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rvkwzokh.html


<!-- 参考信息 -->