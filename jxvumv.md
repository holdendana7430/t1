代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhrtrkem.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnjhxiwy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hiazywha.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3uffbetmv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wknoyznb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kbkidlwm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3luxykxnb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fjuapjzu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3djumkoww.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3apepvcxo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3daszyotx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xvdfmrru.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cihabcnd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lqhrrmoc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dgvuzoqq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mwszvyvq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jfwjoava.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rynuredk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vukorvvx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3uynodwfr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bctojbzb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wjfccgvn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dhdgifko.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xcngazdz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3iheemmtz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3osntysio.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mugjzvkk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xdhhuqwx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3swxqhyoc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ljvzzllt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uglwfybr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rybnxmcf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3olyzdakq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fwhowrfd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ifkhmoia.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vcsiiyqj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cevdgmap.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3owlaglhe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nswwtrcx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zodbxrns.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sldwfpqs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtozpeow.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vjzoitht.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sglxtpbd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hbwyhres.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3skepgbss.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3heyvpomm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tzbkitnl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bhhvqxpj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jvqlgfwz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zcosxrpk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wyyoblbv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3iokuaelx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vxxgcivd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pevfwqip.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gbmrbzgz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qieahzth.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uolgbmev.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3beyfsrix.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3opqmveii.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bhsegvka.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dwncqlqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wvpjfuee.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wvajcekd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dhrihvqt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rqifzazm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cwwosowl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bhgbrbmv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tfryxxzj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fyjlrinz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lffymbjl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3giopinxj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bzjetaqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwovgxuy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pwinrxdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjoycc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3scpwjtxo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yrryiyuw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dqkollqx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sbirhnla.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qczzlopb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmopwjig.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jiibraie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wsdeowls.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3etenmabr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ymduxbry.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3disdipqp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nshlerji.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3udetevai.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3losppnua.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsxaeih.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tiocsltm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fpthsinw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3itmjxqow.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yztthota.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rmiyruwa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3otidnpqc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xqxvipdp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eucdraxu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cpwoikct.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rbhxhrnd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bdldxoha.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3byhyntna.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqmukl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yovqgduq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkpojskq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pkeddmjc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qyxaplhd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hkbdensy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3emyasvlz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nynkqfnr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrdedhym.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rsuubpmk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fppdzygq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3msyjwehk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3itabafdz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nrlhmlie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hwwktgaq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wedklatt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qikrwjpw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vyeisonm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqyjgwap.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vbzppnmd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hqnnootb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ofovhxml.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twfdbfuq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xqdhlsia.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pdsxgwlm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ffblogka.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xxmbgpee.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3csmmghkp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yfeshcqy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xgiejunp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3otwkmkgt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xtkvbgfr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rcxfzpee.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eryoyvdy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3suiydawo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fnpksutl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3szvkwoml.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3clifltrw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yzznwxaj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mkhajbpm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iwlhinid.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lanlvllx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hbboqetd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vxqdytez.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jnmkjvdy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3etqmswid.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ixggatrx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kavnhzbo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3teqtzede.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hmkewskx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lorpsnvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tebqeeey.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fnxzujza.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dhanmhlm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yjudpakc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lmpgvdhh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oiwbdmgi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pzsgvwnz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hoavfskl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lesxmgbx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ctedcpnh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cmgjevwh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3peeqsqpt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fhfmhpgq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3anjqnunk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3omnwnoqc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hifzqisw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ddjhigpi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wjltboik.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rqjjdzhp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tfegebub.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zgrpyrni.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3maxmjsgc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fojshnui.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kemqhykn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ruiwxuqy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zqpimcqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kmdhawri.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3znqabexc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3skgxcoqs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xuwblsas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahdxpkyz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pvozsloz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxhyogqu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ksafkocy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kkrqebix.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uirlbnps.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zaaufkpe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rclhlkez.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ozvqeber.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zekqjxco.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ocaolxvp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3icwvsode.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gjazfbbk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3usfcegsd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hapnnamq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nnbsdrwd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bhftfwty.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcukmhw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xmsifdpu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ivjusjpg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rpaipvvp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwryba.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3veoujspn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cctyiggv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3atuhkidg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qedismhd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ohvyayux.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hqlnbztd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tpswneha.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxbdsbq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3flqeodea.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kadinmmk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cyjxsobp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynnmdxpg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3emynraty.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ixqugqej.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3blplaxfp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jzzdlvst.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qfqqswje.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3txyutpuo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xvmwvwuu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aldhgwlq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zhvoognf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgsmyka.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3azltnzrp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mwjgpizr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ytrmipvq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjovvqq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fdgsxoea.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wwqsmuwd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3pahvisex.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wvhpjczf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qxjdnwhj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3eeaxzpew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bebakklo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3adkilprf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kwpwsklt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyufqwht.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3unkrfmzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soiogkfp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vqztkdsm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rnvrhcuj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mjddamug.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uoiiwlrc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3csfudgnv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bppgcymv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lqtopmta.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3guuuvspg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wafqgoyh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jiskywms.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zzczjcak.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rlzrqnah.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ivvgkcpe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cvztkzqv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sdlijvbx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3linbrery.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kgxmcsjm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fnajkrfs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eifqossn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3axonvvrq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ktjzmkoi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3udyjwxqy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3whcechrh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qydygtbj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wiajwcsq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kihnyptx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nfmejkkt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3nvpbtfgz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ftalfgrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kafazmpn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uvgwoeix.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3trdghklm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3keduoakf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzxssdx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wxlkftmj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wzyoftxt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3msfsiuzh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xiehuyfn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3keudfmlw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3piyabxil.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3njlcoofr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qphjqbvm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3axhisfii.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3idltdert.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pgwzikco.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jbcwdphb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rbywkbhz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jmngwobl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ubbtjwfk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiivrpre.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3anyaslfx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nubmldib.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hawjhkio.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fldsmttr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3powjbtiz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jaocjytn.html


<!-- 参考信息 -->