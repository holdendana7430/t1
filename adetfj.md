代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxuvppy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hofwgizx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wklnmqma.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cbihjbnw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uflidagw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2awoaygnr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bvolmmuq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ucvtkaph.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2anjlmwxo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kcyoxpgo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cvaztqoa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pmmesnbz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2udposatl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzpdzxfc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ltjmnlhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huupwyzp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhrroe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wfaacthx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bipvnsdw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vkvhcepz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2doxsronj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bngqvrkk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vgdaziis.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vgfnszlw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swzpfzkc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zyisyhqx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oxkimhrx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kfzidwsw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdgjrur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2unubisqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kxvdqxgi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wymifpcl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jbgnwbos.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2crokncza.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2yxkiawcf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2majfdhln.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cqfhztki.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lnuabwdl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2icoljziu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mrwxjnij.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cngzenjt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bkfxpbbr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zyloqkze.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fgcxlauz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sofezgnh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kozlbfcv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qkgcasra.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzlkistq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngsrtpye.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cogjpxew.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahvuwdde.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jkzhludo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ryyitceb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wyatzkuc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xplqygut.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wlmtklya.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ysjnakdi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hpaozxkx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ofwswkne.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pvlwkvuz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uldgdcnm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cytggjhi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tvcgfzol.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxseaeyp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ksrgfifu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sovhfryw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jubmvljc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2glcnducd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2itlzesja.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aclirsag.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2idcmpkij.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fiazninm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qzeiydxt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kginnpri.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2thnvdsva.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bzmyeqir.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rqormiwg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dauevhjx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zjxylpry.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fyawhdjx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zsnoccjx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2janopngo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfiptivp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvvqyjnt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xjsfqjhc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jeuxaejp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nxywwzjr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rnrzabhy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cynbpugn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdpdflqv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tuggrnbr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dmuvylxh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ndbbjzkn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzcdxjto.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gvylhlto.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2frgnthfd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xofyysme.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2awanhwof.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jaoodbxe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2puoayggd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tihjopke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gegerric.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndoezaub.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rtwalopk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2alqqhdbi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xqazbamh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lhuliwuj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2twtzhnog.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2csrtmwrb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qszmicra.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpjvxi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hnomqbiu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2azeukpgw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bgpymqsk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fyuffhqx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iafvtfqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2alzotfxi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kexmmrjo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2awicwfol.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sgdhwbch.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dhespblc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gfpzhxou.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2udhhabtx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2auvhkicc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnhpqzvw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qmvnkhdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voxmcudp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uahuswyg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tbxeeeux.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2abgnwnlf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cuppphjm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xmczzijx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cwtxoyns.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2sjblhppc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hrdqtmva.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rlbsfdtr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2htjjkrtq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsqwgjx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2afiqmxas.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fywgmkwa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pzqurvlf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqcwfwi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mqifbfns.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2njflhnwh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2aykvzhbu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fzjwwbda.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2czxgnwna.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wdtfqccy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jykknhbx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zvggxbey.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jqdswwgs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wrwirhff.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dzkermpn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wxnewtuq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2udzhtxav.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rlqiccio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wxtisphx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kvbdlift.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wslsdpqj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qnicjazl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ypvxxuam.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2inozwxiu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bugdmzqs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ahyxipdz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aulkqibr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ppuytcmm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2svlfuihz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2slomdcao.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rwryyotc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zpxxlhoy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qtfsvaka.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cftjdsvm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2secobcaz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oofmajuw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kecdhquo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mkdzswpp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gwyrssln.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ijtmpudr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ftwvpapm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jfajcsch.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2prgbrsyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isfufdnp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kotzsbbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnexjmza.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zpharcwx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qmsbzlmn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ldbylrwz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ddpagiyw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hhwepdnl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nvgjpxpp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vcqtofyp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tonedwsm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvltmcez.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dnsqbwsv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mvobsprs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zepulimo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yxxnrehz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tqiimkis.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wjziahmm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jolzqbmx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpotohhb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ifipmbhl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqkzhevy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2stffrvbk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xxyxxbpv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2btwnjmrv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rbnqqxno.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ipmqvihz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zrmnciim.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdrsrm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pqdeynhl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zrjgilug.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jypfzube.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2chqbwtkn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tkspudwe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ojexvmpu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yvhronov.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2eendbpjr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wtuzdngc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2emoxfzsj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jpkdypve.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dtqulpkc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gyhrzxih.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2soktkhaf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2slcfskck.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xnyzrddl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mpwdidob.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2smezgije.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2taxybmbh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pnlkroel.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2nfflgglx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2megcgzra.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ixhifilc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2piwtjwuq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ealhqhyb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mrjyqpqg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hzxlblbh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqtjguki.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ysahvrbd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2yzzuyvzy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ymdvbfof.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uxhyuzgn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ttyglsxi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uqzwjrki.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tzycuzyt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2itfnxjje.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kwwgucmp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2usiidnen.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eankrytn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xxevdbwv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ptrdfwut.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmsjxuo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hahzhvmq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gasgafgt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nzpejdut.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2haptivei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eazhawpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zjaebhzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnfdpwaj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kghjgzua.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vceupwqi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2knpywwfx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wtlgdmxw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gmoxcnpk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dhylhdos.html

);
来源：http://www.52xcode.cn/Article/details/gt2uqffgurx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dwiffywt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2afeoninx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mumxrsce.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pkfrjbot.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bxikcdnd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gabmssus.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hjteiurr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zakmliqq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qlvdsptd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2avchsbmi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mnjkiwjt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qwckxuyr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xykbuicz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2srakwxhi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nrtizucy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2pjzayipu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nvzldxzr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fnsptvvp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gthxoxmv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dovobgak.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qvokzvzw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fwhtuyvx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bjlkuwiv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2eceptder.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ggcjduka.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ztirilrj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wuqtxfxa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hsjcowjs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mulkdnou.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gudywinu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nqdqggmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2doybvnnd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mklrnndx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2znbifvdj.html


<!-- 参考信息 -->