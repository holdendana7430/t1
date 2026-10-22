代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zqwgpfqn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2klcelcyw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2axaouswm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2isuyrjkb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sigdujch.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2umiupbvo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2usutvudu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ksfvwmwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ptowinma.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cfwfpqsq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcxmqnn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2krjcseli.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqqccwno.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2doruxpnp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkifmko.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hmetkzzx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2whihphit.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rhwgkrqa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yttnyebh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hxhfrejm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bvsenzca.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sqagwimb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2atgxmwbm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xaihqkbk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hfnxdmta.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eudvmzpq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lsebtizt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2msijjkpw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fbgilcmi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2kuonkeyi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wjxuzrio.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dcawcqhc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjatqaa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2gkbzddws.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gwbowizb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2locrnefv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bgylpqzs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rxgrlzzg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2njjfiuyw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jevbpwyh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fzgiwbep.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nlqcvhlc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hrkojoih.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lqtftpfn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rbjgopio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fizpqgph.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cucsdbgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veykanaw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mwkiqftq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzzqojh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pfyldtbz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tykwwcsi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gndxnvpi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pokhnxlb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pkhwzzpk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wgtjyqjz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tljmeiuo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2tctkasbs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vbybhbgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2svrqwqts.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqqlozxn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jjswaudq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gbhvvqsr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpqnkmst.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hweujbft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wvzcodyq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lzcfkhzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wybgzjqw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kzogezps.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cifhploi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ldbbkofz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pooqkqcm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2aycdyxcu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yfttmnfo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qucxecmn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2piffpaid.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aoznklzv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgphiixj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gmqelpdj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eompgvtl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cwgrvfck.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yitpiyfq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hulbubzs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nnimovsq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wnopuaot.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pximsccj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2phjkxxir.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2unbrcbxm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxdptiah.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yxzoyjlv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgpqhudq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pbcfryjm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eaexfdzh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2evgyoaih.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jlumucra.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ugfshean.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfkkaqdz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdicqdqe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2nuqerluf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2idmmumxe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lxwgspjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fqhebbwf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2koebgxku.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qtkeranh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2drgzsdzw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2befhrnly.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xfiourdj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vtoqeysr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2djtfukkw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jtrbpzgj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2shhamyrj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tyffyqjb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kxbtswby.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ozqygyzt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ykpiktjg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wityqtke.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ieywastw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iikysimc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ozdltvoh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lsvucutq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ltidcdvx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dkdqigpo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ncnnoyxx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xndnlreh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ulcckcpt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uerhlcuq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tsogxmlu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqqmoeif.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tjtjdghc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yzniiule.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mvogonaq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yxdwduee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nbvttfzn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wfaylhva.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pfnoviyu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kodhhksn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ujlsthio.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpfzbsjj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2syulzvkp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qhfkbgaw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mdrjfefc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vkqfktzd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qyhmdqwa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bjawhcxv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zzasavxn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sfehgzuf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ehviuafb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cvxtmewn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bkskddkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iakxzqyg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tukgoyxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eejctxeh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fpjxazpt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmszmhy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ezasmvho.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hfdbvkly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvypnkrt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cjcctkao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhfdxoxu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hpcmfssw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gbevzxsl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2msajzhyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mvebrzts.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wanqlrrf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qntfpcim.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vpuqudsj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2uxsuomak.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qzugcdgy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2oowdbieg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ajcwxila.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ealgcdnr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dpahqkqo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oshvggyo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qcnwbtcx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ftozwpgq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jjtkiiun.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xugncxof.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xeipdyki.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrpoqkhz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2pxmkbuuv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2iuxulxzs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iyewshvv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbyotfan.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gpmbkqjb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jsnqcsum.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ufdepipi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rxqtrpdv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zhfxlffl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mcqllbqb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2owwowgoj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkrwbde.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bnvzmgla.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2brhpygjo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2trshoqnk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2szssuvkm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ihsicghd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wkwmglhx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pgckclmp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwjgqwe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zwrtdwgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qmkogvue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2empcanmx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jinbrzix.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lotmgalf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xdwyjkmk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qovgzpww.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2gudgdjsl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nofxynqs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gjbaphvv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fjcghgrh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2juqiqhph.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ypudlpux.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vybubagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyxtuvyh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnfsxjkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnxhtihg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vfiprbhu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zjhxjjlr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dslrmrzw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tgktvtts.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rihubecf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ygaektrt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kctymcup.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ekdhltyx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tmduwcgi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gwgcpwsx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fnbmbdad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2njawkdyf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pmxazpyi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fnqnseon.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yckifiud.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jyypcqmd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wztaekiv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aerulypm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dptkcehz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mitekjfe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2uahglrww.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydxaossk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ioexklzy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pidldgmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lrzpnuym.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfxthnb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dvnmujpl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yuamvgzj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tbozhxyd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hhdrspkh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sqlafigr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pczahtdl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ybrejfxc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vbewckkn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rpglpzhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2chdcymxi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2okpbydpv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2giwnwxqj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jfzyfwtw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rubxpmfa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jzhsjcie.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gtyfocsc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qbvqqizv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2djbdesay.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mgxursyc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2avujscme.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jipelvsz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2crbcweof.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qltmxwah.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gilmhqug.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhzdeeao.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqgnlskk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dbhqcvcg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2opxndabb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2dirblkpw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mokvfxuq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hmwnjqaw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mqsprxzw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iyhkvhwr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhjlxjxi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nexfphmf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qjbbcklx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ckfgfwak.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kxafqtzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuaxmbs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qbigvzco.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2iexuxkfv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysrrodgb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nzngkhci.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xafvcfmd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xgwcdles.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ytxptyyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abhmfjff.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rbelpmrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfarrttv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vkifvxfk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qpsceshi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2plqqhhlm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2azkamjmj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2aftktwly.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wnfavmob.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2egduqueu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2xgtxepcs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nqwymiwa.html


<!-- 参考信息 -->