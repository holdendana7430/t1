代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lnjdgqqh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vqgmqggg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wasryspd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hngxxbry.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2foxztuhm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kkdijejm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xcbhxvml.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fkkmypfm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2blcaqfop.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2saybxtdb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wbyvaepi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qxvadcgs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ogeeehzo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xmuehffc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yaymzwbo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cndrypvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tmwokthl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fgilcvwb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kpofdusd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xasbcrxc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vpzqtkyq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2arlkrmbn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gxmjlhor.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eaymtggf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2udqxeajs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dictgujr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lkbhsrce.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gffgencx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rlfociqr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hakynohr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ohbsqkfs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iudlcgwv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2onapnuke.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omxonqho.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nasmtmiu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xhbuzpiw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2loexyxpf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tpolebqu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dddckrbx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkypsgpz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ijgufidf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oqnpcuua.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ztwbvrtm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2byddbsud.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mdqgywhb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rzdtuqsx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsjjuqnu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gezzqlgo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nsdhaqpk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ymbnzssx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zhafzzsl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2baqhjsjd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eucwargm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lmtbpiez.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jgswgrtd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2evflrick.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uejtizwg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tdkzjexg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zyyfvkay.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ohavwszc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qfumtqui.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yzrmykuq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nlpyilmy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mixcugqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vamcatfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diyhswzo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bqikkhdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nckpfkqj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mfiqexrn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoclxvjn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wsyquali.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrnwgqk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhzqkhc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bjyqbnqz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pxbgnqki.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wjpmnxdx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxsvjzmy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nkufhprt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mnfzrnsf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2aidmkmjk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qpukgcws.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ryivqdyr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2spvburdw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojblwpyb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yglcftgy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lcyabaza.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bamtauob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2evzizhwd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lqnzpkqg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2crripkli.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iyrzkkyh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2erdjkwcq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kolookyh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hrnmtwix.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dsljsnrl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vxzqmzlg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sghiqxxt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmcurbgh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ddlwqcqx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2epxrukwb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxfuplwd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzdlkbol.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tauvxwqv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zxbopdcg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2enueharr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2grkyrlnl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvoufsi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fttazjuq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xswasuxo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gqqqrcfv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2iytcmzvy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2royacgnc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oqdycipn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eqfknzyx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wnqrcwwk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrswop.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kozatdjz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iesmtqqd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xwnxprks.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qiqyheow.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2asdrgnhm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nyoqurtv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vuwbnfkt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tdyyygip.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bmfjbbjb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jckygrpi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pwbqfkjq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qkydnhpe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xnuqhcdh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hxlsgqxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hhjnnvdr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yoelogoq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwgawrb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mxxbvvno.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nvmldszf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xbbszywd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wwwbjnde.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zegtmyxl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wphuaofs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zzoefzft.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mkrjeqft.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nvcustpi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zorbovup.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqxjevpm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gevexvtd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pzfujjvc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jxcqosxo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uyrilgqx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2eiotcxqi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ppjehvts.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fvmwaeay.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nlmqavsn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nfxxdpdg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ygydfuhn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2epivpgjn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jujavajw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2sljjopmv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gleoshmw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2loxnuvto.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cmzfjbop.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2sjuvrcdt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kxjihrhh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kritgmjo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cxjpughb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nrikskju.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ifgioemu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bphacrpl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bjdkhgyv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mskikmcc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2uqskrnst.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cehsqrpk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iegjoocz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bzowjpqw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mowzbmra.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2izifltfz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2awbfbxyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwftigsw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gdprxxjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylrodgmf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ctwfeviu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qqsylqkr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dnaeextk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ofbglrma.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lskqadxe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gsjmyhlw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fbyijjfv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ewutvril.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2iquaajqi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jfbeewmd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2aipitywq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rjyzonor.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2akbrldrp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fmdujlxn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qxjosmiz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rqopmjqa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ubujlefh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dcblktmt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wovomjrj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zodpundm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hmfiiymr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tfwgnwlz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oylrtzca.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yekjgrye.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2cmzvenof.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrokulgh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehpfvoyd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ilodntwg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2crqlxvum.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jzpwsfed.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kuvebpix.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wlupmunw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2pybbyuwc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yzqaunum.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2llwrrxzo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcdnzlye.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vgulebmh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwmjryz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zokhigam.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tqocbhea.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lwgfqnxd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2daqtuwhx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sevjefmd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aujdutia.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvwnajmn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dqoffini.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mcgsbiqp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2syvaalik.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2owhfainy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2owtbhgoq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2etzptctt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2obaoamwc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2oisfwjyj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hzuoizpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkhfcayg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2autwjjoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbdyccre.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kpgcxiqk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2munsnruk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bygexwxx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oiiylvic.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2plcugari.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tpnduvfu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eyvcnipw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rtwxkshq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lsnirizx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xqmzigev.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2sywfawtj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oprbvgnw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hfvvtpfj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hwjduyhn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vpyiqlcg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jxjqaizr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uhdgltui.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2axpmlcmg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eskmnbvd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gdzqgxpj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ucdvajkb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2trhcmikz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hwqklwej.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sphfkbpg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zsvdkasm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wdlumkqw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nleuvdpf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2slpjerzz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ztbawkgo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2feekmckz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ndbvajdb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vaovagvr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ojcfcziq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2evskznll.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gfwvreyy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yirkfxjk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2sgksucfe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2aqfhhecq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gsbaxbti.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2laojjtls.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wzhuqkwr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mwcdqucx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hcxvoytc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2urpzaoqg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2enwqxvvg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pdagkuya.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bxsvjakc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rfuydwbt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2nvrkfino.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyagnvbh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aqlodmji.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zzcvwfjw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wjcnmcks.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2joadagjl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2eemphhcy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xzxyflhn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2axvnltrk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wwknwrmh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2odwlizej.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idjglzhh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wtvdiwgn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zcsuqwcw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dkgkjfae.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2icwmyshq.html


<!-- 参考信息 -->