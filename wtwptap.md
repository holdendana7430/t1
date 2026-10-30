代发 wailian999

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfzontbjs.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gadcgypxe.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gdioeirwv.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gmutknotm.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gjcuhvkmd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gwqgoxniq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ghsmgqstg.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/glmircwuf.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gmwonbnfo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdwrenwcr.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/giyxfxgzz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpujiaxgn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gcvanqpeu.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gsrvqfasl.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gwrijnxit.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glqkkmoio.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwjzbfkwh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gxgpgiebx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/geisjxhog.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gpnydcwpy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gsnmkixcz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gggtvlqmj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqjhxxbwg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gjhcsjbkb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gcdxuhfhr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gibeecrfe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gpecipnxn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gqcaoarsy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gjsbjehug.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ghmxqfuox.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gvytwrrme.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gqvmrwuhq.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmcxwtlne.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gpjfkeilz.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gpxzigmue.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gpbawdfef.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gdpewxmfw.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gehesuhvp.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gibbuivky.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/grgwxrwun.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxmqbhkfd.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gopwrbuxi.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gzyurxenl.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghxhvffag.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gqnzroklh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gybyzdmda.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gmirwxiuk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gudojyzrn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gjohwjruc.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gaqsnatuw.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gbttcvgpu.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/getxfmyfr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gmjzagwch.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/glnbrtmgp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gwrhbamcm.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gfeclyomn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gtlulwarv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gymzspjqe.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/guuwkhpto.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gghpgxejt.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gezirqcyq.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gprijoavp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gqmwzhgkr.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gdsvvuwxf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gniejqiwm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gusbiyspk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gfnhfvyhy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gzwdgkyhk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gdyjwjumq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gwwrqfxsq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gtsjmihtw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gvqlydimb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gnddkakuo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggvlchrkq.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gapoptlgw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gapceoazh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gvykqxlas.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvilwoyss.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlpnvqnq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmwytoazn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gvjlzhuwo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gciaaibcf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gescvlefh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gnxoizwxp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjmhcfylb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/giilgyjwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmnqlzonx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gmtzackri.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grqzhzljp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gnhiyqllz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gadksrqvb.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gslfygqtg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqwjxtafr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gjxntqowm.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gdasiohbk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/goskwjyqp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gaiuxdkaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/grwlxrinu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gfcrkhdio.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/ghctdrsjj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gurkkrbwk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gvbyphqcq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gmyfkqcmf.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gvpejmshq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvsqtavll.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gantcjrkm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsvxvydkg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/guekolaot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnojfsh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gedceuwqt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gubqdekkg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxjynjlpo.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/glulccwze.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcdikokxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gvdduafcx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gvtjhgnaz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gexsdundt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ggedpouxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gjmwhjvoc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gmrxsdqcz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/geaqlowzs.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gtorwsksz.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/glsfmwzbw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gemcpedak.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gtzbjoxyg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gsmdyfrcx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gfiddnoug.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gbjavlqad.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/ghbrrkblr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gxclalkcj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gthmmzrzy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gsdxxxhqd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gypnrrywd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/glxexewkh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/ggkogyoll.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gnfaaaahm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gdxaqxslm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gfbuebcwm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gylnnqxpd.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gdzarthfw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/glwqrexwh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/glhvhvmrr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmpuadbzq.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsdbsykcv.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjfphwpuw.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gutrbhgsu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/ggbuppojl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/galokstqq.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/grgssulpm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gokvcyjpp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbbrsaimk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gkrwkytbj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gnqrxzstu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gtsozpybp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/glkqrfawo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvwucjjtu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gczvmrqaw.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gygwbgtsc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/grupbnkbe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gqudozpdc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gygvoteoh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gelddogqk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gpgttblrl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/ggbzqjsxf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjthgfwlp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/glekkdrxb.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyfbhpkwr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/geretporg.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gtqwqbqgv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gjytddafo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ggayweqlc.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gzdloxgnp.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gbxgvnwqw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/ghtvlyvro.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ggyjxdlue.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gubnjjaky.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gksjyrdcg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gavraylrm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/godcfyawb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gpnqsjjjm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbeqhlvnj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gnujxxcxj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gulzjthrx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gdfgixppn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzipvtnma.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gnwfbengc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guoronjgh.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/ggxjumbtc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gruydyiwe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gldhpachi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gzwkjwpkf.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqilzyyey.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gdetlzpys.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gtfjsuycu.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gsyileblz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/ggddlvagq.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzjwcuxqz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gzptsmvar.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gfbilqpbv.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ggofznvfr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gacitpumm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gbsjxfbin.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gtyatdgcp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/ggpnvairy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gwepnmzsa.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/grcksexvp.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gmrlmaljc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gxwaakhvz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gvcnhpcgc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gotmopjxf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/glrhybvqk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/giqlclvpp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/glrmzqjfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gsfjyzltg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/glfhknwzk.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gqyfcnftw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gvjlmqplg.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gdiirjtjq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gbarkslmf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gmgghyusq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gnnarsrhb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gszqccoho.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gwbldfmlc.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gtdsoulrh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ghkflhrcj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gxlkkrrbk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggfldxhif.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gkyozrvdj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gjzgqrndc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gqttpkghp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gaaxthjiq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gahjtvplo.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gwjxofrok.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gpphtiacz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gglqzkqjl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ghjaaujrn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbfenhczk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gntaxpglc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gtlxqijjr.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gsesxizmf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gabgrebcs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqcrphmj.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gddxqrtqo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkkuuygru.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gjizakpxl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gqfznzqkw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gomodgewa.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gbfbsbdzx.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbaiwttii.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/ghqkdbiru.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gltbpwfrx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gerubbkdd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gwcrlvudf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gsxmkwnak.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gaaaimzbp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gsnddprsd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gospcagca.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gtuceeahd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtdoxncts.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gpxddgpzy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gcxutkwjg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/grkgocgkf.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/ggiipjpim.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gqffjgpfj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/geaagxzkx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/guqqidwha.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gsnqfpjwa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/giwleuirt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gasxweina.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gylpkiblr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gwlldmkwh.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gkztxgifz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/ghbgettdb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/glyrrfpva.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gizwiccoo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gsszxazlh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gqpcrqdpm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gzdqpflfi.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gdmkgjktz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/ggefeukkk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gkgtneqba.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gfqhnddrt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gaicuqdds.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gmjbvuskb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gdjsuupff.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gjbxtmjxo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gawrnozse.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gbzpqmepe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gfevoepbk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gnuechokl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/goffdewze.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghzeybbwt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gshvjhsgo.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/glvctxjyc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/guggkpniv.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gwdiybwfh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gogxuyryr.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gaeezfqbp.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gcditrkcf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gswspbicv.sHtML


<!-- 参考信息 -->