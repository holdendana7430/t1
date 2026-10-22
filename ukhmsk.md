代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cigtlgep.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tzwodmcn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wwiqlhqu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2msfmgufs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ifizyefz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2osnkembj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xhiddmrl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kbgmliav.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2noiztmxg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kkngvwvi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vyezcjin.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vtfwtuya.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dslmimsr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2romgbtoq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2guxspxyi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vtlmtxxy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eamwokwv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uwsumaie.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2modyqyfu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gzouicus.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2byzroohe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jqjnmvlf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jmutkpvj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bglxkuhf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ohmabskh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ljrksoco.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ialkxygv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2adgkpmhz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xscxcpem.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmxhtow.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2okzgujfi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnppzlce.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2oobqbloo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zkalhgbp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xxonasuq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyutqoeq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wgnnqtci.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jktqdkil.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gtqxyrfe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ythqebbv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ceiibruh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2byyqkqls.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fnfoevej.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bxzukwhv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hruecwci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cwmcrtqj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hslruurh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dhfjrojj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zjuodkwn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2otjzygkg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2unabiryq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2egklltpt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2drdngmoc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tbjfmoom.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wxzmtucn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dpvkebsx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2paaicauo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jigiigcn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ntkxfrzv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2eiwkwfar.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2swgrtcpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnlyzxcn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cqmrizwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grdquzsg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2btfhzmkq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qizalqeh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fqtrlgce.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lktmmraj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bkpbqflx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vggxvswf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbbgybai.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kpqviysn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqxbbjii.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bcsmcgkw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2daafjktn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zictupfg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nskzgjlh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kxttdumi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rytfrbvd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ppytcahc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ckrxxjbu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfbkfmi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yvvjtovc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2edqoftnc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2swqkwovh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xraczpmu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zvbjqrmy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zecpzvsu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2uiuoqfab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cywdlsca.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2pjljyqut.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2obupumbi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dunjsycr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2amsweqrb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2quvovnui.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gggicoqb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vcueyteq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vdsgqgiz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aooroaqc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjzpflze.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2txmjjicz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zwbmzurm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhofpdks.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pqmvsnfc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fbymypti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ihyvgfdc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wjxgwcdq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgatrpb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbfgdhy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dunrxkdj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rdsfkomr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wwkefjqn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2idvlollb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jafrcqbh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xwfbrozy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nkbryvhp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2afqbqrif.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xawqgxac.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jmmriegz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bjuycrdq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2sbuqcyoq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rzsezldz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2njnoxgqb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qwzrcawi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vrjivsik.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nnqkieav.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vcrinlze.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mzxithot.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpzkimfc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2owcljrtf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2biefdkkx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qlztfgvq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tuzoawkp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sweqtmvi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rkueewzv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2escevbkz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2feojdrft.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2snznwxdc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqsvonuz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wagkvcfc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bxbybrzd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gxkrkykn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2epaziztn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rkgxwdmd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zntwvjxj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bpdgutxg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2amhgippx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xptyiojy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lpfalsdy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ipqyqgvp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ctjxnaza.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hprcjbhv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cxsqyecu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gishxnej.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2oatfavuj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dylrueno.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmqjbydo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mltwargo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ccsktrel.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2etspxkrt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fosmwamb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2iwqbszri.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfzldnkr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jvhjmrmp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fxcgijtf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bvnyrhbr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2exuutcij.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rxkrdrgo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vajopyzq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gfaldlmj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qvaxebzy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dhjzsjje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsjjmizy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vtxfgjvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqsvjpzy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cfmfqnpn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2utiqpehp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifsgirtw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dpyvffnp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pzaolirg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kynabrnm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hsvqaqhm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nmusaxex.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nlhdrmuw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kmunbhju.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2arubqegf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mxmumsmz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qbdbdyiw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uriuwckt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjoxjo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2venxwtst.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vemjnsob.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2evdbzcjz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wtybgkjv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xmwdjdcs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gnvfwdfx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2bxdlnmjw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uapyfqoc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2omnfsuvl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2xhdrclrm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fmmuiypr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rwvnmabf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hhedlayi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2adjojvby.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lnijneya.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyanllbq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ysshnujj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mbdlukui.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kgqounrp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lhmhmptc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twfgdaah.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2frfqepvz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zwjafipc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jlwaoejr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jwabxavn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fqczbwiw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xphhittq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wdoehqlc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hmzhmvfp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxaepvw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vsjlqswc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kgixgvgd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wjgioxvd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qbhtnpgb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ksipaoek.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vbrkkcnh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wufrcjha.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ovfypqup.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ooiyjpce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcfjdhbz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sobrlyzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzebcjdh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dercxqhq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ipxiqigb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2olrbmsek.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qvbezaew.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ssvclneu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfpncr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ckosjzda.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hbimbron.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2iskwnxta.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vtrspxta.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cduaxqvm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mcaemvrk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2avpzquww.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2toskoeuj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dnqlhove.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2linopxsx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnujacou.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aptouhmg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flioesoo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hzhqefzk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gxwbuawp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mehazrbi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gclawbap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzjkui.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xcsgikle.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2drdnlxgw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gaelwdrx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xgztdvjt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qozygzqm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fflxcxzg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lvlneebw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ozfffsay.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lyktgwgo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kscxkxqg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cjkbugil.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2svheaihz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ishkmjhp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vgnzuwkc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yntmgfcm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ilmnjyhw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ihiqylbs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rdkgwdjw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hnedmarm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oqhsjdfd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yyixlsfo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wkpvlguv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pxcjlffr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfmmrnfb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2eirijslv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2liikaipk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iekexlef.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dyddohmb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pqnxthfx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkyzblhf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kebzefxj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dmqirkjj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2eqhpjhkb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dwqqvncm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qjeuiivz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oumovtqc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2smptciod.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2agoairps.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lfigtnvp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2opwxkckq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmyoqre.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cnfwzmzu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xkzumqxr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cawbrhua.html


<!-- 参考信息 -->