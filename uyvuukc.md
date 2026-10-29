代发 wailian999

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqummttnl.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gsmyqzpgy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gatrrohkc.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gefrnihuj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gkpxibjjq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gqgxgveeg.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gvigfcokw.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gammigqlc.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gvlifibha.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/govpbsjpf.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gbpxhqzrl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gjgtwiqxv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gxqikysqo.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gvnagertv.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/galoikdyz.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/guxrwhpuf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gxwctsfax.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gmrkzwnvs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/glsexnqum.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gwzretkip.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/guxspdliu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gyhmuqjfv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gezzcjysm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gnrilwqzz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/glfyfjddi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gvgezjzho.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gtvirajbb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gosxxbcjk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/glgaitebh.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/glcofelgx.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gsbkonsto.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gstctlodd.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gwaknajzz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gxhvdtbys.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gipzsmorx.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gwpbyiocg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gwmwaaqyg.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gdggxbkaj.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gnzmtbtaa.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/goxzrkldv.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gbcgcabkr.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwgnrvhuu.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnxbcwhrb.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxoefrwod.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/grphgxdfb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gbitywbai.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gvuebisuf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ggtmlntmb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gsaqtrigh.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gqhiloijz.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/geawpaudn.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gtzftaddg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gpdgvtcca.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gqzqokjgt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gwwulpkpx.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gntxufwcz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gduhqucyq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gayonviym.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gmejhsjhj.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gkniieflk.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gshrfgaqt.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gqaxbmgyw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/glwalvcnq.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gtejeahko.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gviqakpbv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gfejhbbfl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gpdhgfrjo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvormhqtx.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gtttmacll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtwoqqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gcahkhwjr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gcigydvjf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gdxisfden.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grlctnxsh.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gfbqdueya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghwgachxm.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gppxpolbp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmvmwmsew.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfekhaywr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gyvodpwoa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxlgkcpqc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdrdwceso.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpwdgtpnf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gaurrsyji.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gobvtlbeg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gspknydqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gvfsnphjk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gqrmpvmqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gwfwvqupd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/grtcsgvef.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gyeduldnb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gcphisetj.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gxlnceftt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gcxeppkxi.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gmqzqanvd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gjinoabuf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/ggzwsvpid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gtvhvwoyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/grlziyzuy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gsxxnokbl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/ghdprkjzh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gaavltdlw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gkdqlnpvm.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gyvqhfghb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ghfwkwypc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgeifpv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghhbknksw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gibrwqpft.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gdjgdhtdb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gftxvvjpm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gmnzvxwtb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdfilzfhv.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gkmavlegt.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/geuqbkmrv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/guyrgxkvw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gbnddnyvj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gupnnlknt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gkphfqczh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gadpstzdn.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gdusegyak.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/glrzuhygo.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gqkljkpjp.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/grjzcfbev.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/giporszok.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtbwtxkhj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxuevxvuh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gyklmnaqa.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gnwzoquob.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gvpqvkopc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggrpwwlud.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gcedfeyvv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gomnxamcc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/griulbgux.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gckfbaiis.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gfebasary.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gxnltrudv.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gvyzupszf.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gzbqllnfu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gojcdeevs.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gkuuhhabs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzujmtumt.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ggrfkrcdu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdlkjjuvx.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gptsvvbiq.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfclgrzjm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gukkzkqvw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gyvlpcgtx.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gealquapn.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/golwtnkef.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/grjocgurm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gnenbnxkg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grhkqovfp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gcqameyyi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gvhiztgzy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ghwppyons.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grpxdbfve.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gzfxmqqqo.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gzyqrqebx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gouqyhzzy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gtlnlyimd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gxaorqlqa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gfnnnhpgo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gfszyqkwe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gtsjvvgma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/ghgegwzps.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gurcodatg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gkqrtefuv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gkzrqntwz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqptbuwcg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gbsxrjekl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/ggutednsc.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxqcxlsyc.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcxggaxgf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/glrzarrbr.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gjtvfmxvp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gbdjrtiay.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gepqolvlj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gfyfsfqom.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gxdyaycae.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gkvuteojd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnqdopsqd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gsodcqccv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gliswzxoz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gzxxlqlgr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqoydrare.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gdvhaxulk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwvpzphsq.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gjxfywekf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gxoumhdjx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gfidisxiz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gwliawelj.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpzgiuybb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gcmkqckzo.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gvflvdsgs.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gxfcgsxal.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gnfcbrcni.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gnasknuaf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gwhbchoej.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gzvvkzgnn.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gcxbnleeq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gylrnbrpf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gjldgexvj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gxpmnhrho.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gewsvpvrb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/guuabmxcc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gqlqcqzxt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gofpfcncp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gvdxjphbd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gjeimublt.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfxfcugwj.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gggvtvbew.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/glfnchlop.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gatpmtcts.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gxinngosu.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/glaebhwio.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gngrcdtmx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gdderbbeh.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkoyqqev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gaeuxrenl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/goeifteek.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gelteirmo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gtxnaeaop.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/ghuaxwvng.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/guvjglhay.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqdljtkqc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gdljmkhjn.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gjfpdgdpn.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/ghmyvargy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/ghadzvxxo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gruwhtgaq.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gbyyqojcl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/ghdgqgmxe.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/giiryczza.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/guaflegoy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gbmjfslxo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gxsvksxmb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gyackfajx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gnkkypwfn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gkyrjmymc.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gujuymwax.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/geaoevlhn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzdlzvqud.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gwgmhcqxr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwqkzomko.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gaeqwgwia.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gpqemajrn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gbtqjtbyq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gzlvpeufg.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnljbcg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gdeebujwr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gquioiyru.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gpknwitjz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gvcqrmkdw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gtyrdqjls.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gohaviskw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gjfiaunjq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gotyivzou.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/glcquhhmh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gwzsytsup.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gdnaflqvt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gcvpqxhlq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gewesnnre.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gwwncnqrn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gzahsppbk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gvvwanjjs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gprwnzmqv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/geqoezlhj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gzmujhvxi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/grkingfus.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gsqjiahue.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gvuyidpfx.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gctcsdpms.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gdnjawqpa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxoxpfefm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gzrfqbdek.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gqnvojnrw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gijrjgzah.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gydzunsac.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gllazwlqj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gmcbrwlrp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/giljvagvg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gjedocnot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/guisseagm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gmfjybsdh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gvyqoufqd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gbkxrycqq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gleetrhdw.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gandtasgb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gzopigwlp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gdtjctgbw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/giqnxonkj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/ggenqhwzx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gdjcijbvx.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gsesjaxtk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmamydujq.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gnniwpzva.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/glbffwaol.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghdwxussn.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gxjwwiicv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gmkregikt.sHtML


<!-- 参考信息 -->