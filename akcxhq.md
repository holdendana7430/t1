代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjgafmfm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2juxnwjsc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tahzzbdl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ahkrdunp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mgmwhggx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2axhmxlpr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wukqyiur.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kaxuoxpb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dckrqlki.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jdsycbvs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bzlykddj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qaphokjw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rztfrosn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fjhpqpwq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zsykhnbx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kzcjupby.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yudjkmpo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qfcbvvkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2npvbttfz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yhsmiqmc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wjchahci.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yuotouxa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qvxkaeoh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2godenxvi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vyseqjfm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fmicocce.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jsgxvevv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2smiwucvt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2amarjovc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gblpwapz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zjkoklpi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2juynxmls.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oxddcpnc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cogysbdd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vipwvdmf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eesmriyr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hbnwjezj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqcgrul.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzswggti.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zdyrscxb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ebtrmtxn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2khlrcgmq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2olwakgtg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pxsselkw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uqqfeudw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vijfbvhn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dkdzztue.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tvhgihar.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rvwasjgf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mmhpfnur.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dvcjqttd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jadwlxde.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lyhzwoia.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qwhzfzgy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2desrezko.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yjdvwdph.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yhszwujq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xmbiacmo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uqrhuusl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cfzketmu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2aukdnurl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ivoujxcn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gkrntzri.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2azmqrgiw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aweuelhi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvhpdpy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bkhyabze.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2aqdfyvis.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qxebbjvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrebwjah.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2agfszrpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycpykbvd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zyrwzyyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vwxlllvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mjchabtc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rwaqkhxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cerdtmaf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwdkefpj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omauiqzk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jlwktknp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2izdhmxja.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gsgpgzpy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dhuzcqky.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tchndche.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uyuzqdkh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eeikkydk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kyweaeme.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gibqkdyb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2czufceyl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qahzrtpn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2akwmmysz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mfrquybz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wqhgpssr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2liargjfe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hzaxhzwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ploptcbs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mwpwgrxb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vhjnapfv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yczejhuh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wzuooawh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ryobdicu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nldfsaea.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xslsxmor.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pfnnljic.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcribkwe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mnetdnkv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wqrxyehz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2exvxzwof.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cxkfpzap.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbhbpsp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfiruxyz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2awwlkyeg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eecbtczg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wsfcwvjs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfhmppk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rmnwkyou.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gugljyst.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vikzatho.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2axpbjizl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nnwshblm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urqoxwxp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fseddxkp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xbxfdxts.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wyrdfxxw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mmozrluk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qpnkrcqr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lxphzqws.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tynmnsio.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2lnriwpyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2emposlht.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kjasqtum.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ounaytaq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zqzrclhg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2foktugtb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cewgrpuu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zzlwwceu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgoozurc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2umemqewn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cracirpl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dzskiwcp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qcgoyuua.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ieadhxdc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ruynbmgd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2svcwxirk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vbkviymc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uypstvvb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yrvswwir.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbnehicb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uagwuypm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wpvrtsgl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fjvqcksd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hqfzwmlf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fbbidldo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uejfigkf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2detbkoiz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xlcjjzbg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2adkkwyzt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2llssuoip.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkaygcwz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gocxkakm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wkigjpng.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ykdrvktl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csnzoocm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dsagohkr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cxdhdasm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aqrdaqnb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lvfnqmdh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gnbimqxc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qoxiwrvu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wgjyajku.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hoxwdhlm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2opncitqg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rmoufefn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2chhyrvid.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kptfmciv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iindjmzy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fkikwasi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2icejraxv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2reoaensl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ttqtycch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kixocrpb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2drkwafju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdvtofxq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uvvlfwnl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hipdelru.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gmdlntcc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2epqkshrh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2akjbofud.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xbhksxvs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2blddwezv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pjuqkyhv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jpxakiif.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gxdsosaa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tniduvjt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ntxsryfr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tqwxumqr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2odyueyqx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2muyhissk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qhmevfic.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2akgcswkr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qpcqnsmp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vkipqbqh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qwwgtpyh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cyptdfhf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qndwcmry.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ogsiddis.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2euuueify.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zdgfctrg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fpnrrpre.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uccccovl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2duqcmiuk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nzxxdpii.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jswypspf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2khpaucas.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjvzljc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2krvnhyvv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yohpvyel.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ioqynafx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aptcxvhk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jwqpfzto.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cifhprdy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xylbiexp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wkdvavon.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fnurphsi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2oyengumv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pupiwpwl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sridkyzp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnknyjra.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2okcvwbie.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2igqljczo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydsfgmii.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lsfyrfct.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2uuuapgpn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mjvgcrck.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2scvmzmrk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ihiltkrx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dpolrejz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egjibksk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2omaacgjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvasucya.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wsbypleu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zwjqssyb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ojsnaqha.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2myvotsjw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vovoeiwu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kwvsrxcb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fxtqukpr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2awhdvbyd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xphywdmw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kogopfbb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dldnlach.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwnunetv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tksxwwdr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uwjtcgft.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dazzuysy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gwkxbcec.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjzdfwj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cxzcmhfx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wqdnlmhu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nsggrflr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2boethpml.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bcjljtsk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xdwhmqwv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zrejdecq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jszstsbk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2eprptrkk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2czfhnfll.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vynyvjke.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hddhorfa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ieqcayvk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2avlyjlaf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jeiiydjw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yireonxy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ihtiktgw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hxsugtjw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nqvnogjz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2yvejvibx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2exjgtsio.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kkmexizn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iykqpfhu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2blsgquye.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nqwezbaf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2slrdommg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2brzqifaa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dvkuaakm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fpxryvvz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jwaebttx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fivsldlt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pqkfeqwu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rulwbhkk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clvmxjuu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryywzrbf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fccafkhq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvbpgfaw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2svboquto.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jereepdj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2veoygtxn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tfjajxwf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iyneheyp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2amvvnutd.html


<!-- 参考信息 -->