代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2oplvqhdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vqjvnwsh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ohtwkolb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xedxpwvg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mhhkpbho.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sfyyajwp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2shhhyvfo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rnliqeoh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2orvuhmqg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cfjbzkoc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yrgrxgwt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zcbdjxoo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kgbtfydz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wckalrmz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2chhichjr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2smhficdd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2telyodas.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mzokprdy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bsnmppvd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hbpwyakm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hvcuhngi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2eflrppex.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mmzleznw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vbbwcent.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fvxbinrl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lxltszzp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hpczyjwc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dydwicfa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2szaplmsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgcbijue.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ajhovzsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmgmvqlr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yfvazzwd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cdkmhlrx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vjdekzww.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tyistuji.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pjbpfxns.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywygqdly.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcsfocz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2eisxoxpz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jaryonqh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tlvfsarb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lnkfokqp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wmgzcuxn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzknnef.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwxybed.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qhqpdlap.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2flbowqbi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hfuqudeu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gsrkairi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2yuwsufgk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2poricgox.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2laymnuaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ijtclixs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pnnvzzku.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hoolnofz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rpwysqbn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fwtmlbvj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gsokhxrl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jgaeazux.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ujzdtzyb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uszqludv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhojjmku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ssvqzpzb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2idswomui.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2apfvrrzk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dqzemfwi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2abzqbapa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nfcgfobu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hraiwqae.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jdivyqtw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lalubzrl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nuvffxin.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2aaknlmfg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgkfqsp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pgxkrunp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyzhnuvb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wybkblsc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dkdpldne.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2enifzghe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gvxphbkm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmysfptc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sccfsfnc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nifwgkhu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tqzysesg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xabzkwtt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zvdwblej.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dbrzubfh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nufmrqhm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rsitoodx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jcwumjbd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yxpbjhsw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tmxqgujq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zxaiydhm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2anldjswl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yueghdph.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bkhjysyo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kaqpwrwe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fmtnbmxr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2reqcfeat.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wtxznhra.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fypxdnby.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vkkszery.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qkorawwb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2guufiton.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yusvdtoz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rahaipeo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xemickkm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2acticasp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wdbgtnbm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tuaodhsg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yamzsbys.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iwixpkln.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xnpwkpfk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uioniabt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kwtqlrsu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zsvlrrcv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vztgbpjd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2skiwfqfk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nukfshua.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbitcgh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpqitapq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zdmugmlr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gqsixnwm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcilwvaj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wfyxvqzw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jreajsiw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ryvsvxab.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2obwvqqov.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ekbutgxy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgbqrrho.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xnisewhk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lbxbkkda.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xvejzkdq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nhrboyml.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dahrotcc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2crcxbwjj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2swllqzbg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aahamvnk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kkkluhlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drxwsjaf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cnravbev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obrwqyrj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fefzmoyl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zgywjetf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wvpvdiqv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2udsupulv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ybdmeprg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zavaoehu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mbtfgsee.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ngtxqsju.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qstvmwuw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lbkxdcid.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tdhdqbvk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2syhtvzgn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cbirifju.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qhmjsicn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vhggyxtm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ekluvkcb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2seimyrnb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2odzmqljn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jajqzern.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2atdlnycq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wsusqotk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sjzwtwuz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ktoecahj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfowbbbc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dvmewbbc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2blulwggg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tntsqjwc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nkfdgyry.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ghgiaxfc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xnmbphvn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cvcotjwh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cnfuzbhr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qxpfgcof.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wovhgclk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rbizbtvm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gshcsluq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lzednmfx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zytpgctk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ciwisyhw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wjtetlqz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yrleijhl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2noxqlyjt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2iiuqnjnn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nduricyk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqmevpm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cutnhjyq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zfaibzjd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2enypbqtx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cfepohpt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oesidcyz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nidrcbpv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kigsbrdc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kvrqfxgr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ssbgwctx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbsxybyh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hcpplazu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvqinnue.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gyyxzmxb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cevyjcqv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mxkwqicr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mssbycyx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ayojwonz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqjmlbbb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gcecfcem.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eignqesw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yirtdcgh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sugejxmx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wmgjfanv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2puvvcaym.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wyzyozlj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2iqdlwacv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2squhyuaa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dytotxvn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgzyxvx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ejrgmddi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wbduvxxq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xcifqnwv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2sdqiwvwd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2urbrwkna.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ibvwfhni.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rodkawiu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mukhmtxs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kgveywqu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vphgbdpk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yxfkzofs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jcsmcgnv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2smynkcem.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vekrtqix.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2aqxvgbog.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wqaihaay.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fexcdigc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ogzjtwlt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2spzkvluy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hwrrgbmt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jtlkxgan.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2igcoznfu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ascenppq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyyxwid.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2faflblej.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rgqizcwt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ehmfwxli.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sowhdcvz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2whkvcxca.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2esuhkdbw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2osgfpjyc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2eysmmfzu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgkahize.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yooddkvb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucnbzfvl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ummfnuwi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wqxspvrt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2emcsjfgq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ofcomvid.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hwtdrhhq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2otbyuvhi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qmtpdqli.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wmpwktii.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kagsxypx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fsnnvoko.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rsfgzkbr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2baaardfg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fnsivltx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rxzcbyfs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2osuapybe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ginnnuui.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ngwyamno.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dglxrajn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qoibyyth.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ebqjljao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rihhuvzm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kspwadpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idehhhnc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kyqahphp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hndjufsp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yntnctab.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2capykkpv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cuqxvice.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lgabeuqt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dcnypubi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2quoqndpl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ozvlntva.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vnszcdxe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ohwknmed.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hwhtzhqs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2blzmgpho.html

);
来源：http://www.52xcode.cn/Article/details/gt2kgyhtuaj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nsdkvyle.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dzsdhmim.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zhdaqjxx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gbdyciqi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iqwlhgkk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2giqthyzh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gbdwgsoq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2drslxjdy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2sdeeline.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mfxafpov.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gopihswk.html


<!-- 参考信息 -->