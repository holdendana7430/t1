代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dphkjnyr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vnfaghgk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hpqdntre.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yufudlna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbfufozi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yfnjjgel.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3estaifxf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zlmxmgce.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ozejnhxw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ryzsotcy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3paseofua.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sqfwrarv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ignclrcb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kngselda.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3oojkfwxo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vbuluagb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fhhzraja.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vpvcdrff.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3izdizbtc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fjjegxlr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hvrsrgdg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bfapjazu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lrwkdoir.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mavhjaxw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sabagwrr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hcfolnfk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vqbntctc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vkkdmcct.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mrneykeu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knuixvqv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwmhdxie.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ejrjcxpa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zekpwfij.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mddntrto.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3eqiejtkg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ybseeinp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jvfugzhc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mzeaopzq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pzoxgkco.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3isdroute.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qrwagfhi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tqammxtz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hjcucuyr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vbxpyazg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3blhacqxi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3goajajoz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zhhtqkds.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nibakihw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3moaahyfd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3osibjwuk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3okzpluba.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqplhoh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vxnzmpiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ngtagojo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mrdmlauo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xmvopeky.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kbanrenv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mkgjrxtz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hwjgwpkb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bwbrhqbi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rfnaeiye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqibudxs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gwbdatbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlofkbda.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gpgkumwg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtudqdc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfhjuyn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zaskltwe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fhhdtftz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlhbqina.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ogcebzwu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwrlhnb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3takvwudc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bsknpxjl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dwcinvaw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bawohigd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jpacyjvg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3osffvqry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vnuusxmk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpxezbsj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tewowlpr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yrsuxjdz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ldulilot.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hsmbkcxv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nivbbpbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eplthbnq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zwmhhpoh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wxtderpm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3kbspyutg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ohnzsftv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gzbeqluw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ztbfhdns.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvszjtwx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3owmduyxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sbmctygi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ybhsbzfb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3stegbgjg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kudzkycp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvaocid.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3acwbrmxv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zcomlnux.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bldmeqfz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vigvdfya.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zfufqgyh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dhcdbzvg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mvorctlu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dsitylgz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zrwhhdwz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dxryfokk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3woemoeyr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pqdbuhqe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ribsqbyx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nydkvpps.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aqybbtfu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jvradiri.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gbgmkbxi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gaqxhzie.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ixxlfreh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3infmrmos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gqeikenk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zwurzflj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bydmhdvr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uzyisjgz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lqpggfcq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cksxvpig.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hxhnyndu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3umzrnvka.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bcumtkoz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkvyxqqu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ajpailsl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uvdwcptt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yzgjslca.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qlzcymsi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bflrefva.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oxamrxoe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xrlzwtul.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xnznoqgu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3crhxxbwy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3asskiscq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3phugrnsh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nwjmljdk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjnmnveb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fnkxescn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rwxvktci.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3selcxnmx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gaxyztzp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qkzuwxto.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3grcdswoa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrrrtp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wliwfrhz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpberjbk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3laiknvmj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3umcvgnxc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqfhxlel.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vzeaycbd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3abbyjauz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ulljxykf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vzpnqbxf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yyrfeocg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pcsqmcij.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ebexfetx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3npxfgphn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vpdwxdhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3thlswjdr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3agqxhcrf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3emofsnde.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wuptwufw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ffardvfd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gfdzuhxt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3trimsipj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kzqpynok.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tyfltpns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzlkyxzj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fkpvlptc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aicmeprv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pwjqaamt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cuhoqkjr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3iolgifnc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wqijhdyq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jtqjeaaj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zvxoruxj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vwozowsi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ppyxliqe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dcfznttd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ecauxuqv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3azizoqjf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xdyijjgl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ofwlfnvx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3eexmjnkd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3voebhcjt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pesytfge.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jnucysza.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dopltsih.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qugyrijo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3thpqvchi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3deqktjjn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wscnrgvl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pnyhujif.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vyavwvai.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wkqcfioz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iukexxwx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fpsbyqqy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sdpctcjz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mlgusnyl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fuishlld.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpnvnqyj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zlhlphkc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cxqygvuq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3thcohaqs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zrwitvxj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xoeokdbx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3exiasoll.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qxyxraxx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nhkmnyzl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vpcnhhaq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjjyemf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3meletjyg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3csfaaznl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bmojysxg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhebqzau.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3couvubdv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3oilfizqi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3svouwgnf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dupcnpoc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vfxnhmmx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3oeonortx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zcvjwzfn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lersmtlr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mjjlsuyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyrfhxul.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rvmokypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hadziwaa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hwamcuha.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iatsuxsq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zeynluhx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qkgqhcmg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ajvmbycd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3arnbggum.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lnbiomfq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gmcukbyt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wseadjnj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lkbeooge.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ovcdiqzg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omecxwme.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ldlxbrnf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dbcmdbpi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3elsjvcer.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ajergcix.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ypcgmtbr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3orrbsaea.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hjlgmxdt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ruuhejin.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ynfckzjn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmhdqvre.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jtaimxof.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcljgr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3yccarznr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zsezytax.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lhlftzol.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ebdmtsdp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yaktvhwb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hfkinltl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3okgcjzkp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lmztbxmf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bfswkuaf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3yjmuhpjc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ukiwfyjx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3czqxntfo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mqwmgwqv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jnpfbilx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pexottar.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cwqtgyzg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ciaojvvb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lakdledn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3oluexyxq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pqjeiveu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qvlbabwe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3inzrxeqn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fmhwudbo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utpttzkn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ywfsegij.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3reldymfz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfvnnqzr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3iugovyih.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3eedastxf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtzsvjlm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3khovkuqq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gtfdzsab.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3drhdppdw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3exzlwffm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ztdobnqy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqerosj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3itoasydp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sptyzhnh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zdyscskk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bsaykuyo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3eehikdpv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ugrmflhl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bumqllee.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvavmbvf.html


<!-- 参考信息 -->