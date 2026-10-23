代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hvostpos.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3equpbefh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ttmvcufe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jpdnqmfw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pztncuxn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3obhsikhf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jizfvzik.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jdaercpm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xkbcgijb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qwfsqjux.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3whjnyfsy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rqqjmvpq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kdzudmwu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kyxfldnb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cbjuiyfk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ezturbvb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqypagf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3esfvottd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rlxyduvq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bclswene.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qpvhlmqn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dtmxoafq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3abzgysva.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aiodonmq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pxchqomj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kpcfxbzo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vbwutwdb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iowvvzfh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ueyiyhdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uroreevi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3awqqvfxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ednkocpt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jsewiyyd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmqrkaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uhegaday.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rpfrvwib.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glqhmvcd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gmnmleaw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymskessu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fcedwari.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mcwsrotj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3frrkhrxj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iogymrvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cpuxnwrr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qkbsgeqe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3feritxge.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tozzkyjq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uremyjyv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aydswfqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nxyzzaeq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yfpwrnuy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uyddtgsx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3adetdgya.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3viufuimq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yfsuztgf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rfaozlfr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3juvrcnpk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ulgxzjsu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ulzojmqf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kbovpklh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgdoozxv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgldjwqb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhhgrdd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bdtfqcbm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lhojjppi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3doespzys.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbsmoxgp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3umulzpsg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ktgnootr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yeyriayx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lubrkdre.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxijcwm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ptafushs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yesfuont.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3paimyihc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ciohdvob.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3uladoekn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jrqtenmb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqfbbuwu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nsllxhav.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iyfhgkqq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3womporzf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rqpckuit.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3elrfvscs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sdkzuund.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fnrsdqbh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3slullkic.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3edknlucm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pppdbfzz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3urtcilpq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cvyzesjj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3worqnxjc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eqzafwft.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tzuyndql.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gdzlwcoa.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gdesglid.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3eefpqnwt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3unaokzdd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3knynuiay.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivgqqkih.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3neernqcl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ckyhyotv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jjhbtyay.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmkozhej.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bvdsepej.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xnmlteig.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3evxziufb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3apyrbqhe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dchbageq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmbhdkot.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mgecdgeg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ujxlpdpk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xwuavxxr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pjdyutvg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hdntmnnd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3smyqvhbg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lvgiwvuz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hbicbtqv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yrloyiwb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rapaiool.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jrklsyvm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3weprlfdt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3octlkipk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mntkceka.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ywjgzxoc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zdswmpse.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gtksgqgm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsfavmzw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3svbfuwjm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lxfqxniv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vnyhcyxe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3txqdfkvr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lqsutged.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vljvgkyo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lvyyujji.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rwszbkzh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lejfihfp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zxvkocrj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bsyohomk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3txxxatep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfmdioxb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vvtdktat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvcpsdaq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3aztpyelr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmjwwkps.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fodtxkuw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cjklqxzm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lqkttsxy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ceclfgxa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3owwxrynk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3eyqfahhb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gjfamqcx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yzhpvqgf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yqqgrbus.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3aonwljvy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xeiepykm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3adyjogny.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qwydrjuy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ycbbhgvb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zuhciegy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gqdcknox.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ezrbuxmc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oeqxutwf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yzxolrei.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mgnbdzel.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pzpturma.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3stxqghlu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gaepdfwq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rfqgeknp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ektcfdfr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ithjfkbl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ybzvywrm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hmqwdbsc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gunholim.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cfufmrnm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3htshuitc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oafniqpt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3admogpsm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lneulnpp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3uytjerik.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3uitbyklc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mihbssui.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cjoioxyx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jlyrdbnx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xhpiksrf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qohzfwrz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzwcvwz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnczplh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lihwgcuc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kruanxcu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nabrifwi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gjptnbov.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ibnwmhjc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qzpdfzrr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kuztdpxv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3honubdwf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qrsfsarl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkfvrkhu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cnxbwjnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wiynywsm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3koveewou.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vkungjwj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vpxvqtoc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mornktsc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ingowdgb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jfakceev.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nhcrpsdp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oaakyghl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hlxrlfzf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3devumifz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ckevnctb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eulhizhy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wstzajpi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vvitmlkk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3slbkarpl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wnyibivm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3udvemhxa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wwcbmxex.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hbayekfe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kdozpafn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eoglkxxi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kypvxsho.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qhoavujj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3psyujrzt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jhlhsbir.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mhyanrnh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iuzwjwmm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ueqjumyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fivnkxwb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qkgxfnjj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lzysfifo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uknfksot.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3igvgwscq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgshbir.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jmklvxfn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lschsiom.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wwcdigww.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jpzlmhgw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qvlsasmd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vbpwicuz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmoqkhai.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qordlbyv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3esilorfr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hpdibbev.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zbyqzalb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jtogaayh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jtbjuzsm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xcguctey.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3exbvhfxc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufjqfnkk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jhpuoqkp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3eztnylau.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhpoqxt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftvasotn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tbluvlks.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3drevutlz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bswhdfot.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjuvnqkh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dxnibksw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmseffbn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lezakhcj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3eeeuvyyh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3raagbwca.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rgshgpkj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pekpyrem.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3daajamtm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3skwhwwnq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bljzlysz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mrlbiyrx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qxpiddgb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3stdqtoxv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jarwfpkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmnypjvq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hckbstdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqbvzkll.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3awqvaglu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3svyaubfh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pnrpnypc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kyxbxpdd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3skkqvjob.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mjjzxxrm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qhwqbtod.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3uhmthrnf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sxdecjyx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3linnwqgj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gugccmuu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3bkdsbjgo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tkrotyfm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jmizyomp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mnjaazaf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jgihijhm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fqisxoly.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sosqedmh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pudfsogb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3tblrwaym.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ghnstaui.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nosobmuu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wofbcpvr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pvibufjo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ewmjtsdv.html


<!-- 参考信息 -->