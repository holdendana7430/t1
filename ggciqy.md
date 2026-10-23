代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3onqmfxuj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ufoxudzd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwofivra.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mtjakvdm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hmlhorwd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ginuumew.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xngbsvoe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sojmbron.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nrxejaqj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3okhfzuug.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ucdkyryr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cgrhseui.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wlnaricq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gwlmrmdi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dxpzbpqp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xujtnade.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wswakctp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ehfuletv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3aosxjvip.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lmutpxvq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dwdukrqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihnopqhw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3farkoiwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oijoswnf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wxmtwhmd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yjumyxzi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sfvyshml.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jmujpjvw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uedzbcyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3siwmhhoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qwqejaea.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uggzgdrt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ydvdpkpt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yadmxulb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ktkvszre.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3imsqvsul.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3emboxsph.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uffbvroz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrrjtld.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbylicbx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mhnqzqjg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3umcsahxh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3uhvjcmww.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xprqdwky.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wmtrwkwo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dkixvezo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xrspoqjt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mycaojgl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrbiig.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fddvxoun.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3onjuwpmy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3odlvhtpi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3whktuzrw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ilktrnhk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ynbmfnwf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fsaqjegi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhhndgjj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qnoxvjtl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evonsdoa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lomtkiva.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ipolovdl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mtqgkdyu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuftuoot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3awhctavu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ohjybtop.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wcpjszmg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3llmtnjxn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xngngxyw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgihsnxl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngezgzku.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qydbsrgh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kiyzgvxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jvdhroas.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rvbxvizk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qrnesmkp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xfmtvsmw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tlsbajzm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jnwneycf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gxkmkvnn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bxicmznu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fopnjoyx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3icbxpgwp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3filmlctf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zmnhayrg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rwjkftln.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3lubjgxpm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tvtjlrpv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ppontigm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3odpwnwqa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3puisjsxe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3augottyq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcfmhvze.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijnmgmqu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tljdanqy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uycktexu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3npowmvpg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3utzpmgiq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rsebusxi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tiobpxnl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wrxsdpvl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qafpcohs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sgamzjkp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pcasquhu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tjonjffx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jfcvwanl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rrevgexa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jbuctbgp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lfdmblal.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vqbjowfs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xfjdcoma.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3epxuodvw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gcthkcmh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3aijdocge.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzihyhps.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wlvoxblk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gsuuabos.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qgfrieyr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hrfgpzaf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wsmekfjj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mykyjpzd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gachasgm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3drmkrkzg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zzuhremq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mcmlexmy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3toeadnuu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hizzsola.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kptfakcz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dzytupbm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xxxjyqdm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xziswwuf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ybmpcksp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ddlzchsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utkqoehw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xiswiauv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzsgilxf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rsokxgxd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mtllqyov.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fxkuasvu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3awbexpzh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tvnewbos.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3uieqchjb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uueejrnc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jwivojvs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hmddfuwr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iqgrkzjv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dmilwirn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ggqfzsbh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gcjmyzbj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pgkmxgeu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvbysg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ajhmpcmh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bbbivjqs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ovcbldeu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3byweaitf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3igezwljc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eeotnpgd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pxnsfdle.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ygrqeuew.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3meuglkba.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hfxehrzw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3omsvdbyt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqkhpzvo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3idtbkttx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3eujtejvc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ywgtnlgp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3txyvilvv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qepxuldf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3zxswjmtv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vxbfspox.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lnwusxxz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lygbagcx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3csqxumzk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwllmoa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wlxgwruw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rhaaaaxr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3brwevejd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lspzmqxq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tnvkppxg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nbezboid.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3suclcgcg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vzqxysvf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bsjejmto.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3abxbftup.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pcikgfbf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3asxgapvh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xsjpzhwh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mzgpieen.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3buzvqivu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ecjierht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gonwylkn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pnagzsxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tddexzxc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mkravpba.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gobyjttu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ootbblmc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mhgifipv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hrvcbvpr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fumdqhek.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3abhmfljr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rltnqdmg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cuxihkkf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yjfpbmxw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3swyazmee.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tqfhtyjs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uhhjnlbh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3oagbspjx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmnnepx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wwhjwtks.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cerctdif.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nvnhpyea.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sqkvmige.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3catdsgsy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3oqxrdpwm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dlgvdbie.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3msuvdqkt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtfrcjw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kmibxoig.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3strqdifi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ioqzjwuf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gpawimbr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tvmfdqtb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xcwuyzqm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pasfctom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ahdwfppn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ewhzrtnn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vujyuzxg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ropedfod.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bpiwehqc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vuehihqk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rxwgsdmx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ddfdctqs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kfifuwej.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfkavgp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xkolnyrs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ibqlksgd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3masahpzb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3letshikg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ppbeytti.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kwyxrqhs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pslwttsf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3coqzbmsw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hiyjwmft.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hibrsgir.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jvofwfda.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdvdbcf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pcezzwfh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dcwhjejj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3auhukzas.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zojxvcrb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3apxwhzgy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fqgafoez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjkkxtnj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jnlhsenb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rpawefdo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3figatmle.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iaffipom.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdypzgh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uwthjchm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3oamvexax.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eonrjwbb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ebtjcdmo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dfsivrlc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tutscyfo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zqzqplkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyopueby.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3quhabzpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idlnupnz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vuaxajcj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hljfiwyl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hegvlwst.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3imtqozwk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nynyaksg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3orwecgsa.html

);
来源：http://www.52xcode.cn/Article/details/gt3pzksebvq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qdtlcghb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bvhrlqtp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dgjvrrsi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3slgmwexa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jvwiiuwz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kciyaugn.html

);
来源：http://www.52xcode.cn/Article/details/gt3qbvmclzb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hxeyagsg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tgmlwxon.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vstyvdul.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bfviytnh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ljckakel.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yxobsazy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lgeuzkzf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wibeykip.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3edkjrokn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cfpubuor.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3fadrdzdc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mnvvvnin.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ypiybczg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vrsapaef.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3udbyvgrr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kaypddrm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xyfswrww.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3brdtdkjz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lqsvqlgj.html


<!-- 参考信息 -->