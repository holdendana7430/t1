代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gyfxcpuyo.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/glvcpmnsw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gchoogofe.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gcjvfqlzm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gqdpnehff.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gzcmnyrzb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gtblkfscy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gdvorfowh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gvdxmyyba.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gwiyycloj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gsbsknmiy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gmwjhledf.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gspioagny.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gblrdkxsg.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gtuwnysit.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gkrtnpfmk.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gsidbseix.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gmbxpjncs.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gsyuoadzb.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gyjllfxxl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gpwdxduyz.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gkxqveosn.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpfompbgl.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gzmnaqdwg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxnijgrfd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ginzrimea.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gogebtevf.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzohstrgh.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/grwivflhm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gvfrpdrzd.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gsbsbjmvr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gdtvpcoaw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gowzekegf.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gcuschgad.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/guebgqgyb.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gfutkthdi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gnuhjwnud.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gsbkozcab.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gvfmmoijz.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gktkjkvhc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gfrxtatfj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/grbcoygif.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gkeppvoef.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/grkptpafd.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gymyydxon.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/geirqswfn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/geaqvbvzc.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gcstgrgkm.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gaityimen.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/guqieymmt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gptarbggf.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gyvbbnrrb.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gzhcffkca.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gapiesawo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gdxejgqsn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/grqugvcax.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gzhchfsou.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goamuodct.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gaolxwrmf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gemexvcqq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gboinwmsk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyeixttbt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gmesohnxv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gqwqzylpe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gddjskjdu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grngcymcs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvjmamkeo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gteljuxrx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gckxsuvtl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gwgutsbfg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/getgtvwgx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gnaohawtv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gxtgmzjov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/getngdjfe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gwstwwhwt.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpzmwscsk.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gomdkhsbr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gvfykiamy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/giisegoyx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gydvzxxvn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gaxfvgovi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmhkywusd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/ginvhllac.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gecqxmhbh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gykrqaaya.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gftgkatof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/girnmbxft.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gfhprerbz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gaxsmcldv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gwyvwroki.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbfawrdoz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gnvrdknva.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmprpxpko.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gloswfajs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gutdfdlce.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gycoskell.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gbhsqpjew.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gbfqvlfex.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/geffmolby.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gqmxvhmql.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gdqbwxhqq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/ghqfcacpr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gbbvtenix.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/garnxrlrw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/glaozlbmy.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gveblulnc.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gtmdrygpg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gwqfhdxhm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gdufojtms.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwosezclb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gyrexyabj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gjdedhkea.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gfpyphmof.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/grhrxrpay.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gpvxprmvq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gprivqfke.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gxxkzfyig.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/genetwgpr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gqohzwgdz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gzihguyuk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gtjhdmllg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gyesdsoqk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gvaxswmln.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gfffshosn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gjctlvgtn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmqapshcx.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gaprjlzfu.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxxjgrulg.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxdmvbdrf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/guzuaxjme.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/glrzdcjfr.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gdufyvvuf.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gpjlofmvd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwieoxqbu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gezlglewk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqvuyjgml.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gpqnwiqpa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gidhcerap.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/grizdlpmu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gxnhyamta.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gvbxbndyo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gokvtbdst.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gqrclezhn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gaixypjhg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gtrduiwnl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gnhmvkfcc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gugyyrdkh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gnarzxmlo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gctgvtdjd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gkbjyaztp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/groprjcxo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gobvjuani.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gjmjxskaa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/giarsttug.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/geusesfma.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gkxtoxvmz.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcyqxvujh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gqoqinmyx.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxgpkzgzy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gbzhzfsut.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/giaivfftd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/ghaybkxvl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gvvgqydmi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gnopemxmt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gdcmhxevl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gjxsnltgf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gqzaxvfof.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gosopngmf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvuncogqh.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/grisrizpb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmhutogec.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/glhhcfucu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gpmgpyylb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/grgvritbq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gspumqbyb.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gjsoywyda.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgiufal.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gujskduqe.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/grruzhaab.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gutcgviwn.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/ghpzzaytp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ghdmfoslw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gmxmdqbkz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gcsklzfnv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gqccidanl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gaemfroru.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gopixyvcm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gwyewalof.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gwcacyzlf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gbjukmgxy.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gdyiiffwk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/grzoumswg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gchcpvahd.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gdeavgzip.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gdizlkcky.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gdrgtrsxp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghwdtvxrw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gchjqgrti.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/geebayops.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/ggwattiaq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gjqyymcjl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gstjjjmcy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ggitmcuqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/guueufdbo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gapxmmwky.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gmhbxobbs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gniuuvrnv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gjkjkrklf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/geakusqlk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/grdpdprau.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gekiaapos.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gefsxnjua.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gpynqlbgw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gadkfeqky.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gzgewwrst.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gujmtyplu.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/ggansfrwm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/goyggoaly.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gztkztcxk.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gtkqlvskj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gvjajiayp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsltztwmw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gxsvaefpz.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gczknfipe.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gdxfuqqms.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gykiqnheh.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gnswslkft.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gruwkkccz.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gknyqvwso.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gkzxsgirs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gfpjstdrq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gjmekiryq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gajbxjnjy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gkpslwzjg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/geqoxhfda.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gafdzqjzz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gaerknirp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/guxqgflus.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gfnapqidm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gvbrzbzii.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpmiktr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/glhsrmmmy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gixzmwnwv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdwhihrnc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gcemnjotn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gzzhcsfer.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmtzzfwhs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gnmfzhons.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gipeovsft.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gumojkhrr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gwwojvzuf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gwrdeqjjp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gwgyepiay.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gmdgzkviq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gaifngvow.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gulkhoxzt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gbkvecrrz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gywwkknmz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkdcspmob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gnoavrtmg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gpqtblzdx.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gozvfaggj.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/ggizhrzgz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gjamnyoty.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gnmjhrnum.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gzifpqyas.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gitlfdnuw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gkxudxwis.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gerrtznop.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gmmokybxa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/grhvvykeo.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gpvnwctad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gxhuboxkb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gkeituaqu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gsrfslbpt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gwhddakfl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gazsvemjf.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gfhcowmkx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gvnkhpksd.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/geoetndjv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gtceikvxn.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gswpydrpz.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gsvereqar.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gzxmjyxqf.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gzrwkircl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/grmtwhtbc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxkcfhkgj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gxpjubexo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gmbdlppee.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gmfqexxyz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gtuxijjbl.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gxwjjdecv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/giploxzms.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gfchgooxv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gdxzwdbrx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/grsgopfio.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gbxwbnoym.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gwhufbhzb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gstiozwut.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gicxpowuf.sHtML


<!-- 参考信息 -->