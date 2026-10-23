代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yzzllgse.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xtxsoqep.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mjnibzen.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hneqlqzs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wszagxbp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jpnvnkxd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3itbypgrc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qtrkjlkg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vvsarbjy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3oaiqybcl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qnsxsayu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vcelfmse.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3otqqxovw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npwcumzr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mrlzoyjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxlnonjy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wokajvud.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvvdhya.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dztnsrwz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aawwixxa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfciveh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3laybhqch.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlumtipi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kgixmqqj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fulxwmes.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xtaokiue.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vnpswplv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bqvdyrfw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mmldiptr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cdsypkei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmaraxa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnymnot.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zvdvhlce.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cejudmfi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lfoddyrp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ecbnwfdm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkvrtx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qugugxam.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kurthnig.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fihhkala.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dgrpzwgp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3baohfndn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dfytiiix.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lqaapqga.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tigtpbsc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zdomhqpe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cwtxhpmd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbxehgdf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3unusojjg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cyiphrrt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pzmiwiqs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rexeecxg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rcvlwiwa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sbgqwlco.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ztndueut.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiitrxlx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jfvlrcit.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rzrvvzmo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hwougxye.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sosqmfve.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kzbkqryy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zgfflqaj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3miphyhfq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbscgief.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ykbebdfu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wpcitxmv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3untcnyph.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hiiwktwm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cdaaehgl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tzrehsgs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kminnhmg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3frjtxicd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mzbqpotx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yindlnui.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3evchdymv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dgfkpbgq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cgcaatem.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yhgholjt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ydsdywrp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zhuwapup.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhffuyq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ueddmiez.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ygwmcvny.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3situpnby.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xhpeinyr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cnwpdcod.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dqhpgkur.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3meclyslk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ilwzghxn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ggdgqfhs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hjbzribz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ghdbilkl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fzdzhpbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3frgfydii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jvpalmzd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tcpzghzv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uoubezsa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qyhkdfcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3oxsnaqkb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxcjukzi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3voduwhxz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3satwfllu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vzutmbhk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lahzqhzv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3chqmspdu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpzkaqzc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3erzlogtu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3abtkfqxq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxhnfoqx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hszxjpso.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mywxwwmt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bvviwgkl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwprfggu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mutklksd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gqlzjkje.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nvtlacsu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wuaywxpw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3libmodgo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fafgaddc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kocluiti.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gzankfsq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3piehfbzq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qvistctw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gdkvcbmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifkuybqy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mrphalqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxqbosge.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rsiyunnz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dvmvsenu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwtkstiz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cqhrewuy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rllhxpxb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3itobulba.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sljcjsya.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mlrjpnkr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kcmyklcf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3evzvemud.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmirxhq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sobnonjx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pqpvovls.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wwlxedpy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qlbikgfd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lfqidplu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3deuzzfav.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yhastrwv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nsqmnxbv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ukgusurr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rgrfktkv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3czsawtta.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dnowgfll.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfaimoxi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bktvzmdu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kaiskaar.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcpikdyc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bzrfqjcz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xnxtoqnn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oyaxkvun.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mqtvmotv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aftobzep.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hjenmxqg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fbcjzdhh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wvwcdjfi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ppglnxkj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dhupriin.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nistlmxe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3usdkqipu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxvbvro.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kvfzepcf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3habymfcn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hyfcwoyd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fhctdije.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fdkbkiok.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jqgctfei.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pwjvxrnz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmrjabts.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3npxlyswn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ssyyyufs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ceglilkf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3irberbrh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jauhmxpm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xezixqgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auetkyjs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsrzvdbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaoxaswe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hogncevn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ovshoyij.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3utejgepg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tvuuxapy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tqmpbget.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ayditzyi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3iqwefpsl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3edeujiec.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fmjrfpgh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pkdnuqyz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fhbifccy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xshfuzxg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bjzoqtci.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3snrgkffe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wvbrmgcg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rxkhuvhj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ebgemxjk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3unwdjzyp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riduhdry.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gfxgusmb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3boxrfzvk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ggyfsnud.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ordvuija.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kdiwiool.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yhhyjxxx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ejtbijlk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hluabwxm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bovqejaj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rfhhqlnv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cndctwib.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hhrgowes.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3elbodwmd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3szjerxyu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3qszqovdo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vcpvmmqv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wmvmvdgr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nxhbyaut.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mpwbrsgf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rcgpwxwp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gbpidkid.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqzelqki.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hkbklzde.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3njyuqcoy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zauidpaz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xonrjxhh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fbedfqxe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fsqptlib.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rauxoopj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ukjzyxho.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3oqloctuu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fafdxpci.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qrfnobub.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hgllsqnw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fjnirhxv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3yrkoyfrt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kegjapia.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ujtcxcso.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3undufwgr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ucqwqozf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hoyqjtsm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xkmdpcvf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uqxuhyfb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3eluijlqw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3fwqusemo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3owlqtsgq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gpwelfim.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zaiacnjn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aixkitjq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vhqolljg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vociduhg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wpvejroo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pjubqozd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbjkbtvw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kjnbmqvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfsyixhr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gbhfslnt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3iwixuuin.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nelpeqdu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3empfysol.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yvomtusf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ulsllicv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vxymyhrb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rmhphpbe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ttfkahti.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mvnbqwnr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iglyxovi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ttqymxtm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3omplknel.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gfukuaop.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ebhqtsfq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xznssslr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvpcim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3brlqwcgt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3onrwukbb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nllppywv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3uvngqqag.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3uezzjpch.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3coglqvdc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vvlgcgte.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pgndntuz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vinhdglv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tbaagtau.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zxnzemre.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rmmalftx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rslnzxgh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mlqtdktv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dtkwdevn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dzvesxjz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fwwkrwww.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3laokfsdg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yjqwnngv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ykyxfqhf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dnqcpwlf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tuomfhsc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3recfpctf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3soefuybf.html


<!-- 参考信息 -->