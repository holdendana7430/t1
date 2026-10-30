代发 wailian999

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwockywmr.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gnesgjzso.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gvdjtfwyw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gcavapfmd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqrorswxi.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gtaehcqec.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gcwzxgfwu.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gmfkyxarb.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gesndpogo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gxdifcees.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gddkeifkl.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gsfzczdnm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gtmhqpkrv.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gvglimqua.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gnzrtsitg.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbtsmldjq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/guevvoeqp.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/grfjhlklx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gipdgttoz.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gjkxzfqke.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/giwtinsqo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gorqqxfbf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gzhbdeeay.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grwkicwbu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/ghaihqlrh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gejpnicdt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gftufixgf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gtvseocbi.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gbhojnnii.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/grwvcvhyg.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gveslhhqi.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/grlhkodin.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gmbanwrus.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gauliahfz.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gtesxodhb.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gouieufot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxmitatjd.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/ghkuhpyvm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzxoylhhp.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gthcitpzp.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvccgwsgv.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gkpyxfjmb.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbpvcazay.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gkzssqiyn.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gswikgryk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gvrvfwhcs.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gdxspqujd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/ghflhvyiz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gcrgsxfyd.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gvfjjzmqo.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gqsztppey.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gnlxzpakd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gkvpjmdqj.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gixalewzm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gmsdoafwd.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gdsecgqfx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/grkvaavgw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gqwfxdzvp.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/govqykzsz.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gnrvqtxqm.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gjiiuialb.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gavliwkfw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/glssybkbr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gosswphgw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gxuhtxfyv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gvbmfacmh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gmitsgwli.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gtkebdfrb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gxkvfzskz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gfahpkpqg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gzsmokdxr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gsdbwjzhh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gcnalwsns.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfvorbfaz.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gpqkiluyc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbydhskfo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gsijacgln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxstavtto.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/greooujcf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gorebfxqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gqatzuesl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gswlbgdnd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gotwvqujn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gtdnfftbw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/griyocjjm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/ghxtowyrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gambrtkiv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/goavbiles.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gkizcrnhf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdnsglpbg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/guvtvbsui.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gwenlinea.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvwbifqsj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gtccopatg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gtktwhgxm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/ghflgovwe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gzhcdxhor.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gkvehicup.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ggargjcxm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/godcfmssv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gsgaogtbv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gfqbghcky.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/glfvipmgg.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/glhzdedkh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gecsfborx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/grxejpxtc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzirejmfe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmlcpocbl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gapmuuphr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gejkbycjr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gvmkhckiy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gmbrycoms.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gfwwypvjw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gbsovmlai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gammkflhf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/glmzlwiwa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gehnqnjxy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gmcedjtro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gnoadmlmo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/ggbcxpcst.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gravwtflh.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gmnzwvkfv.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/goasxhbbm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gyksgfeka.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gsrnzdivs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/goqyrbilr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/guyzndvja.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gvyhnnoan.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gpnaemipw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gjwsodmth.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gjwoppudl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gtpcykwtf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gmmcmzmta.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/giiclstoy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gkzhipmdx.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/glcjjwotq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gdndohlmn.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/guovfdxkt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gpwkyguqe.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gkysdmnmp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/guotguesc.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gcbrauzpg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwrrooiwz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqsiczqph.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxlnwtjev.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfkjlhlwp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/glkfdtvey.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gyzwtscim.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gpsqrdugm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/guhjganug.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcgezhokq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbnzmcqwn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gblmjxioj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gynpstfpx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gqwbzlkqh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtunptfog.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gnzghuuev.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gjdquzqfm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gjkyohrmo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gtmlrwiqi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gvzglgxlf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gtnaxetbf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gsmmvfmwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gycquvnpx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gjazgzkng.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gxmftfzqq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gittsaokv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gbvyfyvxe.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/goquskskf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gfcadoyrr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gsvvycvvx.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gnghdsvwe.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gpnirfdsk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gjowkordo.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gwucablda.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/ghajuzntr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gohfdmqqd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gzwqrsyqp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gxomhtmtq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gnhytakga.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gqthoqozw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gkctxgnyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmxlkqdur.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ggcnryboy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdibzgprc.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gpziormkr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmxqvfyzh.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gqntedahb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gspssdcdc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gasmlwemf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gpvvhleko.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gbzmhjdfx.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gnkafylyq.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gjkuwapfs.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gylokxzse.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gnwfmntqb.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gwzgtfrrb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/giltaxbef.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gctaivawd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gcrmuewem.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/guthvwjlt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gzshzycxm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gwnblofkt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gbwznqpyt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gacklyxsr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gszehswfr.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gfwjmpubd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gwkdfwqlh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gqtznavsg.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzbeozdxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gizsfagxh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gybxxecyk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gavwqthhg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gqbkwearm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gigiuvppl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gbeaqskvc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gcdnntebh.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkrdozyjz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkuhbduzh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gqxjepvpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/glfggrhnf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/guaaulwvo.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/ggfzfxozm.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gwggpujfr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/grfrkwyyt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gowzulivx.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gtrpmcliq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gaiwqvtjx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gldnvyosu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gteesxcev.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gitfphwsu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gtxpefxbe.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gqtelnrsf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gvhtsvrad.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gwciyvwkg.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gkagjzxwv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gthaavval.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gadehvoqp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gmhkmigtf.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gwjrfjcgg.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gbaijpfcz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtywtwvfl.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gyddvkwfw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcmfvkwtu.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gzdnrjert.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gxeyaqmpp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gdjzwlzrc.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gdlwiizju.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gygudmfig.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpkzyywrx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gkslrcyxw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gmyaxojqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gcrptmnjl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/ggksckhuh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gztkaanun.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gchyckccd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gnrntauqi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gezqkiinp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gtcxypqmx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gxbdwebzn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gzvcaxjpa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/ggzjiitnr.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcqdwltsq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gqkvkbekq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gsrpkwlhb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvnwthxoo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gaxkunloz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gncxszcjk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ggmjhjobj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gxknrttyf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/ghqyaxpeq.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gwgkbqkot.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gxvcpnuev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gefnvltam.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmssboncl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvwfszpmd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gnsvpzgwk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/grildenyb.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/geipatnoy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpxlgehsr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gpavddyyk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/giottlvot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gdxbmwutu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gukpgejlc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gzouuiqqy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gkxrgdqvu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gserbarjc.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gopbzovru.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gegzqgdmb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gmthsewrv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/geonowfll.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gvcfyfelz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/ggvywccft.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gjcyfdkfu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gpflpjncu.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gfitbieav.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gawbpuwhx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/grepmuxbs.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/goxpixbwy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/ghsuunysj.sHtML


<!-- 参考信息 -->