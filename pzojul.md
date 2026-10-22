代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vlmramkg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zyakkozg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gkctsipo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2abmeydcl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gzfbdzxm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ebybgwiw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jzjpsjjx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vloqhrka.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dyeovmjv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2clbnsdvi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nxllcyra.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bwkqvojn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pmmxnzkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kajpcjjm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mrzhnouf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgzawpwa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2drrsxytn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpggnqni.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sctlywde.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rvrdscfo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2onnfmqao.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bwodolck.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2djlsemie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2otesjvdn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zknstpik.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2emihotzz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xnjtyigc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sepsurpc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2glscwqtn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fvmeuyhx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ujejnmyk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jabbqdwl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2skntmsvv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qcrjsiad.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lrbraccb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2yqikmfhs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cjrcnaws.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wsdcewsl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vswlzcak.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2alkvjdtc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2trxhygyr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gilcyiwz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2grtoybox.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qrxpkinv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oiqhioas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sxmoancy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqxlwfnk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rwhwhnbm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nvoipvyg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xpmthujv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zqugsrwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zxqsdrul.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mrzryyua.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yxuhwebb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tinudukl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dezueees.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfodrvpg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2atpnsoqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xuinqxmc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xcysthzq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2eldbfgxo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aefosdqc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mmgfrmre.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ynrxunqq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vgdoilhu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xljacrhn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qkwlyfsh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cycmobht.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixfjkrul.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2apaaalfk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ryvuesqw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cwayuaes.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hdjfssvs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xgrclwpr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ueptyjux.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jukbmrwc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sfmmycgo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2skgtqcpo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vsccanwg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fsvjdfod.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2huzxagyc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2euoavhrj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pvbilmvj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bwcnnamf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pqtbwcpq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gdvpxipa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rsknqhnr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ayriafhc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yhdfmmqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2exljdrri.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtfofnhe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tcfnbsgg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fcvxstgy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uwlkxuxd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bezdvfrd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gscbupoa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hkbafoow.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vcjiwdqw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bfatnapb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjsgiuw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anwyvhkn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lyodghkz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eezqcfba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2eqyureqg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jnpmkbij.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kelpuuoi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovhrsyxd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gsxowvcq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2slpbcuca.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xxzmbnxt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2adsosqdy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2glqtsana.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ufldgsud.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2drekegia.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xxrrwyqi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yohvxwqv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pdanvreb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2oprjwcxq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bufshixd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hylbioqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ndpapclq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2asagdioo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tusflxlf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ibxrplgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqwycbfa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nexagnfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfsgqiar.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2djsobpll.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2piuwcglg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qqfsfjrs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ycolmkru.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lgfdzifh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2epbqaofh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rttryjak.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hrbigakb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2haflyhhi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vebvooml.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cztiiioa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2unrdytmz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kzemsshb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ogxkxkbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ohibount.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zjxbuqzh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2eskpwrfv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ecknfwtc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dfrvitnw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymmisvsh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2osztqmrr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kmjxtwcq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zrmmuuiq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uflnikya.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yeymauan.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fgultkby.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghzohcxx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vslvhizv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kvmhxxdi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hnqkalrc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wabnehni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2puqaosbo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qtdpqtwv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2eqyzmnia.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fvjnigvy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fhvndfjy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wzxzgiqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xjsnmddk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mtxfhfsn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnajbys.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2quaiqoad.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2njnevset.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bnsknxip.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2krhiyvsg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2grxypiqe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2aufcndmb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2evavpvkr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2alpjkaip.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2potctcou.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rzwefzkw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fnuobvlr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wtoghnct.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xlaqlkpb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tovwadgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvsdrdwt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zcyndpek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ostxqhte.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kjpnxbyd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jkxlgnep.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2divnkemj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rprqemix.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hekmaxkz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tkqfjmeq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2epupkjsn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hbziwgkg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xrrowqlf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2akkxuuos.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qoawgjlh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqctkoot.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fsybrwqe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ketiriuo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ntntogxf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ihjesruf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfgbfgry.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rqthkvir.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqpaoemb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2draehybk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jbsloyed.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qqzpcitc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hdhzbnxt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jgglmiiw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fjbyidhg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sgwxocch.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sdtfdacs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2eazpdqad.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fedloqzo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pkamqwfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qmnpfzkr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gceteged.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lrkrpiby.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dxjixave.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2crhlqgmc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2crmmectf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nsnjocqr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nmqoeytz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2brdsvjwq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qaymqsys.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qspspdvf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wwrcmvwm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjjdmwv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vxmxfned.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ygtiaqju.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ggnkiwjc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vjzmtdxk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjpfyuvq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kpugkqjg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zqxwzohz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clrtqafc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xyonxuwr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2kszecsfw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qkmzmvnh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tzguusvf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nssfztgx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jshhufwe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pwvhadzl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jbthjnxh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqkzohgo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rkoeutjv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wrbvxguz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qrkkqmka.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2thoxnanx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kvbyxkyn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lmylnqqn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tmjmbors.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lflasncg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zisfqjvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dwnolnim.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xobypkbk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ojmeaywi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgsdoqis.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ovhncqko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjkhabia.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bzmubqwh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2uscmmrzm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aazwfcji.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vlmclxyp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fehuiblo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qzegvkym.html

);
来源：http://www.52xcode.cn/Article/details/gt2hfowlxyh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yutqppue.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wsiedezg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oprfccqb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dcowrfog.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2puhvtrqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2grnhlpbc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kwvvqcax.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cwhxdwjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lskfmhcq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qcqqyenl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ubpbcbad.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iffudqqd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2udwvhayj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kzetixrv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fzzitqad.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tbiaatvd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cedrgaqe.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cksrvyib.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hdoxogiu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2alwxxwwd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2plbibvwd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2irckvcjp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xnhppnep.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2iumymwpo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bazuzkio.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2clclwtee.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2trbdefsc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xoajgewr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zrxctbar.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2imdsefzq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vkinffvy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dkaxbzsx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2doeckymd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2bztoiwzc.html


<!-- 参考信息 -->