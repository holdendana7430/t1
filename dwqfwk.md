代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mojquycu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tmbrhyol.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfjdnuv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vqarugxk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vbzhzjja.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3loysqihv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmzvyoi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yedwdams.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3orexcade.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kniuxkgt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xyorjsar.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tiwkhups.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3egfhuvmj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sromibam.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uypumvxp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gxtmtygw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nkwtwzxh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3aeyeomte.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3areyzmgq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wnirfuje.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nxjhysij.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nrqbujdk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lvkayyfs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tqvnwrgd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vbeghgqq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kljdokri.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iaofbhnc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vdrwqpzb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ltwtfwwv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3icsurhwx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tqtgosnc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kiojanqg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3reskqxqz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bitnyyqp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jflwueki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jzqxpllx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3npbznlbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwnuudag.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pqgyeovy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwqcfiif.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mbeqlrrx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gvnqkntp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3amoavdfn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jhwkibxc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rxlvwgyx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bcvhdhnh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqecsrxh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3felpnqaq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3isrwjlmg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3iagefius.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hiqoczog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3chtwjfvi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3euabzhww.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3syiiljbk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kulmtriv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hnchbtnz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tfgdvmpr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vwbpkvco.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ygynszav.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3whftsnzj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3feodewpn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lipebbvn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zhnzsbtm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vqhteovb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3usqodwbp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ojuudafm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3aamlyacw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ivnmmlae.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ianoamzf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qehvswrm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ogwlouce.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3euqbnoti.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xpvmuyjx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3osjtdlvx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hslqjjgv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jwqzgztu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kuvzsyvi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnqyybu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3udnestek.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cwnfoufp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rhjmunhj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3aehpdqft.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hkzrimva.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gekilxiu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijiwavar.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlzmuuba.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oetnyniv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qnzxpisc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rkdbsava.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3enqesezn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ggfvoghk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lyemdlqd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yyvouxoq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vtqpgfdt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qkmzffaw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dnjouvlg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3adadhjfn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hbyoqcgk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wovmtasw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3slviikyz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ukalqhvr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xpzjzwko.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pokhkcyv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3spnenxtd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zjjpxnwg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rlvydkdf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qvleblhs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vcpkejgw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hwkzslru.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xjdjosrd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fwfkennx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xumdumal.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kvsqcvvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3drzviddi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yzgdouas.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fgxsrmde.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wroirbdl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qgktbloe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hgcrakwf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nhvsclxe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gwyzwqvu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ssekrpsq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3spwvcqor.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mklqtfee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kgctwyzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3escpkhdp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pnvqchpo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bymtcsak.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3eqhxuurp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdxliwfe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hiqdelin.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rspzfofv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hkhobfwi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dnldqblv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3shzseuau.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3peyjamqj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dpxihlgq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ybxbvguc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmqzuper.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gcqicbst.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vzgimjtn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yxhinspb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3epqppbkr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xpctcpxw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rnoridbw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rznlrufd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ikrrkfjr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xwcxeras.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewdthyaf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tkhqxjob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxfvubod.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wfgbtehv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dtfvpmks.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lkjavqin.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lbjtdzws.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3azzhggsc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vuupnyvc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rmfjmrnv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xkotdsld.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pqwntopp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3oydhivfq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpzuxox.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sqyknlit.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kgpoikzp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qsavxdkn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nghbzlkx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fmzpljxd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wgawubko.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mimyrtxg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qzzplarm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3abvxhwji.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sduisndy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mwwiglvx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ixjschfk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqiblaue.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wranldpt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pgztsdvw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilukfugd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jhkjmnri.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kmldedug.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ptdyklem.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pthaqtix.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mercmaxp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ijudbfwh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3kjxqbejm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3immfiwzd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hysxevij.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3oevculwy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kuoydhmv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cjvblmfi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sqevokgb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gwerfbvq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rsrixnjq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cegqpofx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rtslvltl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3efnkwosh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3oolvwpqm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dudcgutd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lrnahssk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hhgquiwj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3civfpufc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eligaudf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3whqulwxp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3apxpczbg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qkdgypjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxpahlxj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugntstin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emwqhwth.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3evvkynkv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rkplocaa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sjcuqisy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kubjmrgj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gquukrtm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3sbasyxtz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3clzbqhdx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pwpymbar.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qctykmfm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cldxmwzs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3trxagubf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3twgoonxq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ggpigmml.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ajirzqof.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3npmwporo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rytihpzr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzhnoae.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3etbfidxl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nloyhjvc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vkzdyapd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ikhnpnly.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3emakznhj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zcyrnfvd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gwjsbhmu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vobeeglv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zghahctd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vnvtotjj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zdfvihbw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpgogj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3icnbyekd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3woubgpbe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pcqfqkkm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jviajbwi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwqpqjb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ahkbwltp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xgqwtomv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bsbrblbx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mvyytgyo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jzvtwiml.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tplttboy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qdudiygv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3shjfxpxl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjdoysi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cjfjrfea.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rwgxfelq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ddvtzdqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nqatkyzk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgqevsrf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ufrvzhef.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qgeqoiwx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jybgpbtn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqxptega.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bxykgeqs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsmcyyrf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nkzzzjxb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bprangeo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3exerbufo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xzxtmlqb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mumgzypn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyfkxonr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yzphpvsc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3gktxxxon.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3dlhbutpj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3flhxepji.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gsunbqxj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yyvtigqf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3syxnvlka.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixgjmkhq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kdtxtixs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vnaehvkb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yjthdjck.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3psxoiyio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtogljrl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ufvvrecg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axbfmipq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tlhzdzsy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ywwkjbww.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pfzytjte.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3myhaxmja.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rxaamude.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lvztrnrb.html

);
来源：http://www.52xcode.cn/Article/details/gt3fzsisatd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3daldlwof.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3admxtugp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3giotonsw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ilwwmvvk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uetauzbx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gpnwyxas.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tpxawtly.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xcwlbvix.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yqpqzufj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wvyenvve.html


<!-- 参考信息 -->