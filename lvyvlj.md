代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkfaxou.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2owdasama.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kxsnaaas.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ttbrpzsx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vbfnedqt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zgzwarny.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eutuzrbx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lgjbazku.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xftrpooy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qdlmyffn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sugtkajp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2twpqtplk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eeufjsbg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vyyfnqkt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nxcjltup.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tvzmlgpg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wmrnfbps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rkbxwkwd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fuulsang.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qarkioro.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2yndhnwgi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ntjiiaac.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zefzyjgr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lkdrctvy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ujstjcwc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vozoaool.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fbotwhwp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozdvawae.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2juymnjak.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qngptcxj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2koebjfxu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2sjhhjwva.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jymzsuzu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kddwjxfw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iylzbdhz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2raoxrmia.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmeyczp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iloxltmy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nbtbsnjh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2khzzirci.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pfseypll.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gbqkhjzv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ghdmnmqn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2npkektlw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2unjbzzge.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pptnvkcm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ulvqxnli.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxvets.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vmnlkikb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bgqarghy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yjyipgva.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jaaqlfbj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ohmyhldv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nxofeywa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rbdgrcvm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mmhxiyew.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxyibrg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ujkyzsls.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gxhgxmle.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cijhczjy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zkzsoqty.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wuwnqqla.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hovpipsa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dusgqqyg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2usxrwchw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2glxuusay.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2btonqdig.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2avoclbov.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bgygzgsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evclptvq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vnsfymxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmobxklq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cpwegaoy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lowhmelo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ywizubmi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kfvmjzml.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2afpymzad.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdecamt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jizeygcp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxqgoyl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zsxebgec.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hluqelig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hkzktdui.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lhmfhjhy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhsztjux.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xphkjthc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2charkzdo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uawgwkpr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uxjrruoo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qwudmwrx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gduwfinq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lsbevxhg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gelfnwbo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2irkpwcim.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qqjadkyq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ehkxrghd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2znahrfvt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2emrhgdyb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lsiwxuoe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rrkcrsuj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bifqzwqc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzscogn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wwnmotgr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwrcrljx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qaefxshm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lxjacaai.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrieew.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qynntluy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ftjvyhjz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2urobgsdc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzmedjko.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hxfoward.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gyiyazit.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hgwivdhx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2amldcors.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkfpezbl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ooshlbpy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icnuzlhk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nfjvpehi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mesviaui.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oxeepquh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lcaffewd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zwhqcahj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aboynntg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rdsrpzqq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dbiamtsq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bkdgsare.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2atkbqyrm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zosqqtiv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dlyzquzs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2divbdlaj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ofynyujc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vsahyhof.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2otlyqczh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xujoamkq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mtdwylef.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jndoheaf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ftqkgbab.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfdmpxug.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tnczqvry.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iomqirga.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2grvomuxj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nehccbse.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wdwjyell.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ldxzewed.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uhxwlslo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ndmhwrqi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qagwkxtf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bkuajtkk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zdkswdwy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2varmlnyg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xhphwngf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ivpcksiz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jhkeyzdp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wwrpylpw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xjpaoamt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wbcmpjif.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ococinly.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2btpizimd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2raayfhzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwvzvfb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mruzoffq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ixhcdbix.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ocpczqct.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bgfjvbik.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lqpcfitq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2railxkkh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbhqxrmv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fenvcptg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2syfsighc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kgbutmtw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tdofpbsh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2sdzfwveq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zleyvedf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2azjqzxfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yybkquyr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fiyxborr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ujyfdcuf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mxehugpx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tgcmgtdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyxutmar.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2itkbuueh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkblbvec.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2onrvvtcp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2iihtrmei.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ntkbaqrp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fmdqkwpj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zfcqwscr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dngvawlp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rdadkvkk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nbrrmjkl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jfglydxm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2gkrmbmfi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nnxkqcqw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wwvdlxuk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2krfxtalp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jbgxztqt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2sabzoldc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mxgegtgk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hkvzzgkh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2szjsczzm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yjefydeg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mtfwbnqf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pstrohdl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tdpnxmnt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2feamllim.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oolttsvo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2autwzcsm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmkmtgf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkkhivc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wruzzgkv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sjsezyug.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cooocdhr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pswplbeh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqeozycv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zqdeoura.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2idwomivu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2srncjcjk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grofsbqc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2engdroxs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vcjftvat.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cosqgepl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2warqzcfm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jqplunqq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hdatcqdd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cqbqgiuu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rvwjbywx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2imvxjwcc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2htvfqsdx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ehawyhsq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2udeyuxdl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vsylwtav.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ieokbaqd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wcigveov.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lyovjfiq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ftazpsdz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dsnmtjlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmkvtybk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2aqryfunf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjdnmfnp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2umuryuyp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pohhaaan.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rredvxue.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hdynrnwn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jruzglgz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfdwcsdz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ebfhwnqq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ygipfxid.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2knakpqsq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jrkuwvbf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2oixonikf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jprfsrra.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rlgubrvx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2eqvfyixl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2prncclrc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xdcwabyt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfaxxdo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yqvabvge.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnajplvh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wkqugveu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gjduvcni.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jvutdmkj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2leyuigxo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dowvhhyu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ruglgxxk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tarltqau.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rqabqhjw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qocyyrut.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fnjdqbqf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ecssqdxz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2polwmnmn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dreqjciv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2crzewcov.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iqoihood.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qtkrsdyb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bzqfrlxa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ucvubvwz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rikxpzer.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rabchxst.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2aocahysm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2muaxspwb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lwmlpopz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkqcpnh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kxbstouz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sfuavifd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fpncbklt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2okvbfmel.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbfldmut.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2iiknzubr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcxwefdv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bzrfmwid.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2suvucmss.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ohzpvdla.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hhhtbvou.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cvlldvce.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dlyxjrwg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2gbrmspty.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ovefildn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dtbpczse.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wuitqins.html


<!-- 参考信息 -->