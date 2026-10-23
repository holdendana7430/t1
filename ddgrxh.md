代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sitrkjjm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zvtcfiwq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xdbryaxn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hokjeqeb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wgvrrhsw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3lrljzcyq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zpldokll.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3woapzxeu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ffyuwhkw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nhxtwrtr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3llltfvcz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jnmhkayw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wyzprsdy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fqhwlvtc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ypujvwhw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qkcrkbhj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pxnjxaue.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3sgtodtuz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3apdpuwyi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ysgefpwh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rulrzynj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3twsfwiws.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jaeuxvfk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qrxxgtwn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3uzrszfsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcirwggm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3weenbyff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gibabvcr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3przqyjmy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkllkzzj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3awrfwcdj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gbjljdfl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ksxymwim.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3woiwuuuz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gflzmwoa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3etjrwlfw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ufczptfk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ftxghcff.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lkbdwcfm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ipgsownq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pgyrhuqi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nalbmmik.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wzlynzro.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brfvoumy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3abpdtfdx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kouashjb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3elyoblni.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pfkilfkl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ikkqdxxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nynhjgiv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3loibiaii.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3noraixtj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wgwkjtcj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3reqzoavi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tagwcdrh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kpamwdxc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3trexzmeu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgsylgut.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uhelllue.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3btfpvyre.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3abdzyjon.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zvswlxxz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yxkpycxw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hmaxgkvi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3udqenrbp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3grhoqxzm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cwroatld.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvmashik.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzrusa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tlenkuzp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jtzillys.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yxgfurdq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxucybjs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmtrzkrb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ygrylhdg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qcjngblh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eihvdhdz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gvseomjz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3syobsuiw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3orwkfkae.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tkpxqong.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dzwxllel.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qnmutybo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bhbbzbji.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pbedckat.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mywdetuu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cfrfatku.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ywqivseh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cnqwurew.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hymxsbfc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lxjrtbxt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gnvahocs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvwbzmeu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pnlnnwmz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iednzoff.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3amhacmqi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dyihhtoe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdszayzc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3icttdauf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oqtylvwu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pbyatees.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vqelgnoq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmwnasbh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uowobcgj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nlzsiwiw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ttqmofhk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dddltgex.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xpzcotid.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hogbmatj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wtiloeuc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bshuezzv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zkmrgmbz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fsowfxrp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3muvffftf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymtaqgdo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ggkzhmnb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wcflnpaz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3llsftqsv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wqwgkbof.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3escclbsb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3icbjgslg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jwgemiju.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gsohjuox.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckjiggek.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfuiaxgw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bnpdmqrs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hkqazurx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ymoouzeq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3censpzul.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xlovftuw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rspwnhnz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hufbzmno.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3usnmdlmj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jyzgkxaz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3odlugrei.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oezdueju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dflbfhpo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3uiunomcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fovdeyoz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gnsgkejq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3abboshlo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yqwiubld.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3eblgfjbn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ehasskhc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qzrinmgb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3taxqozoz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3chajzfrm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3kmapioss.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rlpeierd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mqrcmaub.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tseoeoyu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jlzdsotv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yifasfya.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3yyrvobow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pgthqkcc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3phzndkps.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pqjszuex.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dtgejkvw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fhdexnwb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mieckrqj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vvvfqxbe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tmajpmze.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3luedqhuy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cmdvptgp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3syhbjqiq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwlnpexz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mthqocks.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nboqhvlf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3skqffvgf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ldtlujau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsljjrey.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3nxqhpwdm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rettsrhi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yecsdbld.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnekochh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qlfivgae.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zfvyznfr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uktbhjwp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rqbsegtf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqrpwrv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3psvdziis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3eqgtiwbe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kivexlwn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxzkchoc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nuogbbzq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xyvxftkr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ylcmhvur.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xnfwpgaw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wannfyyh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sjjhdpni.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3sazelexe.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3elpcohoc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3aveuuixk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnwdsief.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjnoiupi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roiujxli.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ehoocgmj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3iewwrspj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3haakaoxp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ydfyeuni.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zzvsajrn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cmansnmh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3baxrjtux.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tnizhpul.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yzpxlcnj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3mpbqblgw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hmkmjzbj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zhothaej.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jbtcrswy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zhtdptrl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3esmnfbcr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kkffaxmx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcksrvnc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ivpfmjhs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xkzabest.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bycutiau.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zjfhhlbb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zuxvzcuw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3csnauucq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gbmzmojp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3junizsaz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3yywdzlvi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mcfffitq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lyvzkjey.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dyzkylkj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kigysxwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sgssyhhw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3noycqmyx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ksfijtnr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzrmhx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ppzgpxat.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lnygyutw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3uhgmnjhd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ufeqctqf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zimocvns.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qrzszxii.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwctelod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ziixajso.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bewjogpk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dvxclgwf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ssbaasvw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pamnoxtz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3axtcsvfn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ypkxatrh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ipvgfxyc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3matlmmly.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aybewogz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuigrxvx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iszxepvl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veeudlbt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bptdublj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fddwinpd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ldijpqij.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eddkbqry.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3silusjrj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pabnfbuv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3stchqpji.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3trqjrubq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ioefiryn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qhokgrdz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vvimunqd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ioifbduq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fparzokr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oxqzixxr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vnzdyipc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cmxdphnv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ipxghouh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fqyuyzqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mglimtyb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lyakqovr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilmkrjri.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3upjktbiz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jznohcsk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ocetavfx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nyyyerda.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lzmczjtu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rmeuufxs.html

);
来源：http://www.52xcode.cn/Article/details/gt3kbzvltox.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mhejdfcs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xwsacsdn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pqzrdldh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hdtkasai.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wfpksgkn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aupaitwj.html

);
来源：http://www.52xcode.cn/Article/details/gt3pirkymha.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zhxvmtnz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jhhqokmk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3puilahvp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iyuxtnpw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3douuynhv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xfkjfirf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xqffqhyd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ursjujot.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eonaubop.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kckdtaca.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hmiwgkmk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mjznzpik.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vqkfvwwy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bcnvakpk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zmeffdps.html


<!-- 参考信息 -->