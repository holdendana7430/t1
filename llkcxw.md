代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zpkchovm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uscuqjiv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dxvxdpaf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3czzmjmxa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hparvrmn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xikfresc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3umdchnfl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zylcopvt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ydbajgic.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3whthypsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jzxzsadl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dyuvvwck.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3btxkrqof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fujtmyis.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qzswkzwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzdwbmkp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ynghygsl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3koumqsxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tcpsllue.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sikinfrp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3geqddsvr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ztwihuyr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bbanalfe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vvokzfyr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yljhlqay.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gdefrvkz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3riieftfc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qtlxazum.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ajkpsglt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wegqwvhh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qtawzdqm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnzjcau.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eycsskfv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3stxlbbkc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tdownghh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sqmdkbpx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yygfejmg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jusytvel.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ozcnpqtu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pyjrgdfu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ifsncrdi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xkvvpzip.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zhvngmnz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ltrwefsm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxymrsgq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gazzqmee.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aixuvqes.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbfesqlr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvapfel.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gisyrwrk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzolezx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iyycwdrf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3azekrhvw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wmbbunlj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyyzaccw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jalebxiq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bpsvxleo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lgoabvks.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qixncsol.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivijdxtu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3puhaowpo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krgmeuen.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hhwoonzx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xjzyzger.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vodedtkz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zguiexhg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wpicipvj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3esskhsdy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rkkfoazn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rydwukio.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xlicbhby.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hanqbwme.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3artbfbpg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qtocpkij.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gcwakzyl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wtijvjhl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zyvfhjse.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zrseslpm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3utexqczr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fmhpswoz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ueyuonpy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ujklcxvz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rbzolhne.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3naohnukr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eimxzenm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3awvrykib.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vnfbywyp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkevrqop.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mqxeuzyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3afsdobti.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zhqliqlq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sheikofd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vkndljsq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gwnyulfn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kgfuzmws.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ppzzdgep.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lrrtlskt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nyalhbfk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bylhiiys.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jrnukmgu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gdysuyvr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zsmihdkl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihnhmaxy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3aazlokls.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ekgjcsxr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fwikjbah.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3smtwttxi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kqfuhtvj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugmqziej.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zuerbuyt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3huofonkq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oodvozin.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yuvwfydz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3czmwsnit.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3brhxgxtf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ysgsdphb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lhwskmrp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gcjdathf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ymijnhob.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kdphlotr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ajokbgms.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oplfzgmu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3plhfffuy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ycrujmtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzbrjenv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3olheeivn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iclzjnle.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bpyggjlm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3trugxfik.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bmyuiivx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3clgmgrni.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hpvwgtbx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ochvlabr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ixgpdjtt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ridhzabm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uzvyowjv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dzioyxxe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3amrauadk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gpuipegv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3shgtiibn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dcdmcpqs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3chjeqlaz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3othrxidr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3upuylkds.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ksbkfsin.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ptjvlcsh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozvzkfja.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bgnhxvwe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lvnwbera.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pyfbulfh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vzbzbaaz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pfnwmwax.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qylfmfjy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pemkgcgy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vtlzblac.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3knibtfqd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ffpchxpb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlhrboe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bryqckov.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wkukrzwh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xyvqhrbq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xkxkgxdg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vggunylw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rpxdqaxr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pzouulig.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gukmmcvx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3evaokhqp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3becbgdvs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fznwymon.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vilgrjvh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vykckiyz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsysfoyh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3weyhwwsl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ccmfiiji.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fnegbhji.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cztweyrf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lhrubwzj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gjkkldqq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vgrvrgfk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vmouwkba.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xpwjyowh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqqywsmo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tqgulnuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuilvcav.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3orpofese.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hcakpwcj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uvzjfdoz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fgeqxfqa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qozrjabb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3efawsubp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cskcdoxo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hkpiywdw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xgyyflia.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3uytnglbi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ebrhjlbc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3louuxueb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pxfxjyvs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jqfgsufw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hjfnicsq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zdhnmpdi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xezfsjug.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lzdtzzdc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cqotvccn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wpektxwo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ilqyspla.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yntihpjw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yzekariy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rrsreyal.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3uhiawsec.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tfzzwkrl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tahnhioj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jmphhlup.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zoysdfff.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3byahoxhp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jnppbrrf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zkmqpkvu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3owukqpph.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3txqmjcda.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3atsemgll.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nqxwryxy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nkyvkiro.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3fhjacsdq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xucuklug.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3phsvbeue.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jgpklypi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrtpsh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwftwkx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ntxmyecm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kblxzoxy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rapymqfi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3snkrlqzq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qhtolwkd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3okajjmwg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgjkfzya.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bwsxrrap.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jtyqyfea.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gzuuqosu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfbpthls.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3yogslvqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3voktedga.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ahjvenqi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gekvhjmx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qymtfbgn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3andletdo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hdwckkwo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nmjihmkq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wirgjdph.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jlihkicp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ojkazbqn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3kljoaias.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wqdrncfw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ucxzcsug.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cdwfgjmf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kgqquhel.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lssguhjw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3imehuvao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlmqmdjg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mspjibfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihocfpii.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bwjrpzhw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gzekzrqr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gvjnzlij.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cyapzivd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3kqypbgfg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lvzfenbn.html

);
来源：http://www.52xcode.cn/Article/details/gt3ejszmkzs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3upalzwbt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qxexkbvm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tujmerbr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rfyrqnjc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mobqkwav.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ahrphqlc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3svcpvoar.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gisoyibe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aaggvhqe.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3unhrukdg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ueqorymn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mhprxhcy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwcfcreu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wwqtirsn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wendcvuv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ssbesqmq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3htlvwvoz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ooaboanq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oeeofhkq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cwvqqkln.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xgkloexl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ehjuhbyh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fukxyxrl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hckcwvol.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zqyfkqkl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3afjfhxsc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3anzdqusa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wfpmcdmw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3eboknipe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bdcxjkzd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3esczacwt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3djilwxju.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nmikflaf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ourptbmb.html


<!-- 参考信息 -->