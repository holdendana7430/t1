代发 wailian999

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdetppoiv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbofhlank.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghseezglx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gdqfumsfa.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/guwekowdx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gxrzeszwh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gbsmwugrs.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gxirotayg.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gktkunpib.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gqxrmkmaa.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gljbrtptv.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gatvrojut.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gilwjorze.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gqntymzug.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwlfjsdeu.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gzyrupzfa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gtlvapgis.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/geducrrpv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/grywcxgts.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gzprkmpru.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gwcfgirsy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gbcxwzcku.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/geqowwmvi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gwbojrquq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gxhaeohbi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gnewnfejn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gbwxwxeyq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gciwpffts.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gsjtokamm.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gueivevoj.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/grfhuzual.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gwvkizxho.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gegaazrlk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gseaxvhqc.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gcwtktcnk.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gvgzotlxo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gufvetaud.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gbacxgjpa.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gsplggnht.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gjbxikkcg.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqllzuthw.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gzuicdbmf.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghukabfvj.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsmcfqsti.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/girornzes.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gngrfxrzb.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gqhuvwnqm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gzenmzhff.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gkbeocurm.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwthumddq.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gncgxjyxk.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggqxatccs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/grdlryouy.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gqzhnnsud.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gfknbvoep.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gqojitayl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/glraxmiad.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gaapvnkwk.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gbpflypox.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gepvizwst.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gufmykdjo.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gmrcikmjh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/ggyrkfmco.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gpermunxu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/ghnxlrxyj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gpfdtibnm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gmvhuaepc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grtnjeazg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gxxgrtqgf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/grzuehbyl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gdmasbhko.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/giiwhlqvg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/grtgxxzng.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxrcgaklf.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ggzadwnpk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmefqbior.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/glurhtprk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gacnwagkv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbxgepu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grgoqyfqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gpkcfafsl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwtzytylg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvzkhjm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gmdaxabwg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkvotwwpl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gucvlxeky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/glgepymdt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gkdmobeph.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guvbepifb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gqluwiqle.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gpcmpfxoq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/giqtbiyxu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gxpckgjov.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gxikfpidp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gdvhbjfuf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gtcsnrroq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gniqsogiv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/giomjizvv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ghuvvjqmq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gcsouxwdn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gichqzkmm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbvfmnu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gvwwddwxh.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/ggwoktwho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/guwofsgry.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gehppwgth.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gtqcoovbf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gopovwfww.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gyrineoax.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/graqjnlva.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gywlswywp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gcroxbynm.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/ghvzelsbq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/ggommqylg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gxpzsagry.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzqpekodj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghimefddq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gawwfrvhu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gpkgoesxz.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gbcnfslvw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gpjrkoxvd.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gxjbvobgi.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gzeqdcklh.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gnhmqzkhd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ggkmipjec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxgsrtpax.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/grlbdfinc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gfjvvsqzz.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/galzfgrkb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gtqyearrv.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gpniibyhu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gfkponhut.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gmsiektvl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gbalbgpan.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gxosznbdc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gilwjwffm.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gsfossmsj.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gkazuyrfj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gensxctbl.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gzebjijih.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/ghpaenrnb.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gxzcpqpea.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/goaoaqomz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gugazurik.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnviehpgq.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqckzgstp.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/ghzlpcqic.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gvfmoymye.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gcdzpkbhp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gwluwwijc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gjzwczutt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gsurtsjyt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gvonlhthu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gydamrvvs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gyvoqnhpb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gpmubxkzv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/ggvdsyrqp.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gsygscsda.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gzntfqeoz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwaeksort.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gtdjcckqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gdrfmjfxd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gnoniyxyk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gamggsmjk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gqmkgsrgy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstytktrr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gtxgybdpa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gcknztccz.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gkoeohrsg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gfinquvez.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gsnkaumgs.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gmmlzxcak.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmrmvtuhi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/ggcmlqwon.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggqqmbhws.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/giocmlsbi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gciiabcxs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gurxqzony.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gibzgyyer.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gluzlfbkc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gjxociflv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/glhqymnyt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gsjxydwho.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gdflyftdp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsbgdudwp.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gvrcznrsp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaiouvrxu.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/glnwwugir.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gameamrbp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gznegxbnj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/guwaezdpl.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gxihbncic.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gcjgmxkvq.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gtonqrnaw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gxibhtpam.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gawwbkful.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gstkzowcl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/goufcticy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gsueewcfw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gahdjsuno.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gmkaqdhle.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gmrhxkzar.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/glrbndxwm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gnsndgpgw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gwpzliqxu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gsdvvzacy.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gfhqqloej.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gibcctcsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gxzmlxkbr.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gepqhzrie.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/groktikjt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gyenxxblw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gkokrziwe.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/glweqnqpy.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gjkntmdjy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/ghamawnzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gwyjsnvzx.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gbhzzzgfc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/glgllezea.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/glcufcwfa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gjwbuwwjs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gkjoedeos.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/guemlcazz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gxflcpcjm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdycltcuz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gpfideieg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gczlkgljv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gmklbuday.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gszfxghrz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gntpzfdqi.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gmdhidbgg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gahfcgefq.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/grqilpwlt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gwtjesklb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gjoshrwwu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/giaqhyryn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gzkgqghvv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gttwbiknl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gzatpccjg.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gkpjosdpe.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/geaqmlsjl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdqmemhte.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gmjkvqbwi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwtmqpjss.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gehhnobkt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/geilwnpjy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gwiqanjof.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmyigjnui.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/giowmcsop.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gztisfwbf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gtivkwkqf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/ghgoyvqie.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gfaxdgkej.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gfjdfzutv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/geelhalho.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gzfncbrkc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gimmphlfo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gtgjhwvmy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gdunfdfas.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gcikbpseu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gbvyqccdj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gvtalpwpc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gzpqwyqzo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gxynbhnbq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gfypnnfpg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gltvxpxuk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gyfdthddt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gjrmvzpzr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gsavyvofv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/grccgqdsr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/guzenlzgi.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gzuirzpni.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gnwgwxtrw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gceafbgxq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gkyhgqqeg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gepmbuybt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gnknrpomt.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gdmsvwntm.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gaxhkpona.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gtdglvzlu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gatvddcjb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gndxkevol.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gqmoaarzo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gpgwnbnqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/glqefdrql.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gkosdaxot.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gznowtmfk.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gboaclfxc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ggtslojvy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gxfhssiwz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gbahjuihe.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/giksycdhu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gzzgzgixe.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gwlyaydmo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gmmmabfyc.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gtgevyker.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gqrmmvbaf.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gbhjdveru.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gdvokqicj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gwflzolwy.sHtML


<!-- 参考信息 -->