代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgrsufqh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pvkhvjkg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pydflelk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qwzjjamb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3erwejcwf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oaxrtjkh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rcricmft.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ltnnorwd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xipeahlv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cxlecslm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nhffcznv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mdseutwa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3htpcfwkd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jnuxluvx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zktantiq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lyrvvlqv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cdxbhksy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bwgpfdij.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qswfdgun.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yoyowatk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3yriygkdc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ntrqkkim.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nkbnxezr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nxrqgjat.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3spdumnrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nuhdnfhr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ocdrfaku.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kgfrqvuc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bsjuxxml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfuzpceo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uhticayd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdfmbcae.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vuqscnbn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxuyqim.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tslpvyaf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qdeuphsv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oslgblbh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pcskqqjo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbqpcjjr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hqhnjmye.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lijpiohu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xgrkocdg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vilkvghb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3stszinqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jyxbodjl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xoyojgkw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wiozahai.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdahbbrc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uerdewrf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3sscrboqh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ozyjxmgm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wmpjlqjb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yaxufkdv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ymmzmrfg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eekhswbt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ipjmospe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vabrkhrv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nubkneub.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3fbltuaxz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bbaroxjz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3scdsqgrf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwcqpubk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnjbzwh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ezlgccel.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cshhjynk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zowwlhag.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxklmaqp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eeemdosd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uyxykpcl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nnjrgrze.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3msxxulna.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohljwxvu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3duzqatwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nfulelbj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xitrmlsq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dfulkcku.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3phrzgpgw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pnozssmw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ftyjrsda.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qdtwnhpr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rtzxlhgk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mlxheoda.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mklzhkqv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zstcubit.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tefjztuz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pshzjaip.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3utrowtgd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qhddrady.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ozwhmdeg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3duebtlyb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jsyovags.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fpioorif.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3caindyde.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fyafuaav.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mctkjtlr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3losvowdk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzcdamh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3upruchej.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ghdkcjfz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bjumllsg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fyxipcly.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wnucnkmf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vnrzcqwd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yxvepmym.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bngpdule.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gtluyntq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kzjvfkoh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcyqzggo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3axgxbfqb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vzahdkuy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3faznmnip.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nshnszwt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pbyuzoxp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3melzrixz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3brddnmnm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rwlzqqkj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xdtxoqpb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mvuzvzti.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3norkdesz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zxuxiqud.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3litchbrw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ongrpnsf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ghtdkmmm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cmahqxif.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmoekgvy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xdkoyycm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gweveypo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rteoriqx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbqdkvnv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gvalmzpx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqqlwhzo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ygdpaxph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3advrkbce.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dvchbjsp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pgixyoyi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wrkpmbuz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rljhvehe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kngjzesj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3trfhjscy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3phtxfsab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruwwzrxd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3utotpzfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydfregyo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hnmclgtr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eaebalfa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjqongcz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pornumrg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cxoowxgn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wkmypetx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3udijwfza.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pngoahgi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3scjzycaf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sewgzirw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3itqqszzh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ndrahyun.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cpwoqcvb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zvgrhowt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pynnbwze.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ddlcuxmm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fsgayipc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3usyldgix.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jxvgxgdv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3blsmxhlf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jvklzuwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vnwkqrmu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3boyjzaib.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nnzblufn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3iqocxlms.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gqpnaoro.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iqbwioaf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3eqzfgxua.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3aigxncvm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fnnsucco.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wcuykkrm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpreucei.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fqldhjyp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3snhfslhk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zdgdyqjg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hezjclth.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zmcnkzkq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qrypxotp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3suvmbada.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zapjdjiv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tgifxlzj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ejjeqmgl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xiayvryb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvadkgt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3revwgajv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ffwcweks.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uspigyih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rwjbkgem.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hkujozvp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dnodgreb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3canszxgm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ffdttnvt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uckocdvg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3byplwurc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbjzysbx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdbjvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzbnjqkc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jnipqkig.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wycsjytn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3etinruqj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3igrdwgyo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hemklzyo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pxnhowbt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3knseslzt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mhdwenas.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3iqrnctur.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nohdgoow.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3aosphrxw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kcgpoutw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zmzxgbzc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3amhtgvbc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3roioznmg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3prkxiidq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgmftxqn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sitbcgps.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgucsalu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ystjcxai.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yfjergsl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bslhybzc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hpmnepuu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bihbmunk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3aokisfwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rhemlyll.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wfznfcob.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xunlhqde.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wgfbdgws.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wwwbairn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qbwssbef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pzkrqzts.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qtelxcjy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3svmviwgl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3cykcbdfq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gcpipzgl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hooojduv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tyaxxncb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jiggvpjr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wzylmgfg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ojgajgbq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3avkomvkb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxfajnb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xbzqnwwc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dsnhncpu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zjuitsmc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gniguulb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjduzfie.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rbazbhyk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3pzvfpcgn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mehsjzag.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bfujysut.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yfuyayqn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ivpghdqx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dnwdlwua.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qvdooihw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vpiilhww.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lgsqaacx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tephpszy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vplhxsyx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zvdkjjjv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fhdqanzf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kfrxbuda.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zklggyyw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwyxqms.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ajpcaxtg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ljgoboro.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhilaygl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xklydprs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wtugeufd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3sgnaurwg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qtjesmtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfxaquoo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qkcoxpyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fegymrnj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rhrrdzjp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3igsjpegf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tncbupyj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qurxyypw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3odojdhhd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dfyfuegl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3thkvqqns.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3boapwnfx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3grvtdjkz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lmnqspeo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zozjpiad.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kcnznjrm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pokcdwds.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mrannacq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3edykejdp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ltcvpskt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3puhpwago.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iqxojfuj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qsmgqfur.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rvizffgh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ujzepnrw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3uwravvbt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dosoexwx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zqssnzbw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tgtarwwm.html


<!-- 参考信息 -->