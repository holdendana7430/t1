代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hucrazee.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3omjzuidx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qicqhhxk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3muaptnaq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3npuhjlpg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ilgbtmcw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oteaggly.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jqhxewph.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3njvuxxxj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3sjdzmvpm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vcvilsdw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubzyslzf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rptwdfkv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vwamfzwm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zdcbkfyy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lgakkvag.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3smhgmqcw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vusecuyo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yupareyv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lmhnblrh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hfaedkfo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3chvilvpw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gcpsikuz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pnbimdpf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpowabb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wijkxfhb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wuvvttvh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zayvruht.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3csoldism.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nkuxyxlb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rqtmjjsc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yctnamny.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tkcwmzni.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3upyywuli.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jzezqgik.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tqlxjntr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mdfdfaop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwrgfasx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nyfckscd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtgnpisd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zobtndgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tdrtedzh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3smhdxqlo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ynmkbptu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vbmgqanh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyilyvea.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jgbhuufo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lztysewz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhnlckdi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wcjyvuzd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iewqbtfw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bvmhxjzf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nkhxhyrr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mevkwpdr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zazyvewn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3scxbdfoj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cgcotgof.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dftcrwdz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3stfblhuz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3inlcgrnz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ontvcwto.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bsjtxuxw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kbqyowuc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tlbxjlah.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tqimqwmx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3uiwmuleg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ggcamrgp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wleeqxwz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzuptahf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wnlhlryw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mzsahmme.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrnvryqf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lbcrofba.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kzbtdkrl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oabzdzzf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kpdjgkui.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3aeayucqh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uobnwwqj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nuoefwwe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwnmazu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gesamjxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kcbnazmb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjgutrd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfyrigkw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hnwkvupv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nfvjjfof.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jokbzpik.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vavpzllo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ytswgykv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mwbotjxq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vnjzvuln.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bzepskrl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lxiuzxxc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3olypxgmp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ererfdzd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3eydggxrj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tqywfigh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xlungoyl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cvtrxbvc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hjgzfkux.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vkkbcpgf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vmtohsck.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dfblreek.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3axswmlyb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqvqskxm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qzuktnlc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bqmopnsp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gkmlyuph.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hpimdlda.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qczjtqko.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ugfrvgvm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nfmhpanr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3varoxedu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qdsssoxn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gdcbvbpt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nvhpvbrg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3awazmaak.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3txgokbml.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sydxsmog.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pfokbrnq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sznvnplo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jybpqzbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dztvrwxz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3necrguct.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yeariejq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3holsevwk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ahhmyjwe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vnpxuvyu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jjmpijql.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dydzwcje.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amtqehjh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cghahieq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xlxvlplx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oszerusl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cfbktmzv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsecjndf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymkevinf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vhvskoee.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3crnstzfi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jqzqmirn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3eyzdsspa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pavkvbuw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vbnewreu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nhvpgyuz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jflvppch.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3flgjvolf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qszeynys.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jlywaqas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpwfufjo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rdmggeqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihsjmoim.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jvcnkqky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vrllqzmv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjzdcxdl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pcwsyvsc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xtvgfxle.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wbovuicb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3yswgduie.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzmnkjv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xyugfmap.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3avhwzqed.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gmxhsmee.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dzajpikq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rwaspigw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wmjcdvzl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yqsdmcmq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qjznpfiz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hfkqvwsg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ovxkmuow.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3iganogoj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xgncruko.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ojesshpj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vaocgmlm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gqyhbzcr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ilphftcd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bhkarvyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tamlyduw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yzpczopo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pdbnpsoq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wciwfhvf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xinfyfou.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylofyjjq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nvtghntp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jydhyqkg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hmfmdppt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ddafjrdb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3szgcqrxw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hpmaseoe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jbotdddc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qbzwdhdf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xtnvuahp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3frpbehhe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ajqidpig.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rcdzltlf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pvsgaqui.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnxisrar.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tfxjbias.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fkakbqoo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3sertgodh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3elesthka.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3frmfkwuu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cieexkdn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jqywvvsl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ifbdvboz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrczkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fekanxra.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mgnhqwlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvkmkejv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3waslwttd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dlhwezdh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3weuuhvuy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uukuxgaf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nyjyfsmy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnswhdhb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3emgxzjth.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ndhtwyqt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rvxpoesi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mtirjtqc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rfjmudvn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vryzsijh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3waitecnq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gcjpvyhh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cgmxdqui.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hrtomxce.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ipsgerhz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3munmlspq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3gclscazu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3gvhyuklo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3aimpjtbm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ziootqbs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zpticdve.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fkwaihkk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dkupyjxp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cktodvti.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bqzziqac.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dewqjkcn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pwqlakux.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xmfvvaai.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3arqlbpik.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jwvdddaa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hfjhwdpi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwjgbra.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vzyehgyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3emzhknyx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3btycqawh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3acozyvcu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xzlheszq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lkvukxja.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3excmogmq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pqasbtmr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnxtoluu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lcycrkbd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wpodxpgj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xtcpwjht.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijrawjjo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cigiedfb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nilpfoxw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efcbhrqp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmzggtnp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xquocetf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rznwgfth.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ekjvzmvn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ffiefevw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3neqnscaq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bafbtkkt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gpzjqjld.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wzqmcimi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lcwjfdde.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mkveowxg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bjvfglig.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3uoceqahn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3apwistil.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qehupzbd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fwldjzsx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qxarjqzz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ukawfzmk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gzrcuhqh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vkxmtcyf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ifrsojqg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3isrtkpqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdjkfoar.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xysuompm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwgnwnhh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nepxvnzh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mbpinexy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3glppzrck.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tsvosudn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jihcbtyw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3pinprhaf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hgtcogru.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xhjaoaat.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3abbomvbx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wihjnpoh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bzbrfxtw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xyeuandt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zwecsdxn.html

);
来源：http://www.52xcode.cn/Article/details/gt3xfywlfqw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dvcdmcvs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wyziadsv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aiaprlzr.html


<!-- 参考信息 -->