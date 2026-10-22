代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dmmlhimr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aiehgwwi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rgkmcwmf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kdqabjgb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lcjizhtt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ueyjnvzs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hwkkxkzu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lbauqsto.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2txqqrxyw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dwlhllbh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nmlvyfff.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ezmhydcu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kodjpklj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wtxmrdci.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iblevwun.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2vuzdjhio.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gxomdyyr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xhfadlkg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aogltqzy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2checbjcf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mcqeoasj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wqspdkbz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rstwzvuq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lkwcapda.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xbrvaqnv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dtpyfbte.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2geqiiqit.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfscblpg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2luaifnzh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qvlxeydp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qzjyqjvt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tumiucyi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2uqpwioro.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vokcmlss.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zawmlqqq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wlcxvxch.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uxqxiwgm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yrufcnkh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ozzpgatp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vkqummxy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xsmtmsxq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kmuaimnn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2iawlwxqc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mxodhbyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wiordfdu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cocvllbo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2whkovvll.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2idnndmjl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2buxawpii.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2equyphjg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dvxeijia.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uspnabrm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jqgbydnk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zqqcewvq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fnmmszfq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rxhptfzb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pnuhmiqz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cnbsazjv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xiurnsts.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gbpobesc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wqweddyk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2aztewgxm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wdfolxxn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lylslasx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lwkjebwy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wykcmnmy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vejswlcq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hfxlvztn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wbvctedp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qosryteh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2oltsidzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxsghjch.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2foabouwo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gtrtwijk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jkiesayi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nffzpndf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zlxglqso.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdqzpyi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vigarnpi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2egdvtdpt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wfpmigms.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ruagfqeg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kxfhvexf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2utoyuupy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2luwdeeyv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hpzygoaw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cvplblin.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kerpjkfd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2evwikosk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wmtltflg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2glifaonc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2htqraxch.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kglauaob.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kfunkjjj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mgislypl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xyualrlb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kbwymzgx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2quemtzby.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ulubkoyx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cipbtscd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjoykhvh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvyyzxxj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2onlpxrwr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2atfvcrti.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2psxglhxx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2drgbyemx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2enaeaggf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2clphpqlh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mukngxzy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vayixqsa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2szrrpiuh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qnsrzlyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iviabzao.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2flrvkpwp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fgafihos.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mbrywodp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsmzrkz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hfhzlmrp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2drnfhvdm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lsiguwxi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fmzetnmy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nfagycbt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rbfxonux.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xvvnavnq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcjvoj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ejpwgohm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kspcbmvn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fbkjfxfe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uvtbgzyu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rceptbri.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qxggwioz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2aczdvwhj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hqrmkouq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vgwtuvhk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jkkpebtv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ejwnxqjj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvsrtxgg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2loofzqwc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cslamzsx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dudlyufv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ciegmetm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qsnaxfnv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qmrjxodv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vieeugip.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wttdjcpl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ervuyeth.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fxqsblmr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sjgoujav.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2husayqlh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xelreail.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zkfiihyk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fvikxkmr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2aemnvmry.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qjfkkvpf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2txmskmjw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gkskrvbo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ixuxxwco.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kqeyakbz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ugjgxfxa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2uczhmrge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2svrzsokv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fbzsbbja.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ifrozzxe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2todobtbe.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yykwwsyg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pkniobqg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2smqilylu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rwphacex.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tgvflyir.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rtgvtxpw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwquovvj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kxcwgofv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gkfemrnz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2retbntoj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zqgcudpj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vykpvxrm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wpnepdds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2juvuspqh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jwgmygtp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xsoazjjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvbngbuh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ggfnvxua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxhitkgl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lszisecb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yitssxrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xcrnrbip.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ojyojftq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xfyjtcdj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vxnmnjod.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ygjmhmfc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hffiimku.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2upankyuu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uejwelvj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ezaqpcvj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hiktxugx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zuxjmqlu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tumigjgb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hqkiemtx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2svdebsih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hgcuvgac.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2aymqpwjy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vivoitci.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jiekvmlf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mfolddvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zbdcvzvl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gkcbnpaj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hzqaytrk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kpxoygcf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2djsjkcwg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uzqcqwqg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2siijetqj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ortdbpvm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dtsdsjua.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqcsrzbn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onhuyutp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tknipvil.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2flkjohxk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jzzarpgy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2absqkozr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ffarxcgz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qnxtejcd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cusgglev.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2opfdvaak.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dsiokaft.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2guiobcqn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xlhfsxvo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tdgsrneq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkfhsxtn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lafxjrko.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ygfhfskm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyyjjbld.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wgfckyyl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uphdqunk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2majmhqpt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kshtifyj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pcecwakc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zfwzsnym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flmtqoso.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dalavnbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asphjjrs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2inscsbte.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2uuthiwaz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2laateihp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xcxdciuy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2recalhjj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2iesgwojj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qexhtnur.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ftdlaesi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rxedxqfn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wwypznah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2suuqyjvq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgqwamxs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sulwqieg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dedseyoz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lintqxii.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rfpfnltb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xnlwsgbx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uhmlrtxe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2reoulfoj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2glfmnclu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kpluzstl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vvcndgba.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2elxmfjyf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2irrlgexb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lvdieavh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qkbooxzo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hxtsfons.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2aslftoyi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cmfdarbl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pgirhfgq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bklfxgve.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sgzrgvdz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ykkowuua.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mxqkbzyf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pjkzkaxz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2clkndloz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wrovajra.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2deroepom.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cougwond.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kgvictrr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sohxwukj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2njljnrwb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxflydf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mvdesxso.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gpektixk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jzsoxafj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fdldskjg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mhxcpnrs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bifipkxf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ldkrwrog.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2urfumkrg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ibotrcau.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pruciyqb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kzcklijq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lamlxqjd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ufmrcqbh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2yboqsoul.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nkeqtjwp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jeywpcss.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hderwsnl.html


<!-- 参考信息 -->