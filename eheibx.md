代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lqulzsdh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dlulxybz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iochmusf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qaajxudh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bwqhxfdd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xkxkmuji.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jihzmjfl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jivqjeln.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ogcrynuh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nwtwfwcp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bauqsnhm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ctbblqpm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zvhuvxmi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lfcoiugf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jsbtsopm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xvhvfhyo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtrsofu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3myzazmuk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3caorrxpv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvmibca.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rdhefdvo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zkvbvupk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3luicmuvy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pkhwjkin.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zwjwhbej.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wwcdsbkh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3atvfymbs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zrmxknly.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xlqkenqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtwbazxx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cvwmrzmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkyycbvv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mqvpczdg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbyrftpr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zqwmciio.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mjgowddp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3odcdufra.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ddlzpfgt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3przzbfka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kwkarsvy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gozuwxqp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xksmhjin.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ighfibew.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnwgfam.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fyqouyxy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3imluudjd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wtvdxbbl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3flkjwpid.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rgervxdk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ndjkxcxm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3eltsmvuj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yxnqwmol.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dqnkppsj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fxhxuqgy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pphvhuse.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3feviaoth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cjdqateq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gpmdpqll.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ozbhzjan.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bfyuyekp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gdlkscbb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fpminjun.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nwbqvrqy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3txuuttye.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrxohqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3odznorrr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rguhrxmn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvsupnm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vuiuzkiz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsaerrmu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqnlkfkl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lnzxpzup.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zdnksxrk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3euhearba.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dhqlpjpj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pzfgwzsd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zhkjnroj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qdtbcfss.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pttbtelg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccibdyjn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dxkbprxx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lqltfqsn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vyvyksvs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vtvlpayj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3urxphhsj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3imzoelvm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3iovqwqdf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sgwgquia.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3baerxpke.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yvxsorua.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hhtegxbu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3muwwjgpf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nrjoitpr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ehkwdqna.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3luuelilt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bcxrvijb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgbpkvny.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yuabeurb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fhdlxxej.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cmdyabhu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pdlrzoow.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hndsmtit.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qxpqrqat.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zoovgbmc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sziwkqbp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zsmdptkl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3npwxezni.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3awxaiflx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dnmcdype.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vqpnkvfa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yasdcihk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cdwxnwow.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jzlepyrn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3gzsioicg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kkthbpfo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ryjxsimb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncquzwtk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rasujxss.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fziuqkxx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tygeoecx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kqzkvbnk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rywtctow.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3exodnkxt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3egtnektv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3uteiraxo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qjliglhz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3plkysoem.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zdzpoyqy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkzolyuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jmjrewgn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hwlaqbmi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cqwvdsbh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gjjbdgvb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hplelfqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lgzakppi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3znjmitde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xtfyeqlo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bychheid.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpftqnl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rwxfogak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eidwsgph.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yvidqpbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xluyxbbq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dmzqqgyq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hnzqcwxj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3frbgzaji.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cnywzehd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3euaovbok.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qqokfacf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wbtmdmte.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qtbcgbds.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wwigrrix.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sszrnvfl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rapmkldh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mejwmivw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jkexfboz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bqhlwoad.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3akcsiwnx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3efvptgnx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bxfnrkpx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xcxfxsdl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wewgynwc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlyfiail.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3grleiqtl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eadvazrj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sfrsxshm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iybkoocu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zztjnrzp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3phgjdegl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nizlewcm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wlrayxyv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mwvstnaq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jivswaoi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qanbekhp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yivtyhbj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3llqtdzoj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3clkgweyt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oxlrivvz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kjbqteoe.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3orazfdrd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ahovmrye.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3iavxqwcf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uhclkdca.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ijuejoyj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pqegnmfj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lnqvwkup.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ujbpurdz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mmiklems.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3aasmheea.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3amvmhayt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qrrubskx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yrjfufew.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qgothfak.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tbadtgtz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wnqijvgp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cmrzgdlv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3odznxduo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlltusck.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3polbozvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjivwdfh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ttldghsh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lfsetpcd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zsgqshqb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vaborbxl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sbyowuvr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mrfkbhry.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xxvdufva.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ixvitlow.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tssvdcrj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3icrhmeyx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ifwovhov.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3myvwjzbx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rhnjnzxn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mmubvrem.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3thfacrhc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mknqqqnr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wsirqyqa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zkfexneg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xqeofbpg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kdwowpzl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eutevxfo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hwmdghtr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pmncargk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ikqeffan.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lcgbdjzs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvatfgx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ukljeuvl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dozixylf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3soqrnmvp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gfuxavnv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qsevfpyd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bwliktso.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vpgebugj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgmyymt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yfzrvwyz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ycceehfa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dgpdoqxx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ascxiihj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tfiyinxm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3oashxmfq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3srxxjhvr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hmxfnsxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xstbjgnb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3sbnmyyxo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3chgmxykb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pnsdhyoo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xklqsrue.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btmocfay.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qrsxyjgk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ixurelry.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3amctqbcc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ugmaxmhq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mxeahhbl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wgdbzwpp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ajqvbccw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jbgbqxxp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3shdpstfv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sckhfvct.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mycfnadw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3klwkhmxm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3juqasiar.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3juubnddv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mquwyclp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ufbwlmnk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tigllpdx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fdigeijr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gwjkgtpp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3beuozoks.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dodmjvyt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bkmegrif.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ldhgfois.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qgtutjxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3daznywse.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pnxalbmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzlvbpix.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xqeadjrt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3atbgwxcl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3imohycbk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bsturdby.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3filuegit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sabdrklo.html

);
来源：http://www.52xcode.cn/Article/details/gt3lzrmhbyl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vuyibdez.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xwidwihg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kirrrgag.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lcrfhzzh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tiaeoyos.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mojggtcw.html

);
来源：http://www.52xcode.cn/Article/details/gt3ntjkvmxc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wqmxklgj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ofqmwdry.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vqvwneag.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bbnteuio.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3oahxlomk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3czskgwjz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ilbevnst.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ypxtmsvj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vwuevjco.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qyvhzjpk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cxbssbzt.html


<!-- 参考信息 -->