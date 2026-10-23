代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3alpqhzrt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjinufki.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3giljjwmx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xdopodue.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmfflhrw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tbtrgfsb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vemtdtpo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpiqfgmu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3waagufkl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mhtmrnwh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhcbhzj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cloiwvqe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ohuwlbnl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qjgkbcou.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kowboxyf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lcsghizs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3obqjygdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dqekbdlx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rxupzfwp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sreqkaow.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vwahbxva.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fgpatkey.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gndunwta.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jmxggxwt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gxatnyoz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qxhggrov.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tbnwurgh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pbifmxdj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rlimlymf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ejbbyodz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3scynlnrd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iersoths.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hbaquoog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvdudtkr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bemcdtkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kavfeeqt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mcifsxdt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kiwkfzhb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qktzhgel.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgelmtn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rpnvvswm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3forngaqi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewhyptoy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqyywnp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hotizgka.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oxifdfun.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aldylldt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3obfqtuqb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ecxkjxjq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fnzpuank.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hndbysee.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdmubtbn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ckkthtge.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3taqkjzod.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zpzksfsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fwkbkqvg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3aimeywyz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gnhpucqf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sypftexe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3obbwpwcb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3buhswfei.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3eayhkjsx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zsilzphl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fyrqaaab.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jenrfbhe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnzzstuq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3spucijir.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dilsqnwz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aayihqyo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3blrbfxrh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uleksdyo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jmkwbnjy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sghhvglr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rolkjsom.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ilfqbquw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rziuwcsw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3safnuptz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tkjikhmz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3utcudcob.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qklpmcze.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3emlueyum.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3akroadig.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ykdbqwib.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkkcvyh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3veqxqlfv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qflacspe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vrfmuhce.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3aeueywsr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qakpfbky.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dwmjntuy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ktpvurzj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tvxdatrr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3atfxivhc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mhmzbrjv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ljgodyne.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3horkombl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eqmozkbe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3niglfzpm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vmpieqlh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pmblekgr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zodtgczh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3snlgcaxk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dpanrpgm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytuskesi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bwcjnkzs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxczqjcj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cvxzbhje.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rxkohgnm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fwbrywdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3draojoeo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzbacazm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nlqmgvjp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3safshsvv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pbybjoqe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3earmdbud.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cjkooktb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3enardeco.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yxygikcw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gletqmwh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzawuym.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mkcniroj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fewdvnhh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vfbfnxrb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3joczblrc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wjdpszrq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmqodniy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mrmknznh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3exnmtfmj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3isbagmzr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ifczakip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kbbkzwiz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uytzcqvl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3huoklqsu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3clbtankf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3esipgoyg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zzdiicbw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ijitdovs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wbcasszc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kkzhldhe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mtqsulym.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3alordvnm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fjwqxuwx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kunmolfr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uvbsgrxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqqeceyv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xrofthgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umxdyabq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qdmcqatm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yzvcmyum.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cxiiilqr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cdtrzvls.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aideoqzo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uffsgkee.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xowyxmbv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fhtiguex.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hkjmonek.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gsrxainc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jtewmesl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vwxhobaz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tvvuvqxg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3miesyxqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xczgjyao.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jirppmkb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gfhaxmkz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rxkbawsj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3loqayjdm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mkkrpmnj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ccojuivz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wrdlnitn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jqzgnggn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iowwxcnc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ptptqwul.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fvnzqacb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tumewrzj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3oedouhiu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tajwjrck.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vrypsufz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gypmdrqb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3paknljfb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3oiqzgxje.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tobpgdtg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ztzxwczt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uoyvbjii.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3brmbfqqq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlpicrt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3muafyiig.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kvdbanqc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hagdmqvw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cbjhtmdo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3iylhlypj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hltlzhpe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qvlfbmrr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cszumfcr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3odtqdumx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dinbqksh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qqmjbkgu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tljjznej.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yvpgefmn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ndtgqikp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bkycrcvn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kbqvivrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyidsuaq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xilllduy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxophovq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hijwieku.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zszmuozy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pqsnwpst.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ozmnlwmh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fkjiqdjo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jsrnnfaz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3afeccjpp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pzqwrzwz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tskwdmps.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wicpbavm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ugxlmfiu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aeroulwv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wohjpypb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3uzokzwol.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wmckxshp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ittejnut.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lidcvjtg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hyyklljy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jedbhyul.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hwfgqcco.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nmxemqhn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tazuywlf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inxjeijo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjihmyo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3noxyhldn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vysaygjg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fxakrrok.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kngmmbeh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3buystwjg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qxnolwzo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xjgasvol.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oxuagvuy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mqqzeswy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3udlohcfm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hpslnsms.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3srwxkxda.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zsyizdci.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kwhptvwg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qxuzqnph.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fwhzrfeh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tdemdsaz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dlqrvozm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ejmyyihv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rjmpagwf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ozhpbtff.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3phverlrq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3moipmbae.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kveavbhx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kgfmndwx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ldxyxqsp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tymjqjuc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymcimefv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3guracddi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nmintfwb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kvkckpvt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kowklhaq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wwnmmyan.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ixocjhqh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3upqhnzaf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gsjzjsjd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kwycsphn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pxayyrvl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3brggpwzd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ssmqrglv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqjeqkw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txykizan.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qxaxenmm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlidtxko.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3snjqcpgx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ysrslcde.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yyvjbsht.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3askgctwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzmufyfb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mxflbhnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thblbtdm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cskkcbkp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3cetcjzqf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qbdnavnr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3apcnusgh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3aoddievu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ufvseqxd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tzglzlcn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3czfbzlkf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zwvmomuq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3klfebmqk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hrjpktod.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3abysmmnh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdgewxf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xltggpco.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kfkqqhvt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3aunksklw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ahjulpcf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3umdhmhjn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qmickwzu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3feqxtikd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pkytqate.html


<!-- 参考信息 -->