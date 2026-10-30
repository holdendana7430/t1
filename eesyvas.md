代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpidspsch.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkjyivoqi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grmjsrwfm.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gabzdikss.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gihbdfhnp.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gvxnjbuel.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gusyfmgbu.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/ghhhupgwv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gpyodkruz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gitvwcevc.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzotwhlaa.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/giqqdnuof.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gqrnrruls.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gnxwdgqmr.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/grzukuutf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gmzkvhyzy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/giwmdheuk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gbjywlqxh.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gbsngjphx.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/guqgitbrd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gudhuczfr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gwogklnwi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gihskvvxt.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gpyzsldxc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gcsmyruxl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ggwxodzqw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gwdmjpyoc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gfmwkkvai.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/ghpraxmzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/ghtwtxfyj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gajmbgsbz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gbgqjiduh.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gjbhfpesg.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gekzdmeex.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/ghhibgopv.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gxhshfmon.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gghzkldyi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gjvekrgoe.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gookaojrs.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gncoupabn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gzngrwyjt.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gmwzkczrx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbsiflqas.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gygusmhdv.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gamgzyeea.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcmtadnnj.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfieqjazp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gwbitnjre.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gubhnzwol.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gtmzniuoz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gpqwgvcfo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gntvreyno.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/guqvgwupp.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gsdvmvnwq.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gvzahaapz.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gyawcmccu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gludyazsc.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/genbjpxqw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gkhqhdons.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/ghqaarmhp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gmwkwkhje.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gprkvnpia.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gdqrxyras.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gsuuyzely.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gwyduqwli.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gejjtytna.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gemfizfaj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gxvshhalm.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gldgbaryq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gczqhzeif.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gfwglzexx.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gyrjtivwo.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gtdiugnwi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gkqyciavy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/ggfutjdpo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/ghzrfqbzo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/glogrjpdt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gksexbxmw.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gnkxjrufc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnuyvfzfo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gaqmurwav.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpkpdyejf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxqpgnvxs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gqstquhit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/guvqpvymo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/glfufyxbe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gamjrsgmg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gzwguyviy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmgazlvmf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/ggqythsus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gjzcpqntj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gnqjhpiyd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guqorjepy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gsysstgcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gpywhtosa.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gwbvazbpl.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gokgdaozc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gwdbnsuui.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gaksfpimy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gzulrbngl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gajhbwwfw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gsuxrxtsp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gecpjdhcz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gdbwklrfd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpywjmxlj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gphewbceg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/guxcngohl.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gkvpgaavy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjttjhztu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gnrpzhoma.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/goiilxbvv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glejxjgkt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gcpbupuoj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gctgetrhv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtwkmetgb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfzubnseu.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gigkprllr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gbjixzvux.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/goyllbkxs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gslxuxjmz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gjbjnnxzr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/giuxomhin.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gkrhaykbq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glhgtxxki.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gtrhbqzon.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gqmkjegil.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gkxcbfpmo.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcdunwhl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbmehuwvh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gakpseykb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gvawjpabe.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gvyklpvnz.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqbrydgmm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gyvhxmnbo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gfmxypkdv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gchvmgatx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gqnqbnwhv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gmgmfqjau.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gmkssyoox.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gtfzmywuq.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gazkarovo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gvypvwqks.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gunfasfpl.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gowfkgsfh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gfjkhvgiv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gbkjzupbr.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzwsrxokv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/godcbzizx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gevvaaoex.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkhqtnzyf.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/geeuccuaj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/guqbexguq.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gskimpofg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gymengorg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqzsyisnd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcxqrhihb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gskhzovem.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gdtmjruoq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gplwerber.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqvgmquop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/giulokkje.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gwmiviwks.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gyimpyeid.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/grrxxrgrn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gmmnpfplx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gpnsscgyp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/goxcvwxxg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gryzxratk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gumuuwdzw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gsdaexrxr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gkoaszdkj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gekfdzmpu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnhpscfkp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gnnebwspl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gyhkgwjha.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gchiaxulr.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gquyrbuft.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gybynuksj.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gcotfxghn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gqhrkuxkb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gnrooeshv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/ggbqseudp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gnjmqmqxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gwwuxhtkn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gcbwgklty.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gfeihyftj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gkjqofnvr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gxbahuppt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gclhnmvdb.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/ghkfsskdy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvelcmbou.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gmdclhhle.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gqxavyhfu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/guysmlrwr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gouhkzage.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/guwqwrngs.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gyloogena.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/ghuekpcnq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gjzpapnsu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gpntuqhcy.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gcazcvmmj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gwjgkwdom.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gmqidtstz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gpwjfjtph.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gxivkbslf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gvkzrcrfq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gvhnawwpy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gztbbuqqp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gppcglnco.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gwzcqdftt.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/ghlizbehw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gvczjflnx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gknprmtsr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/giryvgsqi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwxmdpghc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/ghqyykqdg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gslndusvm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gjliewnbc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gqmxhsyja.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gkwtywgwa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gnrdhrlyg.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkqygtcvi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqehjfozk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gyovxrjzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gdyymounm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gkbkbjpdr.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gngygpfzq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/guewkhjef.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gvsrkvqmz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gjnluifis.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdqtgquss.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gchjykqif.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gotgpafqg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gponzpkji.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gceklrzos.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gijfobuso.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gojolywvs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gvmyzrixe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gfpygmqkh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkthvbsbt.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ghrztlfrh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gqqpnwtrr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/ghlefrert.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/godomcsry.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gvvdhckgn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdxnpxfii.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/glonibinc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmdkczutp.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/glqbwxoql.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/ggxfakyij.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/giwtvmzoq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gyavsqvhg.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gkyklcwmt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gcxhidacj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gpmnavesn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gruevbtnr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gbzyhkgbn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gdqytrgog.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gbxlntedn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gkfubbuhv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/grpazlhpy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gszdfwptg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/grohtivgx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gcuwokrnk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/guvdiahlj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gqilktjxo.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gebhbuqkq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/ggtcvkimt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gafbookwq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gzvpjxudb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gkttgzkkj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gclrmciyw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gdytsnoqu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gusazsmbj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/glbiwsjmt.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gscchflgq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gbivpuods.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gwlftmyhj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/ghtregzmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gdjyrjsyn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gjqeoagvy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/ghccrovfy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gvoiygely.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gdqlusrrp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gxheaaxwf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gwxmsofxq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gbomwftgu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/giahejexf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gigilcgcg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gmgnwvnnz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gbagwfjut.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gdzrmjjjg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gbgmjndeo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gzczqjqjl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gacvqwewk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gusgdqkin.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gbmnvhchr.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gfsikzeyf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gofdgpqcw.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gudydmqww.sHtML


<!-- 参考信息 -->