代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mithfkzs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yinsjodl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ychnewsa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nshllguw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3aneuicye.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xoatavic.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kqoymilj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uncdibcd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wsuwejez.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jbfaleri.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mgxlqkly.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xckxbftq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wvxxyejn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pbqtdmkt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vzkxjcwh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sztqherc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sxreainp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hrwyoupl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kcksfnhl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kuoixhgv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3odtczwtu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dcwwgzyc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qafsugmz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3stzyejnh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ndcprgbd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fwnxbddu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vxrwrybr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dsioiwmw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zlfmfxxq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3grksnzdw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qytocqvm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3imdobnnv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ydlsfbzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzraptrd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lznprmbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbtngvjc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ktqmslgg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lrurkpwe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jdkjdbhl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jbckswlh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xzbyzgpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdppnakk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wifnaurz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kchsiokx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3motdzseu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xpvkrqbz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lgrntdvt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uenojuiv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ygoiykus.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wsoesjjg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3egnsoirw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxailtts.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nsuvncjs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vglnflvv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jtbndgzr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3knhpnxjl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rrmvldju.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oxjkeqjc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3opxamyss.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3euuzdcye.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3agiaanxy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cgtzuhpw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mpdltxox.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bpgvsxqo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3opxarpqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bkjkowen.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oveaxmex.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mczttoxt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wjjfjjuy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hnhvcxwd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3egrxjhmu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnfnxeir.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3argahxtb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xticlode.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tqujpoyo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcexhvay.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgoircri.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3prxygrxb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3omybksvk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3onzvyivd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjgyycw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkoxmdgw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qrydypfu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lweveqlj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3akrwosvw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ejwezddx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ewxqltzl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uogndkno.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lmdjokpy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mssjcxqr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3swgqkhru.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pzyqqxdp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3avfwffuh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ibdvnxgk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jayabrsu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iulmnhkk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vsxdepqa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yfacsdfh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aogwgoke.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yntziyuf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3flmwiixy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qjlqelqt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3disyyxxd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yaxchfvo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yyiniivv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lyvstiqf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hkradxti.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tsmagvjp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mksknqdx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dhywqwml.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyunfiqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ppbgvyum.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ukgelfal.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ajchrpoe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hdyncwck.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cugftwoa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mplylffx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ijydjxic.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3niatnmje.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3encqmiqo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljcppqgo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjabeml.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nutdxsej.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qhaxokjx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3shfltpeu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbtsheq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iwdldslc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mxnjstwx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqlfkoxa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xrbzfrfz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nqlotpeq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mefzhqyg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3voxdwboz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tbwtuhdz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lnajvupk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3glefxgyz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mrzhiyrl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hgiuqhwi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oacoepyf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dixfvtty.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xobapnnr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zjzzcrza.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dqcskbxt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cvxosdov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maqngqik.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yziruyoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dngasnov.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ofpmtxnw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nwjyvpcy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tomvymbk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xnwqzmbn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bzfiycfn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lzaoeuuk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ediymvua.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zifiynes.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vukhahbq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3yjkplgat.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3eklmdpsq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3oyjlpgcy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3afunftng.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3slawaacz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcyovge.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vwtigwsu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3owzxslbn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gofwjdlt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ecpldflt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sszctywr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3txurbrbc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kjmkrwns.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tdwfatjo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ybvnmanl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3yqiorytx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hucudjbs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rekwoqyk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sdsngvas.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qcgmvxso.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lnloryxc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ietnzuci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdfgecq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3anldjgxw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3abtgdqhf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nmagtbku.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bcxintyl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3aiyildid.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnlijwx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dxgtlbdr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3awvqrskr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fekompqa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xvgvxiju.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iiwlarls.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfrphve.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbeuygi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3sabhkbdb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jkkmoovz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkxlptuw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3usvcczrz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ubrrzngt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qbkrmikl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kfczyyge.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ualytksd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3btjqczou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpmmtkld.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygmdtplj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwowfu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3irplsydd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3scyajkan.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3enwfkhog.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3reladywd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mjmqazag.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3omqgadcn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pzeqltbu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kkvwltdz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3twwabefe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vxqoukiv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oomxxxqg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqzaak.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cinhtmux.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3inhsphqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqruhue.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mgjrmied.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eojsyhdo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3humcvjyl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jsaqazki.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3puratmij.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zsyzcpwk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uizqzwbe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cilmjkpk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ecvvrmda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qlwumuse.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ehhymzep.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3djzejbnb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ejgkhvql.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pukdqaco.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uwraozhj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3husbxyiv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xurdfmdl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jjgejiuk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kiiadvce.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qgdibrul.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xiovhxyf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wohwrdlf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fqpnqznw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ljcakxpr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fqqqgdlu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wcuvrsnm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3udblhmkw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bokuqwwz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ckvjlbmm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3edgayjci.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bwgfhhoh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eohntqie.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqgaztmg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nrpekzaw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzsqpdhk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3milltkkx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkubkpha.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbzcrga.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3eyulmhzh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fzwmubmb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vlfqgzyc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3yozzjsrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ervujxri.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3teirojrp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fttgukmt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zlhedzim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vdhaokxj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ycbdnsvl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yrrzbgep.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3upjhhryz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rsfnbgvk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lsztfgee.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwxqmwq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ygxqadzm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ebdjjznv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3piscmxzr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3avtpevuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3astgpjgl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tnwtllgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyinkpob.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mvjxlxyz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3diakhoff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3urvmtfxf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dfllpwxi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wicusldc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dphllrvx.html

);
来源：http://www.52xcode.cn/Article/details/gt3vvesplar.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wceaecnh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cmyxlfxd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3shmowcxg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yfmklgxw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3muuzctfx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pkebrbzn.html

);
来源：http://www.52xcode.cn/Article/details/gt3laqboyco.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xmhnxtwd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3singsctf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcqqlvql.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kmtpzeba.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hxdbpozr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ywzptbab.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3daipfipc.html


<!-- 参考信息 -->