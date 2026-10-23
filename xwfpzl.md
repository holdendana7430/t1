代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hidsioqu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qfbnpant.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xjniulgm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3yttgokdr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vrrzkuhb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3sdutngdr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpusmsmc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kghsmhfj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3acxjdkja.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aeaiysmo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzkijqdo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spxaotzm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qkmjfugk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ifnhsaeo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ujpiplii.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bovnljwv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sbkemkzl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3quolymdg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lxmxpjvi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nefblezz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zozjsqbh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3plaryeso.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eqdccxje.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lreydasz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fozqzlbw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sxzviety.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wyohpiiv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uslfyllm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ezhzcjvd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xceshors.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jodzlpfz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3edskqiai.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jzudmfje.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ufwvrnzs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nhycjacc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oyfbwzan.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dbcwyntu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3iceeqrjj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jecwfhdd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rtmkaqfu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3geodktul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fympkiey.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wngcnibv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkfmajmi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dpkwhbtc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zihhazpq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ovagjcgo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ugxoehvi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nusdidfy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbgzsvc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpygnynz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nulmmjyr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwwihbw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mddloaeq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kihkyxlk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nuojvyvg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ainwlzox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxchjys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fhixgjce.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3myriomwo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dxtrsqid.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jzlomtor.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rkvmciyy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kylvoqhu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jpbezywc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pcygmoeb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ddidedjn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3anzozdyr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sdydsnhi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ztmxypze.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3niwpwfok.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yzzhspmw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nbazcdqr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3icxenzpm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bitvissv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iedzbgdx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3emvpabvt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3berglcyd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqthvywf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lxctzepr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vqkeignp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xizgaiyq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wevmcunf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldgeowwm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpkeouls.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lwrirhcq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3aobhapce.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3odzzpopw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qmfspecd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pyqimuja.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vyvhfooj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vwmutgoi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kybusoag.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tdgjrhcv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ynbodpyc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrzqkzen.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wsxapifh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bqnhvhtn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jphgqzsc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3maoinwhk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mxyunvyw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpanpvt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iieddvfe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nmuzngdg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lnlueyvj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fossjkan.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vwbajpmq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pgyztkqr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qatjdxsj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wbqlnped.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ynziupcn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hqsuiaob.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rktyouai.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ryeofbfy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3uzvqbfef.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ufdhliud.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3juslqogb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlrvsuiv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qrabsmod.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yvkwefdy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hlaorhrv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ojtmcsjc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3flnppznj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sezkmnry.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yacmwscb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wyrfwnvt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uydyggyq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wmryaeml.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3clmzdoxj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mdertrkv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3smwebywh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3djwahkdo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vwkoqqaw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fsbsbslo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3yextzndr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xenszxbx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dlraghpr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bbwfasqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3njoalxqq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tbgdtahd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jwjcrjpl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3eogownqe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yiaemsot.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3eczcwztk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ghgugnvl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jblnfrfh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ztrohklz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mmhbzzbd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qgkfbhyl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mukrnkmi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkirrqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jhlzljeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egrzluyf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ctnmwguu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqesxhrh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gqmbpyzu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3alrlwiri.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3sclbdhjm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zgabjays.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pthktznd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wkbcvykl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3idnmljiz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3baivdvtn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3brkgpkfb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vhweddij.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxifpbs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qmcaojsz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xjxvbzpf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dqumgdrd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ozewrdvc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yzeywbow.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mgjlnizr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vlxpkosq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ksfpffka.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qaodrkpx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zodokxlw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3crmivvwa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ssjqbigh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3inalrdky.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xglsawcc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qyeawzrd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdqyxkvr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xdznguqh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjzrevs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zhltucfm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tquhepey.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abfioerv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3sxkatmuq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3siukljqz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3iltenilv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nvgiinby.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jrgjpjco.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ahptkqqx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lkeutifc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hujvjuom.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fmrvvkzw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cbztfzkm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lugpkbbm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nczodqzb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bqxhhbqm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rddcbkqp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rhfpaajv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wexwjzho.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lwmgwqhc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vpwmjduj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fehaetfz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3liyydppp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xquiddou.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qntsxyxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnsrkhmt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrtoxbqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izaszuqo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qommpuzm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3blniobhv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ozzspsrh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3alitigrl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iftquwyg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3merunxtr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lqksfkyc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ylxshyem.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vekpctlc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3twccrhay.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zodttgwm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecjrxtxi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yccurdrj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tqyhjkfo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xananddq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rjgvsfth.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvthqmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3aivgdmsa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3igdwzfbp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3omrolrbv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ilayqevp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bwdlvnrk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xxefotts.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mueppzqs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cqotqrat.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lvyyyizn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nocnbkwz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3czffylda.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mruyfduu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ggskgrej.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tqtgciqt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vlrywujr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uipdxmnq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mznsgftr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gojcmotm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rrialhkz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qjtufbid.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bbgfahhq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3faaukpwr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wjylsnta.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqubxuhf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3exoxmlvu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qwsfdekn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3chlbezxu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3auleztli.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3trzmevuc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qzvmxylp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xmjkuotm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3iyxfhhbw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ehbuuyha.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqxmmukj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nnhbwmem.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xvfbiwcy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcmpuahk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qrxoujvk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qlbebetr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruixiihh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wchqcbkr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nfwmimij.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qswbejzi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fobjfmzb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3naulzoqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ffhknrys.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kpyskipj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cshinlsu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ndgbqsbk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zmuviicc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqcfvzd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uvegyayi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3flbvvsls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dsxebuds.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qkgatbdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3socbwnon.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3flxlcthv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihvhmxdi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3apzmilde.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tnvjgnrh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zyojyzgd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kkxgocgy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cqjnkfjc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ikgjrxkn.html

);
来源：http://www.52xcode.cn/Article/details/gt3cqilkdpc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tvwuuxzr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zvgqiggy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3etnnaufu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dgpihbiw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gpbzxgum.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vpdmjmho.html


<!-- 参考信息 -->