代发 wailian999

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjnaksjph.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gyjxewpiw.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gimuygtmc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gqkcbhjsa.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqzywdwnf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/goseecobu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gjexgexfb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqdgbvv.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gixlsfepu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfiouhtho.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gvdohcfnc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzlxjfnbj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gqcaaghet.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gctjshmix.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gxmqzuplc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwphwhudd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gsfkbpgez.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gzywvzkxf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/glvbjhnmt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gkntfpoyg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gnmzuazvf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gmxbijrmn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gvhgkvmvu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/goocjuxbk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gjlvxtytn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gggjkjukf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gdqjcfgvq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/ghblxnmqo.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gxwmgvpfc.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gqrkhjzew.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gwsshpfoj.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqnffwjfl.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gupkajrbf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gfpfdcgrq.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gythntorj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gapnvfxyj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gzyscabrm.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gvjyriosv.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghzptnikz.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gybsbwgni.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gecfqpptc.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqfutzgch.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gukawlwwi.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtnulaxoe.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gzrqpinlr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/ggaxkjhel.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gzalycbcr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/grnpeuxtf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gefazzicw.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gpnbjhmbn.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqraebzqk.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gynndztjb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gfpuijnoh.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gephfaxda.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gpgrfqrje.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gkvcflvvc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gsfbpykau.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gtmimseuu.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gxinrgihd.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjfcusnvv.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gajdqatck.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/goubcqnwg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ghgswqixi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gbkwsjpnv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gjakjqlom.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/ghxxvrovm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gylujnaey.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gctkbfvgc.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvkjmrhgh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gfbfkqwom.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/goctlqgrg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gfuqzphrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gisiwgbdt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwmercqmh.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gpbeadbth.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gomouukpb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/grossrdhe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkbykawsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqglwcf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gfefbmmfk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gduzjllja.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/giipduzcn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gusgudwyq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gvemmzoct.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxipyfbob.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/grwjpwbld.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gakmbrlji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/grmrtmdpe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtueliqga.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/galsibrts.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gaurfdjka.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gnljsdkwo.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gupcdxgif.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gmypbtlmv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/guusuiokb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/girdbrkxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gchyhrvzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gkrnegnjb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gusmqgglu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gqkilcuvp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gdrfyflwy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gzjzuqmif.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gcixypyyf.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gqxpboylx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gjvxhvxeg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ghkdupqqh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqbceozxl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gccqkmoox.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gplerjxvl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxqqxicp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gayvdjztx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gqpeyqktr.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gvstczkdm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/ggeqfmkgf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gthuzvpqp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbtawiidm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnqqafigt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/ghenjvjru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/giazvhgau.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gugqqgjau.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/grdqxqntx.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gnebryllq.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/goaoqykui.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gaotgtddj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/golzjcyib.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghztosvaf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gvkaykltg.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gepqxlctg.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbkmanfag.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gdywtwylj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gcynrywcf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/goqnkduug.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gaaqwntnv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gmwezagby.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gyuldcevu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gxbdbavbk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gpzeosxpg.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gwugijsuj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gicifijdv.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gxmajqmlx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gocckuqfe.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gdostfazo.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbldsmuae.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glezwlpxc.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gpsgyoics.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/graqnazwp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gvdqevhrc.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gciicaqwu.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gqauxcxjv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gngatypgr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gxwqmzirp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdvbhityh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gmjumnspv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gnjmjiqaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/ggjdjfuhr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqhjlhdmr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gfrrjyiej.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gedfrdofk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gsdgxjdfg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gxjfaklej.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/geocoaldd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgikthfc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gcqtogaij.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gozisyfjf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gkabxmyir.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gfukjsxkb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gdgswfyzn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gbvbjoqfp.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gseeoanpl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gpdufyrch.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gjreubsqz.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gmgomagmx.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gzwuuzxmj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gciiguwrh.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gienbxtfq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gcwriezzm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gvbqrfnqd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gwljvdffg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gkcmvshee.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gnuxjwgmv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gsycrebrl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gpzbsxzad.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ggrgmggqk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gxsfrwjzq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxtxreuzc.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/glqtqwhfz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gluyoukjg.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gchvpopfd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gairpqktk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gwyvqarws.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/giavpdozy.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gunnvktrq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gumzivtcy.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gcmynlheh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gkobqyjkp.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/grchzbxbd.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gqyrzqhae.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gwzrytlre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gyvyvzrmh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdpweikwc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gkdohjele.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gixdguamt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/geyfrltyu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gxbteovvf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gxsnhhhjz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gvlcniiss.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gunnupijo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gigsefbsi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gesduwqps.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gjbxabsjl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gjiuuddtp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/guyuaiyni.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/grnzdxbpe.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gveiuouqy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gnrjkewkh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gyioavrky.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrflzpb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gssjdvvgy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxksfuolo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/grctfmxgq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gxsajhubz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gsmtkqqek.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gyjpcbqab.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gucodyhfe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmqdylbga.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/glxexnxeh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/giyfoqzlm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghxlgbgmp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gdmlkyhac.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gmnomsgds.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/glsbzgeky.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhrnzad.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ghyyisjpk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gnmfmcbjn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gsfonhney.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/grjpcyqdr.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gwrjwjviv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/goznbyupv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gdpyakisf.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gsjvgplcj.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/getkqmwrw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gudavsics.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gcnzbdrzw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gskctibwf.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gooidfmle.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gmxtpktgk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ggbghgkdi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ghzmdzzig.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gshpeiyza.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gywubsapy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gaoaevnel.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gwhxyfujg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gsdznbxsf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gfsjuxtki.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/geqrqdlez.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gvesnuuti.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gnhiuxxzg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gwjwljtgv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gjfhrtxut.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/guuvyyevo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gbmumkmds.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gakkckotf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gkmbjnxtt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gimtsldfr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gxmwoxzoo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gmorpskzt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gblkaqnpq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjsdwuthw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gjlbtimge.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpgueog.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gztxjhsxt.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gtjzkqelg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/glclyeyet.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gjbiregqv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/glqgxjcph.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gazhtptgv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gmrtkzpyn.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/ggvnrmthx.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/giuaveqrb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gaqcgedgy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gsmsrceij.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gmylzsovo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/guupgizrs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gsuafjxsp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gbcypdfjv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gwhoqpsem.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gyxqzlrgr.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gnrgcwuyq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gvjqtjklt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gvvgtvrjl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gilorlnhs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/grqrdiokz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gdsttcuqi.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gqyjjssvi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gqtvdvrfg.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gpkrcyrmi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gwnydaexd.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gvsrfejyj.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gbiqmuuyq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gthhglpeq.sHtML


<!-- 参考信息 -->