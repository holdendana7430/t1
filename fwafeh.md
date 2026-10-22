代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zylebwad.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfqiekzi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zlvbpund.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2acnnkfkn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ykaqpkrj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wsbbxpxe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zuzxkvia.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rqnqiimj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2icwlfhcj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2duwxgsdx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bbmdxwjp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aaytqonp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2svhtsuew.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xcfhdvmh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yvstaanz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2oyvtjtab.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ygaapbhk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2burfbbdj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ruwgkutx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yvlqkyjm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hyqyilec.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lowzpsju.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cuplgtjl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bhfwbvam.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uucqmvil.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iqapirvd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rcsnpmup.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iihggger.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2culanncb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rhojxdzl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bxorhugm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zoefbwdg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2koagvgym.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mpiwwada.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jkfmihda.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2pinzlokq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hhbvuxkz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zjdxzqxc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rqnoaghs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bjnguqrc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qahyjwdr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ulgxigtp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ssgrydmc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwjzkfcl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2evyhwtbk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xybdrlml.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ildhpxbj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dxcasvjd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ytiregyu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2btswgzrl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xjidxmkx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pkjzieup.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2eiiglqot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2altwvsft.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2emczruyf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dhovcfia.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zqfaujxl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rwbzaoos.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fcbgctnx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxazinn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2eisparpc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ooihtxib.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xfdnsnhf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2twrymtwo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hdczaswr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2laqhzhvy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kwjejkim.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qccghssf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zzwrkiwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glzkbsjr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2olczgand.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wanqtcej.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ynryhnfp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmyyawec.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iiptallu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2atjlejtt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fbuxohav.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgasbsxj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsqdcgrw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vtlfwstj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khcngjxw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2spvlgnwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2waxvzrox.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wkapurck.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wbmtapjb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkkraok.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hynalnij.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgytfxx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mdcbbaiw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2yudzmzlq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2slsiikjs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qfucvpuc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2agfvmold.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rgruqcsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hctithql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2onerovrq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kbfsfajd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ddaejnnp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ldyznkoi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2iiemghtd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyazltbe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eghgcnic.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dirunfgk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2medfzmmi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dpnagdao.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpxxufyu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ldvgjecd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yfrofutf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pgaaqgwb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zxldoeaj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdkqqdsc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdaechwl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sceidusw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ieqrbkhu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vrsoexdo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tvzngyyb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bcruquuv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mpjylqua.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ljsvuhfo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vylkhooi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qqavfcag.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bpqgsxcz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2soklqkfx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2czwuyjqh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vtadhuzm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vnmpfred.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dhwizndw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qkxudtzt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2psqzhpqe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2omnlcxrk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fzdwfibx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ecwierem.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tfolvlvy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2twfshogl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uepfwohw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sdxmztxj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkffkvkh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cpvvqkiy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nhgnmaob.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zddvtivc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wtppwmsy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wfqwwysy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bngfoaqa.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yleyqysr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2twlppxuu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jclexddx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cnrofdoo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfihpnjw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zbgsdtpx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hjdvndti.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2eodclnye.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qtrptoaq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qwnrzclq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yssjdiyo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2onxiojsl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uluskubx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2edbqozyw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nbohieux.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qutrtjxa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gmlatuuj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcbvadd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxdfhgoy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qtmtawsz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dghasyrh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2exttslkm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vchbivsw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uruihmkp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vjshdxhx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vctqbpwn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2domeptab.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2koalbxre.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bnqcsnnc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2earuyqgk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2grliajji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uszqptnn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jhbyxdby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tuoehvpm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdqzzplr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2erleuswy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kvjezcqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvbdkpkp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2quxqgvtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdlzogcp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vdhiwpqq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yadwzaju.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2isqtunwz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2yrqjvpyj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ogarzhoo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zbopyqjc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yzvamowf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2putzlqxf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wtuwrekt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fejcvhia.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrtebup.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gkglfizr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ttewbrof.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hetuvmit.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xghnrklw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qjnaouls.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xmbwflgx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wlewxrvw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yismbkiw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtmltvle.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hpukxxpx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cwpbaydm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pzftbzbd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjzbptj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uxsassnx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nbtrtbam.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nrwvbfru.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nzfprajh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2oxbjfcif.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ynhejccx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hzwdqzoq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oojqofpj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2atrbxywi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qbsbtqyw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nrfwhztr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mhlwikak.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bkddnara.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fdlyhbzh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qpvlrbmb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nvjluqoo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lxpkaxsq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lrsgwrzz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hqtcklxl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ktuzvvxc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixturnes.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zynuityy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cfyfpfxe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2suohpvfz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rvbrhygi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2btqtfgvp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lxkcdtwu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tguekbwj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kemtcuwd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2njfntxkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxgyhdas.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2swcgzlqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2incdeqcf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mkmdxfet.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dsitgcju.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xcuerrtf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gzujowgi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nhhacnyp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vtehpzjj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bxxfpgcn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2boyfplqn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zjlubshw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rbqemxqt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2awqibknl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pyevymcu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2thrlrxzr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kuypuxtv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uwkyvsks.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vfjiumfe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uwrtlrcp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2iwrsmgvo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2gacgudmn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wdfkhmou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hsfooktk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vhhchlei.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2olhlgncj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xnkwbkng.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dbmepnwp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2aeigizja.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mzuivtcz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kilrxmpu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ecxjdnpa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gidiihgb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qqajynve.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xffchfsl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tkxqqitl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2aqsmmqwx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wrqhycgz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rnwkvwgy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fpxgmmei.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wyxhfnyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uleeylor.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mxhppamv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2chqfkpxo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lgheacbd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ywzcyvlg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2knhyitoe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ezxtkzet.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mnmxbjwr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ldtvvgmj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2iddkvxcn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ylqdxfiw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vambkwxq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lopgksmk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hxfrbkds.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wlkrosqt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2erjgxtsx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ebflpzey.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ugncbipg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bqonqwwg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eqkndifl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kpvgrmgh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bdbpgfug.html


<!-- 参考信息 -->