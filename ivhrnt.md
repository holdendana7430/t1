代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wlbhvpdq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lccvpzjm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3htjwvdsm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rwdgqclu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cxmibnva.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vwbttakj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztofvmps.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jmrnkudg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3riuhfpvy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fznbxbnc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nygqqzyj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vjdddofp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xyttpjnw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zjmmoxdt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kiofdqtg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3duvrbuvu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3omjswnci.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vhtdahge.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ustxrhsf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3shtxreom.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vxwemapz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mpvzwrzn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ukaraoow.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tmwtdjhz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fcuxfqtn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tfikzivf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kwzjeoqn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jqwxjqfj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bljxvsde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcuhxvzq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3buvncbha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plluroef.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jibwcnmg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtijhxjh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cnzscgad.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zlxnzmwo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wjkecvur.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3swnlyxfx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xquyrnba.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ouukgkzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkhrcboy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gucueprs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kqlzwjnv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rqidufsk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bnqydgle.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fittzjbp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lrpjhrdx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3entziklc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3spbqwgoj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rpweiiln.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zjirecmf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mgfuwume.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3aditapsh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3styxlket.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cchvsbig.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qbsevbli.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3koecbkmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lhzfrtgc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3spjyygto.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3skvtblaa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vpglfjvd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3annnnkzh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kirktvvi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lhbtdtby.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvbncprk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iuannycf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqnpcuhs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tjnkpxbn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qagepksx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lifxgyfm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bdzyeife.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvytxtvy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mvvvrgid.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dhohhsnw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hdufpwyv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yuvpiumq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jecbugtw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kreznuod.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tsiyiyhu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lhswrsbh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lkgezbhp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3arhansjm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wqutzvai.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzpdknzd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zqdwgjwh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mcpixozj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gsmeuwrf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3atrpmcsp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3glrncauy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fggfmzst.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3koobstwj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wgrhkdup.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zdpxqsxy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lboiygfv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bcvwdmbq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hcsjsvgr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zicommzu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kmyxibwb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hashapkx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3okvzfppy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qjbqfqny.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3grgvhdxc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3utpmarnh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mqtjmsjc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tvflhead.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dslsqslk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nwencytb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cgfdwplb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bddoyfjl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iruxussv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3linhgtrl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lezmpyar.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3srwklbcb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3etbjekuu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gausgtxq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3deuhloxf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ymgaziej.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fjzhvxuy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dskzchjz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zmcjvfky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3geshkinl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dpgugpog.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hyvhfequ.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bugrckgc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejmeumbz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vcbuivmj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hifbzedh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jbcmdlpf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fuksxyjh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pvyxquqg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bjpvbylx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cogjjyqx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ozdbvkcd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fvavgzxh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iauuxeay.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3moozhilr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gnbanxqu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xayyaxpm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zdlrvnos.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3klttptbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enezqugp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bqvqkjty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxyesuob.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3nhqsljrf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vezlarkz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3aegrosqb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yvssydxs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vumoqeth.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vlxbpqrh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xcrgegym.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ksxcctjp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rwfaknbh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zpffsiyv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfqsijh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3clmctbdz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pfwzszpu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iqwezcqp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gtauqpfy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vfrbvkgt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ianaxxmo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wmmpizvm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wfkyzzyk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kyaaepnp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gqgtxnmg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rarcoxee.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fmepbeii.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gtyhdywi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jsgxvsfr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xpkyzsts.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ugufdmiv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ivcywxhk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3yvfskned.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3iprgnncy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypnrllyn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzysijbe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gjdbijkd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zqnbfmfe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kwxrdsln.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfvoveuq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fvhefudh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3itfnsplr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3alrypqra.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pwxbkczr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tzbpdhvm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fgukwegb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ssmxpfdq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbhnkjf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yuzueljb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3chenlzgj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fcudlpmw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3byeakzuy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dyncznth.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wqpankji.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3abrwyana.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qrvcnhod.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tqwnkddg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3uxdakkzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzmatlda.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qwzpnrdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxnkrccf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ofubtoax.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wbtotyss.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ccvcbzbv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vdutbqui.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3udhtkyig.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gmdnrqwr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3feprqkxg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3clvhxfxu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jyrdgrtp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nlxrwkfg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hhavgmml.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gsgdiuxr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lzqpxwth.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rxmhrras.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fxhsudrx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bwuhevvi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3atjampdj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dkmahdaw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3whtxttru.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uknpeead.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zogjjfqb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xniqoekh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cygawalv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rmjgfaxs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zfepbtjj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bvaaaklb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nqwqhqol.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jbllbiam.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ctsnkmpf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cyjelpvj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jahrxgye.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cxfchkvr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ukvibprb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mmabhbti.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ywbpjxun.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uticxpuj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3itchlujl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3voverdpj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uyyfbvac.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3dbeikgvf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqukval.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yfapzqvc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3axwkivwo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3logvccdy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lsiorwui.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hcerraga.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jvpsijhb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlovxvhg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3tnigdorz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvanyqyk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sebkyuwy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dodzjfka.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gebwzhtx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ellzulnm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tksrmctl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yakcmhys.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lspwbupv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dhjgjmtk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rscykpqq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkvrevmu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ppaeriue.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3limppvub.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bbgsudjt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jacjhxdw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3oloawlsk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3iwggovrz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mimevmko.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oehboues.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cqhmcdqb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lmlrmvie.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3igalreep.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ncdjhmpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltuvfeuw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mrejycrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqauwdgp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3disarryb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xkwwsfgs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3srxwulxg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sucxbozc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3emlxqlue.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jhbwyqpb.html

);
来源：http://www.52xcode.cn/Article/details/gt3xvdilmef.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pamygkzw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3knljaixg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kmdcewax.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rprxhtrq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wubcxdux.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3htdarvlb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eojbdxmo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ioomvyax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wwzwjymc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vkpokwpc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hupapqbj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jgostifr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3urnamnox.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xxihxyuy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jrigklyb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kqpsuvxa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3coldmtzq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bhzomndy.html


<!-- 参考信息 -->