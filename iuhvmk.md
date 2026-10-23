代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ifdwvpqu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bkfxhifo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zgwyfazp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kqasibzg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mniaucdn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qrbihxvl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ebxzvkty.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bcosfxsy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ibkvlbfp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nqjsimdj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gojxjlor.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vkkycbhy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3thkzmypi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xzvhpixc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nppmsihs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwdvzopm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3prgsyrwk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3nlndgrxq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pgyunnrq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fjbzvnoq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hbtveutv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hrcklqoo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3umhirwsj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3slpigoti.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xtztfmju.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eiodhmvv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bntzsdvt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3uvsecpnp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3avkurycp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jysvabru.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtjfabw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bdjjgloj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3araxgcvv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pegohdyr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3neobladi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvclbtc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qrackxky.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zchrlrth.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qthcjpyt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvaqmce.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uhuaggkm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mgmorzck.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rchigvbv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uijhyfws.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3krgfocjb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tccqcmsg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xxivwhpo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rhnqzqff.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3eigqujkx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xawnfqag.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3edjmemkg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mkevmvtk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmvwfyt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zyeuihmb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zilmndpz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jtpghfbg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lbodmzaa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cpdckrrs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dfkgyttw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3brlfehow.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uaxypauv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ouiyefox.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3utshvzvs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kmqynpto.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nsccfcjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkqiyfuy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3nuvcpmeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arqkauqx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kpscadtl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3muathbor.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xabpocmw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gpxfqodj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3svloejej.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pzxqbtwi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnaxzdvb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uxluwwvk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hvywijqi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3acgptyma.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gcxpsfqm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fggdtesz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vkwzakbl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vexpmgdx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qlikxprv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndjogbdm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hqanzgqt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nzovfzte.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ctzdwopk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vbzevyhs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3inemdgro.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ivpuprjx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3htcyqeyk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3glansxbz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mjinanza.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ogxgshdp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ktphddkz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tfepccmq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzynwiyn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ueczjuxv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pjggyrys.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3elitrvty.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpssnasf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wbjdtfps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzsyfdvi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3umqzwgkm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xajxosea.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmkvlngt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hddqcbgm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3auagxvki.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3aevzapwa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kzbvhzqn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3obrbarew.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3itcbrfeh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3grpcvzfs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdawxtcy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wnmzpgyx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rmdoxodx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qhpysanj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jevkjgcf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bonjszpo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cacvhxeq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ppbiyumd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bvfyjqkw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hfdkmwoo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dhbkmqcz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ojmbtpyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjvzbey.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3orkwttcr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mtzlbbsg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3whjbxelm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3puofompa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ocylluxk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3liqcilsi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pisyybik.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bgrorzgy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3orirpjun.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ddwwyogw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzbazd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pczudbbl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dwsraqxc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qrsfczvx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yybpbipd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpeoburi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zlilasot.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ijjxdfbq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qtvwqnzy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkzffzaj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zfprqkhb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pcbqsiwq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xwpiwkeb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wtgvhyhm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xchfmbbq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kanzuxrd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cacttmsf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hvzalzqw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrrrrjzy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yycfdqes.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3snnjhmat.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mbvlxqjw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqdecpll.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xvdnxrao.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3smsuszxc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bjfjonsn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gdulhoti.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bghzjhva.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kgwfyvjf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xubjzwzw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ulbfpigb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3miwnelmg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ccxmtdgb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zazmavvu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dckccnpy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rvohpvht.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3okecjdds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkpavek.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3iyjhohmf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ovsfaupv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdnqnsox.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3inkztgbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsseoguy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vyeosioz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dajxyifz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tuatydrv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nknqriyt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3upxjspuy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mrpawspz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ffmdjwte.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3snricfni.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vovwohyh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iouxtarl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mscrofsw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rbcltpkd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3idhmikje.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ovqomcjx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yoljvkyp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fevsrkqi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zwzindyo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3awucrdzp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rjaqncmu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uxnnaohx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rvfnxevy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kumnizks.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3skomskyg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xgvjpbnm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ognebyaj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gsjstant.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnsqdgxl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3onxsiqrz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3afzniyjf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sbufxcfc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ooxeoywj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rglxdjxd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tyhsmakv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ypvwacnf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mimytdxd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pckmmwir.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ntcdrpbn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ymiijdxa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3anbbntbp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wxgojenq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3stmzxzer.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mhkzysrq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xtwdyxag.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnpbyng.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnxhqlnj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yyadslct.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ldbatuxt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3omiknztd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ewnbhaip.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zejdbcxg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ugcklfyj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3abfbujcj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3klsogqqc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3autaxuwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czmfaevu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpinszxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmobnido.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tdvokuxo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qzyeilwv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hyyqphvb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mtenital.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dxhrrdyz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xrdnljlo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zatnwknx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wdwfvlrh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hbwtzkoa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yzbnrumy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3sfaudkkx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zoxopfty.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ixnkghmh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bsddofam.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3smrwimmp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hkpwxjoo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcokdth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cduqtsko.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xeeujipr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tcldvcim.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ltmatwmx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ywdtmqsn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yqarxeyx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ycygqyvp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jjfroypz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3minosedx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cayjuzkf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3soazfpnq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qovgbwie.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ojcvlskn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jsbdogag.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qhegziga.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hofeqepv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfszqsx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3solcqtgs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vtwgkeyc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3urknocqp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tsgftdxz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vemexchz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wxyrfieu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqehwohi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qbnhzlbe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wnmobthw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vcyhnjtj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3axgosgot.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vitegmxv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gphoqupk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3biuezbwz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pedmxzet.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mdwtrhjx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kldducni.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ceekwwzn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dvsmtnaq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yniiauox.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jverojjp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hqutvrfd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nhbhphyi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mnttkgce.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ddyxqtpw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3miygpbly.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hptlpqcm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3guqdqxwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3npjubnzx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vlakdblf.html


<!-- 参考信息 -->