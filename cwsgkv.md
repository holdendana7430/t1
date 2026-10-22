代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jufacubc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xscoszoy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jlhlmaaf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zqggwrsk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zlvrxrbq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2eujzpkpb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tslhmxic.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nsitqakf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2kzbkntgb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tsevupgg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2synszotr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxzzqfn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2obqxmckv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jejegoys.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qetvqcgk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vlvirjle.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hacrhupl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tbmovibf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjthbxe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vfrlrlla.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jidhjpfv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zftznbap.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvwtobv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nenipnnm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2butybfuz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2teghddci.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2afajydlb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hpwfqvgl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mmaehepo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jmohsrzo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gjxjktpr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dzwilniv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yhmuuict.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bfugbhpr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zcyrxlea.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hfygxvts.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2evlbuuks.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2trfmkkan.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2psdpkifq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pfzbptnz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mzdplpfh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cxxfbgkz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2yahddsev.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fbtgjeku.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bvbzmbrb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ykzcbpip.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ituamhog.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2grktuoxu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vwmydipk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2exqnutyz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ekoxltuu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xfkcndqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lzwgwwjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxoffkwu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xgqxenwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2titrdrfp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ifxfcgyz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pchbblsl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pwkcncyt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fksyxbxj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yxsqilxh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ijmwigdo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zxmwqhdx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hynzbjwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wppeyvhx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rjguojlm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2axtfywqh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qskdknuo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qdudfxcc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uflvxrhy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2emdmxzdf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2enasjtvv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eobjdbgj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2sbpqyaee.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lnxpxsvz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2prybonbw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2opgwzmuv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bjawnkqz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ktfnpgue.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hlkftlif.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2shgyaofk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fshcwiqk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kvjjvvkv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2repchvti.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcsjbbr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zzbpiqic.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ssstywbl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mysfejqx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hkcjalke.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pcujfyee.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gfjmlcnk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aglsoium.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2odppxdvn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ufkllsmq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2stunjfai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jswowzbp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrunaodo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bojguhgk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fiznjpuu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2klzmtlwj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gelnmzug.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pbuckjih.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2duefwuac.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2anyiepue.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eqogazac.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lypcynny.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dakeblzj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iyrlgkuw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2obitycnx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ildqqvmt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2enxwbior.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xucnycpn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pkymkxgw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2djwbnwdt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mjyyudej.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hwpkmfrk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dpvqwagq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2iylamigm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2acwjlecd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gctnvrun.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwqvszvp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zgdxcezz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wfcsfeud.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bbcarowt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rifmvsjs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phgjrcdr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2thyupnwn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2phvwtezc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlwqmase.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmqltmng.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rhppihbi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmqatogu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tayqukii.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgunfhpd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rdqyiywt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhrreehr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pqwmwvek.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jcacmxbf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2oipprbzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvhdjckk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aqhrpsau.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2umrwangd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjpxovkc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kchyheue.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2elwdxmxj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzmgkyra.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2amntjxgj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ojbytcie.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrqizfuo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pmnbkwsm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wulvsthr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ydjjdkwy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tbxrnsnl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ajkesbsx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ayqrymoi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fagzbken.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2amwgyght.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xqlehxrd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pughcuii.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yptpbdwe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nvhpgsgy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yuirywjx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jcvrknnk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tcbczmse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iallnhzn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uaurelpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcfinhyf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2snislhbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vsnskecg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfimtcxb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2levnomhi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2leqsfvfj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rzdefvwr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hwmkzitw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qozfoeda.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hdgdiihi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uxahpkjj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wbpdvwwz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2aavykdju.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ylhntnai.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bflseptx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2savysbwh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ttfyribj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2flckzxol.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zcneebkd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ollibmvp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wgevhxcy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vkngldrw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2bwgaphxd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ftjnlrzo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsgzvoxz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ssdbezth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hrgvmlge.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtlnxny.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qwnawxbb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mfawdhwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bpfpjzyp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlgqlwhl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bimphlwy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2etzyfnmv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fzdvmyzl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2njwinrjk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehfgusxu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cmoglgap.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ovcycdyl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zadsoiwn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qpscjpol.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcajxoj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2khmvkyhc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qkumlwns.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vdqnvqeu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sywqlqth.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vjziwqdt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ibwenuwn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jneoxpzo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pgoccdvw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vjmlbpdx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xfxarier.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2etoumrll.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2dqetnyvb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qawkqjbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krljwdmd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jeeguefd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfiyyjfw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ascxdsbg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ktlmiiru.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2drzhxstf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ptvdxxpj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2irxbahuf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lorxkhcm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ujrlkvtr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fkapqkbv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qgjwvxph.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zofzeprv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nklrlmib.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vznitnjh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fvpzubns.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ekzisbzh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ceejnxqv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wlrmqhao.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wlotnvmc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pbxyusva.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yrsgnjty.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yagccgta.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ygxvfshz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hytwixvw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fhhszmlv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zadzkegm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rusvrlaq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tfswvnvn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wcjavdiw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uboerkyd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rszhwtvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ydnetxmi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mnlkzwtg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wyckrguk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gfbphhkf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2wyxvxffq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hyfnvhid.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xguzdpjj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uwnlszqd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nwkqbmgz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gydymdmz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ywygetos.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xzudoshs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vknhzqpb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ynchievk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dxlppmfe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2dwjaketx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eorkeucy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wtjckprk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yyjygftv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rdjhqjvy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bestosdu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehemoypx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwiondfu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nybpbozh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeuvqekw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ixobxfsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2cipphgtw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2knnhyewj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fnzottyu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2byzdhgad.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2nytoiade.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vipmylqx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ppowzltc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2akccvssl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kypmowvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rrhtxzex.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wqkgmaky.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lhsctwev.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yyrxjomk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2moodjlxg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mmnrxtag.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qrkgahkl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2orurfbej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkykctuq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kxfjjmwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llyotpuo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hnxihypk.html


<!-- 参考信息 -->