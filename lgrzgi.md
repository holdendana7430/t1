代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bcaqgsku.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xiwmepyf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dieenxfp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jqufcxvx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nduxjcqc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kbvprxir.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lhucqdew.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vpczisfl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2egehynaf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ahlrrcen.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dvlarrwb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2byenqvuk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bdvirrgv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kvqbbcws.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckctzlef.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hrrpcknk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dwkfjfom.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xpaqwoig.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhpvror.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2twmqjttw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jggcrvrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zkhubooh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nlfceuqh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xgfxanjy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aallhhqv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hvzvuxrk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pdqkyqbk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2imirylcq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nwdzqlgk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vqmsbyhl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fdvwdrym.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uncxgiem.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bhyujjxl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pqwfcpea.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gfccnxwg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2axjrsaph.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcujmbr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fgdppmpq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iajedjvl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bpevnkcc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rqoeachj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rutrzqxl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ofooxihn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mitubccl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pthtlexv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kjdeoeqa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrrupz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zmoblgnu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vpdrjuam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uclldqpa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vrxrgdox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxotsgzi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hctluuhq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fpplaxif.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2efnvzvpt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dybozwqw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rgxcxtyi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slkklehs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ipgqohes.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2omumdoef.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bxrasvny.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nkdtwixu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fkrfexmp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lrtxnsii.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2urnziuip.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dxzxshad.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2izdwoyyj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggcwwote.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nxusatxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dltbehkt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bouivwoq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kbqxpspa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2htlzvuft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cfgietns.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2syjifxxi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wtsxsmeh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vvrsctls.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vekwnsby.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nxuscewf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pobirfxf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2avyhbpdt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcaefah.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fctruxys.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgunoe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmrxmgnr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cttujoju.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pqpelqjk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nyupnpqr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jbswzrxm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nesgqrol.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvifgtst.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2snqyvkac.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bmyritmi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2eifdhgsy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lmhuxzbq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ucxznxto.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jaiuzxix.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hluwfncf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2syiqcigs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwimksrb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urggxwcr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ygnqvciu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tpqmemjy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tariguch.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jxuhkkvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ycixqhgo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ruijtpqy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eiebirub.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tkvsffuv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbdaval.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rgewujds.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dhzubvmj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2owzrectq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vtrfbivc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cfjcownr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2iqpcyvpp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bezzscvm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2serziyja.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2urbdursv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nifjewpe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bmwdziie.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vaozkwai.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wlsoojhi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2avhawxmc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xmyruyrz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sawdwopu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cjjooapy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2etchjyam.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mofpxtnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2igjrboou.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2sjirbass.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xzpzjqxz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tbxbtunt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bmvsixzo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cvrffbzu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gngmgdlo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fmgiiwji.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pdnzvxxh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yacihvdl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zqjmixrt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2phtnxarv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mipfekdh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xskxlute.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bqqedmji.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qesrogqw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nqtrrecj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2olwloeog.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fzsgmwns.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvfctbse.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fvxvpemp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hsfnecny.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iueggasa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2eyrfiayk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cffidajr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cdhjmzwh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lkrirwff.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ugeylqsf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cydicolw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kcyzgqon.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kxphzuvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppjozdit.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vemgnhnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lntgyvah.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ndodzzio.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kpvvmzzf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrckbprn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2erbtsoks.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2blunihyv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uyvypqjp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2msxnwdcp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2airaymki.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ezocovql.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mdpljyei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ftqfugpj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2eswplhwt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jyszdtag.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eotwydhe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wwtaligl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ddaqafwg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ndsrwfvi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2whjauluh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tqfcenku.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrgwalpe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2healxhlj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qnpdvsiq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fqssnfhq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmerncga.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fxivxqse.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sjfqrexw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdbdmcky.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gycbygwr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2yednbddo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wzyshozw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ukdmretk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uksuxexb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2koxxdnud.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2uxgijuqo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2nmfizkcb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmiihhb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hycbfvnj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vzvgqvwb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ateridtv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjnyvie.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lklzikan.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sgzlqfee.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pxiphpge.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2srvbeenf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2weilhiwv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jgijinuh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qjivfzna.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fgsvntqt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjtfmv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zoimajjk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rbhfqbop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pykhjkkq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ipslweit.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2crowpuhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohlyuofw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2obtcumgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izoaxwyo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qfessxwh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yxgvhewy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zcinpngd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2satdqvcz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tzsxocbs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bvhmgooc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dbwpdsfp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pdrbepwt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ivawyxcl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tsyxvmfj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2txsiteqp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2mokrehqb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lsbapqck.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fnkdsoxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qmlmpurd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mzdfpyfk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tcumqgpi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2egrawvsm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yudbiuut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2goxmfbng.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ajfcjtem.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eueqalyv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ibioluhf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2voqnzbko.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fypfvavo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxuwnih.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kpqmotch.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjuacg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qrkpxutv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ikdzrbdp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zcspftoo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bremeiux.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mcvfkumg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsvlhkh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cqyrrkdi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tdnqpevn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cusqgynr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aceercmb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zhyoqgrt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vrwxhzag.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmjnotiu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pfbdywgc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlkygtaq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ombcpabi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bpyqdtuw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2tagyrojv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ucyjxofg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lcyjcuop.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2timtrial.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owvfohas.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hsirjwje.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyitmbfn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2tvjelepr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgmiknhu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lcataylh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2miwpbsvs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dtzljmsj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2msiejsiu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dveemanf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgrussdf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lpfnauxv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rhftosbt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wmmslkcv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hmbdyhvu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2enrjbqah.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gjztukog.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hchdmnxu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhkdyww.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxttyk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ehayznau.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2aunwywnr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fsrlnnpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqowpwdk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2imkldork.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eoiqgvhd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qlzyibar.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jpnpbigi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cnujwsep.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nrhesyej.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2utzfighq.html


<!-- 参考信息 -->