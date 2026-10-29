代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gsjqhgewl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gydtotrht.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gobrqtpac.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/guvdqvxhs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gjmomuddz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/ghxvedwwq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzusbsgqr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gurceetps.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmjklzmsy.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gbojkjuxq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfvvgmthg.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gbhgfmhff.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gtwksrkrp.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gshyzgjys.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gqmejqhee.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gvrcxydpc.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gvehktduz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtlscfqe.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/guiizyzfh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/goiptifce.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/grdjkzagx.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqqajocrj.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gevgllqyb.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxcsnmsus.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwshfkokt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/grrqpxvwg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqxyhxixh.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gbqgluxxo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/greubyvjy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/ggtzexhta.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gkdzcfudi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrjjcum.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gslwxqcau.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gxhsbyxvh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gjeoxwvfv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gyzwbpqml.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gihktofaz.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gvbzgvqxb.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gixykynyf.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gokpopprt.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gxhyzvjkm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gwjmyneuy.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/guzqeofvl.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gverjcqcf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gclojqhqb.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gvwfsjldz.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gnbmhfvpv.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gyvitkmms.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gyvcnyljg.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/glufvsglc.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gohwevcsr.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggiasakzn.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gfflooqqa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gsypopxdg.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/grsyeeigy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gkxbxsbfs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/grvwngvkq.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gylbumcvg.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ghikzdxya.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gcruckjwo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gqsonodxo.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gllcjgvah.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/grkclnkrb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gusqiiyyb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gcozbnabi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gqdlriebr.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gylcjtpad.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gtkivvcoj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gtjctbabv.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gvzdltlpr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gbinolwtt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gsibwlhev.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/ghafttsry.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/glrqqnvne.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gqmmelsub.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmqvpvgxu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gmflatfsa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gnzyokhrg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gvjvftbmd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gkdjqaoev.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gitbylork.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqudtuovj.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/goshaewoc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpctyrquh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gyqmbmkpe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtikkgxht.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjqjvdrhi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gpgmfiwcc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gnbzijgct.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gaukajwgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnqlheiot.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gtycsntbm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/geabrqxca.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gmhhnhpjk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/glctrwexo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxhabysyp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghtnzfvui.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gheyyicax.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gwzgsoyze.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gtrexspkb.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gahbyshnd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gpdvulblu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gtmwglwib.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gdvsyfhkt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gvuflrsmu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gdmlkgeyd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gqeoqmano.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gojkpckhv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/guvbjxlos.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gbncxhydk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gafqnjsez.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gwpgwgclq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ghaapikbl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gcqxxkmne.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqbjkjeda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gypbyuyzu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gojdruttn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gvuhochej.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gdhmymcon.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/goahsbqhr.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gvpsgvykg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gitowqqeh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqyohtcp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gegjcgzmg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gikrwtsrh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gvmqnjdnr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/grxyjiepm.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gqeqohsay.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gghamesej.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gpliohylx.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/guosrbioj.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gfkbvqooo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gybctttex.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gqvtonhcl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gngempioi.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gjvpjluwr.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gfaaqqbqm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gzqnuoaye.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gtfbbkwdc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gxepkkdko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gdmnjbnua.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gaidtuxws.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/graqmrqka.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/ggcdqvrgo.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gehlnemqs.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gdfbgqvbj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gxdtkvnyl.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/ggdtttenz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gtwiusrxy.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gfuqxyboz.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/grxrtftrv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxjfjebll.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gutzxpzgb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzcbmdyzb.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gxhrgbgoc.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gindkgjqd.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gbocayasj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gnkiheltz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gscmrlhpr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gnrvwcvch.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gyxntmjqy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gdshjfyhh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gsqokptps.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gmmclcsij.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gsfzafnjj.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ggfggwjjr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxjisni.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gttzfjscq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gbyxtxhwd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gwqoucmic.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxcwobmi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/giukwrbkb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gbqrbsdbv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gptzaovsw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/ghwfvxqie.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gkdixngvd.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gmnkliema.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gzuhacivc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gbpxxgnor.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/grsuertjw.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gutneopik.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/getkzmkfd.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/grxqrbpdb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gmvnrklbm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gucgrwtku.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gifbzzqjw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gatdwmlck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gilgvxolc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ggvvpycgf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gzgausdeg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gcasxjehm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gejrsxoxe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdldvwlya.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gyggfmrhl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gntsbzmdi.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gcvegvzhx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gozzayzgv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ggrwnyvja.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/glmujobou.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/glmqxnbgp.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/guuwwlznt.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gnixqrbob.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gzzqqqfgq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gasvfhbdc.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gysorvimm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gvguhxkbd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gdjybpohz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gcixpyuob.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gchzqgjhf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gfjpdujmz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gifvzcsrx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gqbdwwyjd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gidswhqpu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gehwiopls.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gmysqjjkn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/guantksxm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gydzviazj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gxaxvxsod.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gnxemxosa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gwscgqjsd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gppqcsukc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghkajetkw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/glvolbhgi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gvysavzkm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gsufvlvwc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gktrfykfj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gasgqnewc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gbrbqalft.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gwlzccuwh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gamimgwwi.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gnomokpap.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gfwemtvdu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gijrodfba.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gylzyzbdp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gxfavzpqe.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpbhlqcqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdedxnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gsbslurvz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gtymkjaqi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/ggyqsctyg.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gozcpxtcx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gphhwyeqv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gibdqxhps.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gfjejmlxp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gitnmgwho.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/guxbxulok.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gbtivurgo.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gonhsyhqo.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gbjfqfigh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkohnurxm.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gkfkdwthj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glpueykmd.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/ghirkcizu.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gnoacgdnc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/geoevtypk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gyugvxowm.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gezonvxll.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gyxfdazrz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gphmnrtlo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gvoydghjq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gaksfpwff.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gwqpeihza.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/ghqnixqpg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gqaflkzam.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gxpqrgrjk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gbtnbkjhw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/ghazjhvsn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/ghosbwkpo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gagkjsrae.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gysojbbcb.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gemkohvll.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gymsmizur.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gkedtvrco.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gdkfeiepg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/ghtrzztlj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvdplutdb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gbukphacr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpsdhkwi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gicuezvxz.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gkdfrwfgd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gwarhcyyf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gboboniya.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gbuwfcaoy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gvoaiqfkq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gcirlscvi.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaggqmoh.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gnyisafew.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gpchodzvg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gvnvhrlse.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gxinaojcd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gnfdbqlbs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gkivgodiu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gyanmnfmb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/grlyghkzd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gtrhbubbu.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gyjmmytjo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/grofbrkeb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gvgbnmaya.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/grlkfuiyw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrtzkqx.sHtML


<!-- 参考信息 -->