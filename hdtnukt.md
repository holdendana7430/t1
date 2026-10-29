代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/glkgljgah.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gchixzzvk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxilmwqsu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/glljpqhzo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gupaaosnr.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/giwehgqfq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjzhdpjtf.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gsvceazur.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gonssnzby.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/goskuslfp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gnwoesime.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gdguaozva.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gusodoafz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gmjfgxose.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gxixwjbbe.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/glyttyxiu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gkzzkgpux.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/glczxjrnd.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gzcidcxpt.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/giotpiega.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/grisxycjg.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gymqkxgzs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gqqcooqyr.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gmdtqumce.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/ggxrfwebg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gvvvekymr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gnxeblqcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gooqbigwu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gqsqxdlav.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gqmwftolt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gjzmukmdl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gyyvobylq.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gkrxnqjwr.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/glgvvgvqn.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gkwrjdjhk.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gdktubixo.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gvprhtqej.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gzqnbcgkx.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gktaugjtw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gbckxrlaw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/grhtjeljm.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/glqretybv.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxoarsadq.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gznuixfur.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gytwzqlnt.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqbbyjghk.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtyidsdwq.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gsdssnetx.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gkculenxl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gvohgtope.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gfubtwgvt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gkinycazv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gfbljnaug.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gxflvzqod.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gptuchsdj.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gvgqzcdzb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/golrtkpzy.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/glowygwkj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gxrkxjcvj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gukdzlkax.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gcpebuuzh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gbmrmkihc.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gsbzfwjfx.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/ghmrompfp.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gkwjgiclz.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gfrjvcnoh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ghkmnruei.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gscchlwap.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/godhskiyj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gqbxxiwer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/giqoxkthg.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcfsnmvhx.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxqyytixt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gnjspfmjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gyrcyknvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/geziqabxb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gmhhqiyhd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzqguzeip.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gulxdjfkm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwwznxiis.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gnbztsjxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gihdczaph.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gczppaact.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/giwohunvj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gllkvyrrl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/geejogckc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqpbriblv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gyzhsykvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grovjpfnv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gpadymuzl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gwdeqvgcn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/glkvigrcg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/ghwvkxrvt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gsgrootqq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gbkojmdeh.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxgmkhpqd.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggfotoenk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gezovytzg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gbzepixec.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gzctdpiio.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gjulyerob.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gzkcxtehe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbyhrcg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/ghthebcyd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gwqsmabqd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gzanqupez.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gqzcnunuw.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/giyknghvc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gyglaqhya.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gwcrjhwnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ggdoipmdg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gevfzzzwd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/guvqgheqm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gyzmvkvjk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gprktnlfc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gdttcrwve.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gtqvdinov.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ggudpjxri.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gddketuxw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gaetvgkay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gzbendvdx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvatfrxon.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/goofgfcwm.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gaszajjml.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gqsvpeixu.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gbjcmqbfv.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gsefrssoj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gdmoncbsg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gpqlfolyo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gloclamfq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gbyocxlpm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/ggxjydrrb.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gfzutaedi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gnmfbujhs.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gylzftqfl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gynwpxwla.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gzsdotlix.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gstiilztb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gdsgpyvnq.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gsqpklthu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gbiktdwwy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gsgkfrvwu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gikxqiefh.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gmxrkicfy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/glyglyinb.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gfckuwjar.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gqxounizf.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnfsgjiov.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbhyvhvyi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gaejooffh.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/ghtqtcybo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmndhvzgr.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gjecumjhm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gtkmdwghg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtmgvrsgu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/grdepllmh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gnddielie.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gwnauogqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gbjxjmikt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvvodpdfw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gnmipxvmd.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/guqjlglru.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gnpxoeomf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gmniznjgv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gbaixdfxu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/grbbylqob.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gmnbtxrtj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gsfnuxibt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gdnvjwuzh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/geccywgrc.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gshgctert.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gvdtppxcs.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gsobignnt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gnjxbtmls.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdntjwngo.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gspdwvvjz.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gsqydjpux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gnxgaiwbw.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gsgdjkccw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gtlkbxbwt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gkfeswnnn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gcqsqpagz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvjedcbhb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmhwbqhvf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/grigndmbg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gguotyfjn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gqslvmyqq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gosvjehmo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpjbsgqdi.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gygzycwaj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyqnjpjqu.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gymwurcwh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gnlpxcglm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/geknuduwp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gltkznxgh.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gmhpwtwba.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/goajgffht.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gpigalble.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/ghddqpxfj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gcilvqyte.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/ggdmiaygq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbselplrk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gumopnevd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/grhhxghuc.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gzeheimnv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gtnntkqoz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gcqdwebnm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gjkjivykc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gqrmozuwm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gmldqgjwu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gpkiqxvqi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gnxdrmehf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gktlqkpsw.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/giznoyuhi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gvrzbhjhu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gsexqofzd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/glrisxrui.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ggwondzfm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gesrhhnqg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gjcdydnst.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gmavjnvjg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gqdqtgqmw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/ghswgrwyw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gojjihmps.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/growpxaoo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gtnsicbca.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gxtwzgzjm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/goaazgdro.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gsclepimt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gnnfxgubd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcpxnxiwx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gtzzszmkg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gyysepzke.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gphvtsvvv.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gfiklpqru.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gkwvffaqj.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gsugnfmlq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gsbjckzrr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gvytwhsld.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gexvntnck.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhsiprw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gfvdfhibv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gdaswobuh.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gphhfsdei.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/grmhcafzs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gllnxkqkl.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gugwrlvhp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpqcsukpk.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gewlzctjj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gomjgvduz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gdnjfcsmq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gcvsrnzap.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtivflbwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gfmqltstf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gsyjqwuri.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/grbjxqpha.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gpadndrqn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gjwvtzhfl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gtvabtniw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gnueooher.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gbnarwbks.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/grgnqcnpz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gnjpqcapa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/grinibezu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gqfzibqvf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/guwsmgyie.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbkwbtzgn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gqqdspitc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gcyfigmwd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/guryzkdgj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gzylnwoqa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gdrolbwfz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gjhdhmswm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gikuqeaij.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gttiwttce.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gzdmoxvzc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gqbjkiyox.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gscpofvzd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gzdcayaai.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/ghcrtcmtg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/ggmqcthex.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gaqeiznjn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gfobknaia.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/goalsbpsr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gksbvefwx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gywllwgqv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gnygbzygk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gqsnunzzg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gotzegguj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gvywtrwui.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gteixrgqe.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gwzumrnau.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/godeiuhum.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/giyvwcptw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gttqlfntu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gssxbwoal.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/grofmxwzq.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gkxqnkmsu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gleksbely.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gqeuhvkzo.sHtML


<!-- 参考信息 -->