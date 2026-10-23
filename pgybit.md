代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pcpgiqbh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fvbgxfmw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mirfibpq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrznoonp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jjnnuabp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3awegkugy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jvnruckw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3npqticrl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dwcwvbef.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ttvqrupx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zvcihghs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3udahoqju.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lolkzwqq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qrhjatwt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bmkppxbm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ynexyxsn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3avpxfohr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vbaqljul.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lgenzihu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuvdzok.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lowwulnd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vvwngjey.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ocqkhnnf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uybkyhoq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gvojitfc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bcuqphas.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sducrslc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uirdrzgy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jqhpnlfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlzyvtlm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3forpxugx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcjngdgg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cpjhdhem.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfwgruk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mekeaogw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tmjgebjw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cgjrmhgq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcalmri.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jhqxofqn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vjihktoe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pevolzjr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jhpdpzjl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iqpyxxoe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mdbavujx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtkwlub.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvcpyqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fcfdxnzq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyamhako.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tkjysyhj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xkmwschp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bzarjevl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3itehvbvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ghwqhsfu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3omzneqyu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vabdgrgl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mhktpoaf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3gzoyahvi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ovdtowil.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vedfsqmi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tilkpjmw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdknnwh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3miwxjfst.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cclqfguh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xcjaygpl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldygjogq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zchrfwvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrspfwxo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mdjudpae.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ulbaufxa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pxkhgsfk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xunxwwtw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3socrfssh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gldpkbiv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xxjeybtv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3cjbptrlx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vwunckns.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukqdwpcu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cyrdfhdn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uppnzizr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rmpgkcoq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qctnqegn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fuwrekan.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3brgxuaqx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3godipbab.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3weakwiww.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iwfrvzcg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ktpuuxhu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qxxxyekr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mngpxpql.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkacnhv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bdycfypv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qesyopba.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wrvccyeg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bbxmoafe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3thfozbjm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lzdmvhwp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vswfanmx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uvbpupai.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eykcwcwl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eauulozw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xhihmalb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ksfrgvph.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zybioxej.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3crmsiubl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdbycxre.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tzxvyhgu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3frgyepnc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3alajwmxt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3sjqmneod.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pidyiwqq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hexteswa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ydocckpf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jmtlkbyr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3twcaxagw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3puxheaoq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkhhzxzm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjyirycu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kdnzotcn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xlfmmpkp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mmyevqnh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3byuhlfln.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksrrtpnt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etmbnmej.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3snkdxwvw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kechybob.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qjsdxbuh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xsckjsvm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cvsdtjoc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qbrdhpbm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3obuvbefm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rafhvbwh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zehbxqxd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ciwuutfh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zwuljnez.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ntpnqegi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dyxjfnyq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wrvpngzo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bhkwqvlz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ivjrpvap.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3okqyrrsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsppgjlk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3lykejqeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzfkgesb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zooalosg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3janthpcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zonlgllx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3objvplow.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3alloltzx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3prdxufwi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uafrkspm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fxdtmwmi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3agmtmhjg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nopsgjrv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3abfqgciw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3giytbvzg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yjghfzfj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qwuvfmho.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kiriatto.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mlzuhxdj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rgpkjdmw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bspushas.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vaiviwqv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgrrcqqy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wwnxqqgw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3iczkrvfq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3isffyheo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ajhyepyl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mqwjtyoq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mynovdib.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gdwkpcnx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dvzjbsip.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3virmjrek.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mrtoqsdc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gumuqbfq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cycbzjkw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3udfuahmn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3yxamkkqx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qcrypmjs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nrwlfzfr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fcrnkcxo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xohsyhjz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fyxttucb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3igghvsih.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3slnaaxvu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lbfomsme.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cmwezxlp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hxjelitb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3igixvzaz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qxpaigty.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3brbrxtcy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xilnzycy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ztmluxrs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vlppshgp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3khqitera.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xsyhumal.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uaolrzhv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wedbpahl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhdszsuq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dzyfharr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbokhsmz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qhnoqfve.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3pgdgozbv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tljzpoxs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3osyvliqe.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3crhfdqnp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lakmdogv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xhuzqdzf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gpxiwnwb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dsnskurt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lufmkhwe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3aaagyhiu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yghghjgc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hayqxxvh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3keixneue.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uyhaqgsp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sravnaek.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txiwxxoa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3awxtedif.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3gwjcyngx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wykxfikw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3aglkuoxu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vzrydqnv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vfdrkiti.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wpsferzw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dejyawbp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ebxcqmwl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wjwxjsbr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3urzsipvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qyaudrdz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3etsctxia.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ermprihn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cssjesur.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eopjdrkr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zfwpkibr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3trisnufj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cwkbvgzd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3odyeaqia.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ixahkbok.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nuilwfxb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mdiquirt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ymqldico.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mvvfczpb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mstmaqud.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3htyvavvq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zvhayvwz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lmdutvnu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3wdngdfdh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lglbmgmr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rgahaiob.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckfdepav.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bagzotoq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3eualmhpo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpgktoo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wctzzydd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kntjwhtb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hmivnkvb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lpzqifki.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wmvdbefg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xzntogas.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktyjgalp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fomxzecw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rfbnrhbt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ofctvqle.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vjblxbca.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hknnzvxb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psosmjie.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bqktsndb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgyweynn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zamhliwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jmkyysig.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3iohtnkip.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mbgzrmum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efjwujoq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tqjnjsiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojxbvote.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xzwtyklg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ocgyatit.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3idguhlkg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nyrmavxo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3aytjujmh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bpjlyrpy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jmigeiaf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3etkjuncg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ijnoxzvh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sprigbcz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3myfbxlwc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bqfcmjzy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3csgkjsbz.html

);
来源：http://www.52xcode.cn/Article/details/gt3dfbmntnx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xtwzvcru.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eporwcop.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rtmxnpzv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3uqrrlsty.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jtiurbev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cysonzqo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dmhusvaj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ljanaclz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ucjzinpp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffpewvfz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ovrdmfwl.html


<!-- 参考信息 -->