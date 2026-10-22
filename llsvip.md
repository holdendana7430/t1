代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rhkcjujq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2udhbdcig.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fhipxaay.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kcyokghi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2prymitxt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mlvgfgog.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vxonurgt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yekonbsk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wxnwexfk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2czbfwqgt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evlbvckw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzujdtyb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2edszocjf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pouhysjz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvdudrgv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fyeeqgpn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tlunpixq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2coygkjzp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2upupskui.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfuxkjvl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tduibkrj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2thntgmyv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wpxqlard.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kdfjsoqj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zrhbupxp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mfbhmfec.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2migtsrkx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tfzlmzsh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jfuanrxd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vqwkgdcj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bhborqne.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hwohxdaq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bkijxpwj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ghcbryqc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iaojpbba.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jymwzdjy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qqybgonr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sjqrtwrj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qunpfjjm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iicoisos.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xoydcbhm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dlxqzjln.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ampisplg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nfoijwbd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yspdkrcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2waixcshl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bnmbrxog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oskvfwcj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lnbjdrvt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swhyibur.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hxxkxtbz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdjjaqm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tzsziygi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2szundsmc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntfvotqq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2svhaaxoj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fksnvwjs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lrpbirav.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dkulmvqf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bqzfhzie.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jwdzumsr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wzyfogoc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ltlismah.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcnxsouq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jlzlmfvp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2yzhfnven.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2snaiyisr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wcdpnygt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2oroqtvtt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2znbhnimi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qbdcboqa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2uqmvvzws.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rnyghfhs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2opdygexg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2abjfmqht.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xssvplit.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mpfeqmyu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ehlmwrvk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnlfxyqs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yryhnpyq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ytizwfry.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gexeecce.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vtnfvjky.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kewbwesi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vddoadoe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nmzzrxui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hteckpuq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bbntnnha.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxtyxok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kxdzohrp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2phwtolcf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbmfsch.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vybfudsj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lzwwzrws.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jelbjxgh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lrouzjwe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tjwnxqjp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lwhzpcoy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2abzeftue.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cqqbkolo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2crtnwjtm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dyljnifg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ytibszjs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cmrsmorr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uiafrjau.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrnpaxd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tsagoajj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sozxhqsd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vdagthdq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2djtaekss.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hyvfhpyg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bmcdbmkd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssplhetk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sxvhkjbi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhkyecaj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sptegcuc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zyiqsimj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2stjaddma.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2midasmhe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjxwdn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mfdggbxv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rcvpxnwe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2prdikjrm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oewohyvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ljbloatl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zptruhgv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2eqaakios.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lasakvqd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xijyeedg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hpvtlece.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lbmunmul.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgwpcsde.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2apfrudlc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2valcrsdz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2snwumjia.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qqsextbp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bejynfxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyrligid.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2klvwrclf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2gjlklnos.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2naypxjrn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mkjehezh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jsxqywmh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yzzquicc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2flilikan.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2yvnonxmq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ubvhpgfu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ayzjueed.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yztydyxd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iatjtmns.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vzjbqpqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bpdcrehw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yxhzrnse.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tsrssawe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tqwjzgnb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nqtbwphr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icvxqjlb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ejqkxnhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqzdixwa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2raythpsj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lixboinu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cxitebhw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ppyxavzt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dzguoskr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vkpbsgzc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2diqcdcyt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yptgkxie.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ynnzohmr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2otqwekum.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2iayrgmkv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ewzvjtum.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gbandxwl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aleyvbft.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugztjxut.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2yocuvwas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hkcvsmjn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2haahhioz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2omfqiysr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssyjtabr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2izyejcrx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mgxszccs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2crgvglbf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbvjltsq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nodgmsju.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xsmtzeew.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aoufjmfz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ecnzhket.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2iwagkrah.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2eppgaqry.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2grzdwmps.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2loerspwv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jfcoqawb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2piarkptn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hfzcsjqw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxswbksq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xjrotxxx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rjvcwjyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bwxrkncc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ulspngkk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtmdyns.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2asnhkebq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ibypdfyg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eulmghsh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2swllwcvz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tzblclzu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xbxvuhae.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwbzaulw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2judketcx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tgxkbngk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gddkipxs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kxjgfdhp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2updanjcs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gcqgpofi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxgvqtvt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxjdxxzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijpvijud.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lxqgjehz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xcgdejzp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xhfcbakq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bhkxzhen.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gwusstpa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wvzaacnj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2inlclsgk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fwisqsed.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ewigwvdd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xixkvjwu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2luborndh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqzrbhaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cjvdyjpa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wdfroxap.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhoyrew.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yhxyzert.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2luvuacdf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xunomovv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dsashaxo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hcjhjfds.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tafgtecd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2whwivtmb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ihxxrxpj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iirqfvpq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nqxevefq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2uxagsxco.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bqglijhj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xppqtpxm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ssjcfupc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mysxrzys.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tnuzujzo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ztgenmxp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nwfbwdbb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gyvnzsuj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2drujqvrn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zxlaaese.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vmkvydjo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lqaktyem.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bgbehnrs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vqxebbrg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kqjovqzx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tlaxioak.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnivatw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hgouovss.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xzpxgizb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2iqblslrz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gwsnkklq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hxztjsvy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2iaqhglrr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwbyyvio.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpexenyh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mdjuazxd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uitknyke.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nfueqlfg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qqdfkyxp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gziezkvs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wupkqvhs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vkayxeil.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2idmayzpr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvvmlfj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2znznswua.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2sesrdunm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2pguhqsqy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cgugchex.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnvfjxy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2soowppgc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tossuowj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpkyksij.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hwjicdgg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2katarblh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zstxlkyt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bmvzfpai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdnnpoln.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ljhzcpnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxqbkbad.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2pucncley.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2sefsfgfc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yvlxnzph.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2riuafumx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2uztdwtqe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2yumonurd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ivsdftaf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2sjwakffb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zjbepzkz.html


<!-- 参考信息 -->