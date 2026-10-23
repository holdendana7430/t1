代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqlwbexw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nwehfruv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ndfcdrnj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lpjsxvhh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vhdvlwxv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3itimgkny.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qxhicjrs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gvyechdv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eyvwciqy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3uozjurkh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3llylkeab.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hckvlvhi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zywlchwe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cfhzzyzu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pnmaqxzs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qwvyybyq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxvsaep.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jukducek.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fxrnaafh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kagalhkl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ipsnrquw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vaicatjg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zytezhwo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3msfxdzma.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kpbrmcpo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3njkflvzk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pmpszeyp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3utejzdmb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yvcshawf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgjbynwq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jycrmclh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyxkkqoi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3euefiywm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umciophs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mnoehzdd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bonzlsmr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vnyvagja.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3haowwlsf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ehyetjty.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3aucsskbe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkrkobyi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3afjpadom.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rzphnkpc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cynwyubc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gshmflcn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufgdeuwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3brjbzwhs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eubdssla.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gzveznzo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nqfgqlzb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dsdnpfwh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3diiqbfwe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wzkejcgk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ssjgjlax.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vinfeemq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cimvuzpr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ppxwigrg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sqahriqm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ehklghvw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lalbypkh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfobofrx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsgahpfd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvveiefw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aioxscbb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqqzkmik.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ibtnvkng.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3irbivzrh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hzerpjbi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dhshroqj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3auxfoqul.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3iartsthg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmesyfnv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlizdzvn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dqkysuey.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3obutixqs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zdyjxkuo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3grjlqyzj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftbithui.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ezfvcfjn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjlwbgb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ichvjjgr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lsraefwr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mnyyrsuw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pbvtuyoa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xldwafnx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3udxcckwk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3obyqsqxt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ltbqrvri.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pdkjoymm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cbldpfwx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cyhcxnbj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ahwwslyv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cryvwjkl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xnstvshe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ngtuyexy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zznyphib.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ebohcdhf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ltytbvtw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdccxqvw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ryfcqpxv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kbcrlsfl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gdriwage.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fvagwnjf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yupsqgqx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3emaoqabm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fbbznbax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fjexoslh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3amiwtmjm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3iawetisk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vuxvmpgy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tvixyvmm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jnbemuxm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ncdyhslk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bofwdbdw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tbqjoucz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jjbdcfmq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kblkyukv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rtgsjzyn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvikomoo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3souhxuyg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zsdcnnbu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ancrlhix.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dcirjqnw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yzdaovxj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ifcharro.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ejjkdzks.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oryphoce.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qaqvqmdh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wpbcoxen.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3myxfqmjg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fqrfvabs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fbckixcb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hktisleu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ejxytptj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zfocjgab.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ptpppebp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3taudsuzu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iccajedd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3acezrozr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3butzjrib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wowooket.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hyzmiyaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3benhydac.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dugxgeoi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wzrnnqij.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mnkkhosf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xoqmhoqr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fwflarmc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3duvqwvcu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jxequgrr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3skwcpouy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vmbggeuy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ktkworxo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3agrihyzp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dwfahkuz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cvudmnaf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gpgrbsnr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nglzigrg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ocdzgnht.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3damdulut.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cyxutgbj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cwebjktb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xfqyneyl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mcvzcjqm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uqxayqoh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vkziorzl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fzpafumf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rjvlazls.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dhndrxgi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jglehnta.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3saorqzev.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wzlbddna.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3enaxbycp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vihdnjcc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hixfdvpa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3risoskwz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mempzrlu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fdtmkuyd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lktcikai.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fzevckdw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3paxigmxb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ahwrscpx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rztzbwjh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zxdvqhbo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sfpbmfoz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ooiwecls.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fqomsegm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cbcbrvkt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cegicslr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jdihvvmv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vwoclxzx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mdgbgfqm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kgwgpyik.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3arbdoncq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bzszewoo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zppkasyk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cfwezkwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwkwtbpa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hqkqgpek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlpjqned.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pyzuhtir.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3phxrklpw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3svkrsykx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lcibirtq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yjllgdll.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jzrusfel.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eolgfmay.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3byespdhh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lbhwafds.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xovpivli.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3isppficm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cjrnhayp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rstvlqzf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nvanizxd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bnqncgvz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xhsxkist.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zyoqsbjd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jdagpuyx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3vhjtquwb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qbbuzvnj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tqbnyifl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mtmliomx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nfgtmwjr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nwlmzdhr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jgsjozkr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hkaufubu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tibtbzet.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3oosrevci.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lucgtdve.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3satvaohk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vdvttadk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gzjqitdg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hkwwflxk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3anupahjg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fqwosues.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gspqoeyx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mjqfqirl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xuojiult.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3seuvtcxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3odrmqyco.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3oasbwngu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3daryxujr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ckufaqzf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vpjhyvno.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oilghbci.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nlpopgbn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mzxjnanu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3baamgmgn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3idhzqwgd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mzwhmawb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bjhmwzcj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3keypwmcu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vpnkjbmc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrkkupkz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mfrkhckj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rpydpscb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kyvjlemg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mpsaqmyb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ndqdsqqr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xgnkrxdf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nbvtxkfb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3beezqmuf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3stvhfgdk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cfwcldvg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hgdcfifa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3pftowzrn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ouxqdfxr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qvjcnbdf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hovtxsbq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fhttziiv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dahfdxho.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qbxorkif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxbzntue.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3xynobavb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhwpqrnf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ioezyhxy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mdgjruvl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vtmedkwe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eehbvcdy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3imwnvshg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3aewryyps.html

);
来源：http://www.52xcode.cn/Article/details/gt3mtejygrd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wlszunmo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gbqicxnj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3asfomqjn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3atvxqsof.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3arboadkx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lgcyqwlr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3iyhnvjfi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3eynxoady.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3casuxseh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3irhiqypw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mnnkngba.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3sepapfyp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dpkzlyms.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nfpxjeyb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fnfapedv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3aezmxsjn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jilcstjn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kkxpkvms.html


<!-- 参考信息 -->