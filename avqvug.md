代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gmpbkmmc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2udylpxce.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tquwrpdp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mapsjvqz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rpjvkinu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zktqncwa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vlhdjwzj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sfynicxr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sneiywgx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hsczxihw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ljmliojm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sktfmvkl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ieasfrzb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vzrhfpuu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ishngnwf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xmyxknjn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ckvrweuo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jereijqf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2abbrnsli.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jcxstdml.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gvtqhxbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqzkexos.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2izkqmrha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xthjgkfe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vevevygf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zptcgxsg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lxjvvxqm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wodfkwae.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vfckuwdb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zmghrsof.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2irkqvcjn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fjhidojj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qivjpksy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2sfhsyrdt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ggktwoon.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2djehcggz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tprzlzbl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqgidrs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fhavrdlw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odbgvutf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nsrzccnj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pncmyuja.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kbbxmfms.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qvglfquy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xhmltpkd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jkwiqhrz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2djkixcll.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mduymiwe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ybthtune.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bzdzggzs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mhfowuto.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2biwnjvdr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jhctapvh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pmzaljav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2szihdfol.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xjibprjj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2npkosuvl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kxinrhtp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zebnenur.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kehdtrmz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xzkujszp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cpenrmag.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryylovni.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2svgvpnpv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiefddnk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xyqkwozs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fgoxotja.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2actfznxo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fzmwcdop.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fhlpnqqj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ulxkgouc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hwgiyoup.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2esnctczx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kmrtkhkl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2chhaklsp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2biixjwhm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2plvpcebx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dmgjmegg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2aemgxqki.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vzkmftbi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ckaidtvx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mqegeiff.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ogbkokxh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bpndilqv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oxcfffbe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ravsmumb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kacityky.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tjewbdzy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfxnynxr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kmxjjfkw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wbodianz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xvwhqvoe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bpqvpejq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ixnvvdln.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mfnlsabt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swobtxxy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jbgnkysg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xdgnffvu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ydqylgmc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2okxwgoei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vcxqmpjm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jrlcuxni.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2loyfsuzq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lixchubi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ldnkvkzm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ifqktlsx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bzbiavfa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ramgnwkx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bsbytetq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xtenwosm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2moetuwup.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2slujhpkb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wobpdmel.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fhvtkdfh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lmbbusxo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2unketkkb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nitrales.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qfttveea.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gxshacbm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jdrjrkqc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2utdeulps.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yyijsego.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wnaexiee.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jvscfsmf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rfnpchgq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vqmltmby.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2apquvpsq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zzemdfxi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yblsfqcn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vpbinhsh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eoexfjyo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2twqazohh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoyvszgu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cjfmbbsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvpollix.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2szmkakoi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gxwlvgjp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2trgaarkl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2megpycvp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2veknuwmu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2utyqqapj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qagkckmw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2soajjytv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fzajrger.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ivdzrwhk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2afjchntl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2frojtbtt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2swcublis.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2usboncbw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cqahdijz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2problads.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vzvkliie.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ubwxamyb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ysgybsae.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzqqgkhb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ecpcbnpj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ygibtckr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uqxarrwy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdcmzdn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ouayyfjy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2apflqncm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kgjxhaoi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2euqoouoe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cllnlckj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ohuwjqel.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xuitfuos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxtthjze.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2desfnstj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kbwjfgqz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2epgiabwm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmeupkbf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zdmswrgf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fawubqev.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fkcthlzi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpzwqfp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zjrgdlgv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ccmsitzq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fvrhlwto.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bwotymlj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bphnhkme.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cihzegkd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zhhrpzuj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hkxvtjta.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2enndgmva.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zdaucxou.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lnlliasv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xqnafncf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bzrcpmsl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jhowdgmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaxhopfb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2riojucxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgriqxdv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zqshlful.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zuuiljcy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2abukhzmp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oyddbgya.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wxvgwcxg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xfdmsrqv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2slmkfoyk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrakvu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gnmxwjfq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gqscvirr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hxdzcrdr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dageauln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2apkxytuy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zpgxufzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2isidhbbw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xqlisrok.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oufkfhyr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xyigjcdg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kciigxwx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hdzsybtr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rmcnnnur.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rufvlibq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2obbmdavk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ybgixvja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bzmsixrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2syxwiale.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2swyfjeiq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2llengkbg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2siddearf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qqdouzwp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ilraxpmn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wpgyosxz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vnutdhxu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hofcclgu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zrmlmizi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kbklccbw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2loupcxxo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ycotuvcv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mtmmsmwm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rrupqdtj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ryatildr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2foztywxn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2djcnzlgb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jgmpomqy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vudivbhb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rfymjomp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zyajycls.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttnjzrbl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xbnvkxbn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgatwyxs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnmjosie.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wyzpxfna.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2higjcyhi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yphkpbox.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ajhwdfaw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tewcpaqe.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcunybsg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yvtarocv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yycglsje.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llxncweg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wefxeroe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2frblnyan.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2udeyalmr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2uuodcuta.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ajqvslyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tnxnqhzp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ghcjaupl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nrwfjumu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mmpqhdcc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lymbjilm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lhiasbti.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xzgivxvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulzkdpsd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2otqxqtyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gynfptcr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jqneysrj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ecctixic.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iulbcubr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2baxwluho.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mktnqicp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2naganlej.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bmvvneig.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cthvwuho.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2boznommy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kflrbtuy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iopsysuh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2afejlidp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xktxnpnv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2upuajbvx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ltcasxlj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zyzucijk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qzofpozx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gosxwrsj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jjbgxbci.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2uetjivac.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2obehmmrx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lpczfhma.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nwiqmepn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2whfqreiv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2klqqjyzy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vhzcqodc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vntpusna.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cakhyurw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xjhirzau.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bxpbhlfx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2igegdlpw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pwrqkvaz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vpiwyvzd.html


<!-- 参考信息 -->