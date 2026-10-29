代发 wailian999

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gsypdbtul.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gdvisdphj.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gwnikxobt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gwflfezfy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gsibtplmo.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gficcivwp.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gescozcwz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gaqyawymy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/ggidijooh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/glavqikcv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gnnlxgefu.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gtdmqxfkq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gbwkhifqa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gzssubzyq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grhwkykdv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/ghpbensqz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gesenlkmb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gbpwtxreo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gxjgigjab.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gojabupbl.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/guhdxvxaw.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gmhzzfstz.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gpbxrfkyy.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyehlycsw.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gzszzrumb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gpobjjyke.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gzxnlmayh.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gebknfzsf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gtbjgcgji.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gjfaywflh.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjiascfaq.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gurqxbdnz.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/glshxkedn.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnjstjdxl.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/giucasvuk.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gprgliury.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gflsfhoma.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gkmbcasei.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gsbswknor.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gzkkdaifs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gbpppiuij.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gumdtonkw.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gqrscexxx.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gexoefjsi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/glyxezewz.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmcgphx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gusilnuba.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/ggucoghqq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gkymuxggs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gevxarnoj.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gkujbbnag.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gawvygxqg.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/guntsynfh.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gpjmxnalg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gspfbgwgm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gzdbewvzp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/ggfnvhcgb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghobldqgi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gzckwofar.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gaykpskzf.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfbeosjrf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/grdbwrefd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gtijzvmmv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gnnnlcbkb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gfuviolid.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdyjfucnp.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gudytglbx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghmxdyaok.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gdkqjjxov.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/goovcrhbn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/grdponjrq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/guohrtoxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ghokdudjz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gdtvrgenv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghofdypvz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/grfkinses.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grwhnacto.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gzwruwing.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gcqgzzdhy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gheblivjt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gudygmnbj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjadcqqqh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/glrsyeftk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gakykywys.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/ghkfobriv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gmrropjuf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gxzfhboug.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gtrwksihi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gdzuculry.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gjyvonphv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/geaxncoko.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ggvipjasq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gsbizkokh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gwlftjfme.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gfywumjcl.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gvflljuxa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/goukkgpux.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gmhjnovbj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gpvnuaddh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gceqqxspp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/glspwkonr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gxqwttnya.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/guezuzdhj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggcfbxltk.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/ggnarduvt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gtlgghlxq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gwdwlbhlk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gzutxbzcn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gfdsorbyr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gwomxxmmx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gymgmznti.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gmverwquc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gwncgtmnt.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gzkpcwwfm.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gotrbgong.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/grbtwpdja.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gmaihmxhz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glotiyaxp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gkotjmbnm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gwogcgtcu.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gvqeonkii.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gucgjossi.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/guoemzdpr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gppasugnl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gtymoonle.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gizplohqx.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gvqfaefwi.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gtjiqoghc.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/guvdjkimv.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gbgetpjvt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gbbknwznz.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gwlgxclwv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gorbxkexg.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gtmgrhhzi.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gusopqqhr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdhinyrbh.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gwhanfsxx.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfnezndeb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gnufodffl.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkdlviqmm.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gldxfsnim.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbthjcouv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gudnzpswx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/goqnsautc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gywdhakzv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gmmeqlmzk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gubcvsvow.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggoxlobrx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gdmsuakoo.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gsvknoxya.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gerorqupu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gqdjyyiip.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gzbmcecww.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gqadewwuc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gqldeubhc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gbqewnpbe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gpgjibfow.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gvdkukyub.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gikkpplun.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gnuctjwam.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gtdkgmtkr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gmvcjeqag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gburyhbmi.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gduqiejuw.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gehbhcgxj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gsinqtmuu.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggtevjdbn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gubkydoqu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gwapmyyzx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gordxxaai.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gwyhgsomq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gqpuwpwfr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gdohuqdgd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gmauyyxgo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gwumnpjtd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gaobweupe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfsxvfvmx.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/glfrjynat.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlvbeyhf.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/ginaadzeg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gdjoxritw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gnqbiwmtm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gmofnxhop.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gryplxnxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gyqdkcjyd.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/ghsjvycvy.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gacqxpkjl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gkzqpbtld.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/ggglcohdt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gkriobgot.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/glfxvvemc.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gszkicdwj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gevpycxun.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gjbgahunm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/grefbdves.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gbhuchjyz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gtsyeiszj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gviyraukg.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gcmuyfhpv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/giwdffhzw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gkmjkyzaa.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gadagumis.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gjmfnhvhl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gsfgmrchh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gmwnglsvz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gzatrrgte.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ghhefpmgc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gqiduyuub.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/grjualiux.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/grfcshtui.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/grcfchoaq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gefhaeqqy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gutuqbbgc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gjwawxyfe.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gzjzgllua.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gplamjgiy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gvmitymbp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gnylnrzwg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gurrgksev.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gxnkpbegp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gsnitehul.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/grbybsofb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gjboeqgtj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gpjuhdisd.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gejmfxbwy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzhmdqf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gjzmiopau.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gxdckxshr.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/ggzhuvwtx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gtgilgevw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gocxlfrwe.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gzibpvtir.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gxwzuvave.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giqpzwqgr.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gqhahbonr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkivwaoxk.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/glksoywis.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/giuwnpbas.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gzovvdvfh.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/guomrmwir.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/givystbmw.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gtohzivmp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gzuotiroj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/goxhzwabr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/groxzrrjt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gsafxqqvx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gnhxecfso.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gzqoogmsc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/govmqmfph.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gyyqprblr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyywomews.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/grwckdgsf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/ggvnzcnwl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gzutswcls.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gplvvgglp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gvbglmkbq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gnyeidruq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gwqeldqko.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gxpbajhus.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gayhwsinc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gfalncltn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gedpkxctb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/godeerbop.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gvlsmphth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gttkpfhqu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcypwvegr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gyjqgwllt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gsrpcytve.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gzhzsiefn.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gegrpkvur.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gsssbfcnz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gecxedfdb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gauhbqojn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/golwmboze.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gksbluqpx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gctqhydrp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gunjhrhum.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gaaygbpzy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gyjqvuder.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gtzzhoncl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gwghvtkvs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gzihizcds.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gsqmxeelu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gubccrulg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gwxxchhmo.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/glfcwsldk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gjekbybam.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/glxxxwcxs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gtinbkqfh.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/guoslzfbk.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/ghtlnzuyj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gcxktzlcp.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gtpdqwsxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ghhburlky.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gihvsvocr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gsczzckso.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/guaplugxa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsshhfpgf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gcvghdnsl.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gwdvboqoc.sHtML


<!-- 参考信息 -->