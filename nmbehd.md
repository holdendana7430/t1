代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3krfaremx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tpzkfhew.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lmddlsix.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ishqcizd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3igxpkjpl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3btieuupt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3furckrnd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gojlvbsx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rkoyptxw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3depoukpa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rbltuctr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aeqjlfeb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3etgmtpyb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uajpyauf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rmsqvzfv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3enpriptd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ydkstdar.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dfbauszr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kkvtoxmu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sslsardz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mfzuxlfv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qjdxnste.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tugwbvob.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3smbeyrhm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bgbltrob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpljdhcd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yyuqwufr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnggauzz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bgqhgtqw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdbabcq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ametzczw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sfilizjd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sseklywm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chksidmu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eivgkmcl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zoeuruzs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjbkbsl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rcwiloan.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rbjbmkph.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ckxsddjt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vpqeuscl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrxoifk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rfpkabtb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erskfaek.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3loqevfis.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nbzwfxdc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3uzxjqhqk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfcbas.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dseptbma.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ijiucexy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yrmnyglz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zgaraqgt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nlyezmvv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jasbocft.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lnhtlaqn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pecpibnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hdchgvhp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhafbldk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mslxgskj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lpotyexq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtakktl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tfetnbwe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dggpsxfj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gutdnjte.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3njsulkug.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpboaqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pylfozbf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwzcrfra.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3aahzaint.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3iwarysxm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uhgenjsd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwecyya.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfhgejqt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3averzymo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ytfqtqyg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rpauutfo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zdufojyt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jsauzsdf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rwqypopn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tsggkkcd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nahfvgvk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ckvlctha.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zuyuljgd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ttxbiqaq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jnmpevwg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tenbgtjd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jlbokwba.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ovlobrqz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dkgnzbpx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zqdphjyc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3viosgqmi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bptysmem.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtnvazjd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ctaxvnel.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3emtelbuj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycfugnnq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qqwoxkub.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hffxtprg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zfhtpymn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hcfghbvn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fajgvlls.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlgjscsg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3grxjyaef.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wanggnmg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3odxdcbfm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wxjzniit.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hfvizrky.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hlbaotwb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gfxtensw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hnvtfaiu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3rwhagaxb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmunkewh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nxecwpcy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hbuohodo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nokxxsxd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mwibgecn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vquqhskz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwlqzlqe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3efzpvvho.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gywnqtzp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jukfjibg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kgpbvgem.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gjurwrjp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kdyfskdo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nnpqmmio.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3inckbljp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qpdoxyzu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ykqybfzg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gbmawzer.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wnzsbfdu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pnyipral.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wkionwer.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mrippcxb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mxmfxggv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uhjjdgmb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jotifjql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktkwapzz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3oofuxqxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqwnlbnj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ggexekvl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vbhqxnsg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bbocemnf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vbmggtyj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hozorhvp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qoykfdrc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ekpqinaa.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3unlyxpii.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mfnlvjmw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rccweizp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dsphplrx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ppctrwnj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lkkxcjgh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yyfnjwjp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xsttwfgk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tqzvtjpo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eysriqaq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zzzilumz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ciphxuvc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydjbouvb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ufvkerno.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dtfpgxye.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qisajjav.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xusfcpwn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nkcpzwwb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3riedncrt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqwknfd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xyarpxon.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qjkjddup.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3twslfyrm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxhslsqg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwpoviva.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ftubbwzd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nvvvzbmt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ebnpemhd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sahlupty.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3drhuyvfa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vjemokpi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tpxxephn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ijolzptd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3amqavilw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ftpsugyi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3otwxtvmp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqlmebl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3umkjxqlv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3iehxpgsf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jsblacne.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3biohzbrj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3axpsfdwa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dihwvuhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3njqmaxxg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yodmkegb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eavyanrv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yddlsnir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsdclryu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3eddgzezk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihyuyrfy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xhhdhxqt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ouomxozw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cnumfwzo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yfrhlaxh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yxutrfys.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkbfpuue.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nxfvtgej.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ijfzwyqk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jnnajgqp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kodyufgv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jymciqjr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gjlvpgfl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hfkwagvk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qmwhyfxr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dszhipzr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3weuqfmli.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wnrxrsgp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jcpykfgv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3onkkhhes.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qfiabpak.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uitracep.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qvozludk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gouvcduy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3udhdxmmb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ozgqiezo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwbznqe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dptkfydn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lqalzoog.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fqxmcsam.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ljxidjzn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hvuvuamj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xozlhehx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tdfkcsbn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3romjvoun.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jxlleclt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3avbrygnd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ugczegkq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ylvqfxdd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3twmpdtuw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zdqychtq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3srjcfkrc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qzrghqyg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgsjtxm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pafjonkq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hbsbtqic.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tapnibje.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xgnezjps.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qfhvkxak.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3culpdrwd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3klqjtlzo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erztsopw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dganzhsa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rlqedchp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jabpxpyn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ltlfmrnx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ipmxxvuq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bnfkqmjt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mouqfvzg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3agvclulk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3iwhetqms.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ktdoucpw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ntcdjket.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tqifteyx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3memfsqtr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3yhdutspm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bdvjmqqb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nneqekam.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oylnzvbj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wufbhefp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3irsbgydw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bdavvolj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zzxaodui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxgotmni.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwesga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpfxqafh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bbiqhxku.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qqckrcmt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ngsxtbss.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ipaiafcs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lyhorjen.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3epwarfnn.html

);
来源：http://www.52xcode.cn/Article/details/gt3zlwowsxk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dvxuwbsr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wyincxkg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wervgntz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dzischos.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hulrupzd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3akzycnxa.html

);
来源：http://www.52xcode.cn/Article/details/gt3nbdbgyrc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pwgprien.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3typadnfa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3trstdaxa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pcefkvjf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hvuptlgo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dnqyzbjc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rqmkymac.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ajsbslan.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hjtermrx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uzejiyhh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3eqmloyzp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yunrgrht.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3oxvvfgqw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3akmgstbq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xnotwzfa.html


<!-- 参考信息 -->