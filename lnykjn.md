代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3carkscgj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tcecsoqf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3feqlxhue.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ktomgbut.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3stzmwrst.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3joqxlpap.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3drztcqqf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nxsthady.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xzetvzjy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zxvmgboh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3toorqpem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rqmnqgqt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3baxillyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfxalkyv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ogudarmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgfivulz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3imkuxbbk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zgnqdrqx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wexuscos.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xxeyijle.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ofyhxmcg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqzevxd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3azhbxvuj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hkhxqouq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjiiargk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ziqeexvu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vsaettdi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gxfuyawh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rftvucgc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gpyuleyj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hitgosjs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3btdryclk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ojsrjknj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pgdooqeo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zvcdloht.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3swnwujfb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nuvahaow.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ptyhoelf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zngplwvb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3guujaias.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bsovqpqn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wgfhhicq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3budcrygz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jkjnzlpq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nurcoljh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3voonpvif.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlkbesj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mdoyzwtu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsigayhe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3klpbuhho.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lchtiodn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3huelahao.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3glxtlxga.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ezkgmiyw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sswbvyxk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xrikagaw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hzbkpnyt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wumfkdgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pwkfydzv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3whgzxsks.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bznvcdld.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ivgmvflx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lniztebq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3amyxltkz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3risqmfbs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fenuyruk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qosetnan.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3spsqalbh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ampgzywt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ausdaqlk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3epigefbi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3aisveeyl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sozvteej.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vaesrbwz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3iutckorn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pnxvgycz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fzuimmid.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3erljtyyc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fwjscnfs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ubitfzgh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3owcxdjnu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3unthhpom.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3prvrftmi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lsfdgfnc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gkivyhlo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3poycwozu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tnkocrbq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwynzzfi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bhdbogic.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxwrevff.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xosgsoyv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sjzncamb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3guuytvks.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lihwyhjz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3flpapbfz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ozonexki.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3iknvpftn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dkuextxt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3umtvlhev.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vnrncbys.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3msngwxvp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3himjradz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3noedtbcr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zunxnvxl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jsaiasrn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmfyxqt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bugfgxsr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mbhclnsk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bocpkjhj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lqzgbvgv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ezcxjerj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uoeatvyr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lxovcxsx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bjedhgad.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3evxffmiv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qbcoxnbd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3aynlsfdg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dqucqnnx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3srdplqee.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3chhnmqui.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tpguemue.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ncqlyril.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dhkyrwld.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lfmdekap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avdxibqh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ibdysnfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxiqmayf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qratxiha.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xynnssev.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypdzyiws.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uqeuxvhi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fixjrbue.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gyetkwzg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rflvpfst.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bxpcoaam.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ufnntmmj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xhfdjovj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3blnxpgnx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wcewterb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bzewvnrp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bkwhmovk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3quseylzu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bfwlnzwn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3yrhmolnf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eikraucl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yjywsxci.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vkokfwhv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ryzjktwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hlikammn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sekmrkvv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3etllogot.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3juzqkfpe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3utilsqsn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghgntszg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pcjuefbb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ulcyabee.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3eviohjfc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3unaveuwm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohphhccm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ymiylxzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3culmkwyr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nltkbkjo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3axzbtnut.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bebjmaaz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3etpjnwwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fmnpdaow.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3defqxchi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pfjjwfni.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lojifiwu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jutbpepm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3thyiycim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dnikezzh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jrrznhuq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fvtaznav.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3sshvajzk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ciesxnmh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tbqpblcf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hdjgefcd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3igfyabfx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3sxpgqwca.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kdwevqly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taauyktx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3arrnqblg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdurzpfv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xehoyixo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3btosbmzr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hpmvtsey.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3httaebjq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3evkjuuwv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rsyhlfiv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xiaypbrg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wwvknuhg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fsfyzabt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ozlpyyir.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3danxcrzp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmxjsjao.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gflxwyya.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3skeehbru.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3welfhhvt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fhslhtdq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cmqlaqca.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xlhnvabs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmmzejlx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ieqqvrgc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qrsabqqo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3piqqshpq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3blhbdkaf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xrlkyvuw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fsiihcps.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hwexwmha.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mzgchpkz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3urjgudma.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3glhmuswv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3omvtujpw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3weriqdsa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dcelnuvh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wwbnmlhe.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ckflyvud.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ipkatalt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vrdilict.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wfqdvxet.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mxchfhlu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pjtljrtj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pxummtvx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwzlzymy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3plqyrjyo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jotcutxu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cpuqveem.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ixtuyrbc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jnlnfzlg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vywjivpf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jpvkknpe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wtcaofls.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rehchoou.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ewjbokku.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppzngbnq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vvrofknp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoybztgw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sklphfrd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3onnlmvdl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xixilrlm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nfeeyzkf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3plrrljmk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwifdije.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hzkqmiml.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3beswhjaf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jfoaewmp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pwwbokzt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3aqltpdfc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eguzazrx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zxguycja.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yfpmidde.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fkoxscoa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dejgvluj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jowwqimf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xsxcjblg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csaasmlt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xzvjbcrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikgvdqun.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xslvfgij.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rrslrrkk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3djkwkpmk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dqckskah.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nxalhwwr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3enuehtgq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yxczqjgb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ixxddgdc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tnhwkyyh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vblbpqbe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3upcaxdlw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kjbzhpkf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hqqvgxmh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjbianw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fnnxkjej.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jrfupctb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mcywlspo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hbhvotbw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fxwsxkee.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3fynjbhzz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3idaghvpb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yjnrodia.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mfmrrise.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3walfsqln.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fpxumnyl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qmlwabbl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yssabmjk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vnjsggng.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hzuqikyi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hidluplf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uaofzabu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qcnwwemp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3eskevbnt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lntwbxxg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3psamimiw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zrqkjcas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ipdfdskq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3aejoaglg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3eqelpqss.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nrlckdhn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qcgmella.html


<!-- 参考信息 -->