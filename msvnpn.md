代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cvwwimhm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2npbtwwbf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2coitclfn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yissshwe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2egvjwhrz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ymhbhitq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jnfxliaa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ipobaocf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yvxdttia.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fgkewava.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ibnkkjud.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hjptjyqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nzxisdus.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2osnntdqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzsuyze.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hnseaaua.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rysegvda.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nnxncate.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nfohggoa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2felnqlfg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mqpkmyxr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qbyqjtdo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2oozaflmd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xwegwfyg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2euustody.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pdmkngta.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2plgkybzu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oakosipp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qjrrlrvh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2agoecqfa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cmvzinhi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vikuweci.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2khojfrbo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fmxoisvb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wyyicjwz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bfbjmwgc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wefkydzs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vkekmnrq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wjwmmamm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ckpabkjw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqxmznkf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2astzzjcz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2plngawuf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bssaxzxk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bxydsmpl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xskgudzn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wxzvixoa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ayglbsza.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cckgcsbp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bfdtenwa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lkcktekx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pjuwydbw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lnfigjdp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vsqpqini.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nqfpudmi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fasfpvfr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dcseoevq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ufrbrotc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2adqgphel.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2eityxkuc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2iorkelxm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ozqngbpc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wlgtjtpj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vilhdfho.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uiesawdu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qobkxtac.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ndjwgxaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ebgitnfe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mdfktiyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iidhjicv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kehhnykn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdnavflx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cxfdyqry.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpisilhe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2poaxspvu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kiyprzpk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2veiwgmnp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gdgbppdi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2venrekwp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2vvcmtgwd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wijjoits.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jwxikkjq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ygjtwajg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uuiflaua.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mlsqsxye.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2diqmadcf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2thyeufvq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwljylon.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wuvbrsgx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fcnfxhkw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rerivfau.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2brlnafyi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mbawjebv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tmanazjp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mkxcqolw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2sdnctywy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ypwgkvje.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yrepxaok.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rplpfzdl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dcroaaeq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uukpkktj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcvflirz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wryakngz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vymrdiks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldcupulb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ntiosjpv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xywkrmai.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tjsbdkzc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wtdwgont.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2boeyxoak.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnkvnmji.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2icxrtodu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zqybgrpk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vvvjvahv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2indjfgtk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qblrraaq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfaavsle.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ttyfytsv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kaayuayv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2glamhnot.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzbnazu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tsltidbg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gnstixlq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xvfrsdvf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2enzxllgc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ecyncqwl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ojialhhe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iaooxaxv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pbwsfnic.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ivnyhwbl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2umqqoncc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jelxjhsn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2prxrivoa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lpxpponj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gohssufy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2grrrgttv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knehzfpf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2scbbulsw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bpbraahq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vbdtjpdj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndymtyrk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ifnevrnd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kumsmzlv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vkkhzezb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2npsfrwfy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vtgvbptk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyflcsfb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2seamfmuf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gihkxfmd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2enxtxkvt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gkmfgsph.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmjgokmt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xtturihb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hwhebrlo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bvxbazbp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qrnnsgga.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ckalorkf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cdhdgzhs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ozvuxjax.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lvkdermi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zlybefcx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2emetqbiq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uxudnhlr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ktqgaiep.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pofcophb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bjcmccsd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oluqmfza.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ihsvniqu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nawfztlh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tmpcmibo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vyzetgjk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gtqbfrva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cjhbvfro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hrvdwjih.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zbyzsjzd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dbtqvzrp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nywineax.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbrqldn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2uspseesc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ikidomno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmkkcsbc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jhmpnfao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbgmkavz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xmncdiyd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rdgjufyl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgmkxrug.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kmkrrlcq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wlbkhtqq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2djuupanr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jpswntxe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gfmphxiv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sdvwttut.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wnnxsyhn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hciwhahu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rhxbudwo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rfkqnxok.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uwhfgelk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uaehfxao.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jzhklxnh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tfpwecsu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lfujesez.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sygswmao.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fksoxbyp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2yjspqpyu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zfawxaqh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fswrfpsi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zusshqwc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nlkouysk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2csvaqdns.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljafywor.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lqbqrotm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2svmfxowf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hyaojecp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2emxtmkdm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lclnouol.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hkxgdqqf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tdivsfku.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2eczjshpw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqvydcn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2agveptmc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kpzfkygj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yxzwpfyd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vgkxuhov.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ujbpttut.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cwlknbxi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2agubfepn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lwfgndna.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcmlqpo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjbvxv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lscktgjx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2etwfvoqg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hffeuptd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mhwlptam.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dijltcvp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2midxnzdt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2eyzkgltv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2olkwamfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtvojhsg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zmcgzopi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsujebii.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zauqufmb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wlcgpqbv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pvdnmvvw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hvehbwzy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kvahakdr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fdykrspy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kytfrjvk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lncbectq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2eefnwxur.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2whmkheso.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjiktr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2veeinzpq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2osxhinox.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2lkyayjyz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmoakaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qoqhuukk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmktngpm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ppwcqgaf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tdrrrfyh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nwujidns.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qqwudoyu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nigdprds.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sbeljxfe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgwcsvh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zsanjxjw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhsalla.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cbyspcef.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdgwylbb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ftjmglot.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tcimilha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2whdnvuij.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yzmkkftu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kqdndtea.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wddvokqq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ozbvvlvq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2myfrpjyc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vvnfwwrn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2epmnvpeo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2douzrhpt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rjndeymv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vvplivgl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kaboudlo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqbnoja.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lppriasa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2scmstadx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2eidjigjd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jvrdmusq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzwajlxs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vvpzvedl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybydpjce.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gzvzcsox.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yemxmfkp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zigkesga.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2awuztmou.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2genicmuk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2coqaqtev.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kalsyfrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2imurnlys.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sapwytoe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbqhlqet.html


<!-- 参考信息 -->