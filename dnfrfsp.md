代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxkztktwn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gcstzzzkv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gdsaldumw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gvuzjijxt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gsugjegra.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gciuhxjen.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghkdopkdt.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/guclglpyh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvgjzvsxy.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gtowuqopv.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gypvshmov.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gonipbgjv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gibitaddv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gzjfzzily.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gzfkokiiy.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gjgmmskgk.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gprsbkeff.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gpqfosrkn.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gdezqmhsc.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gdahigdai.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gnlecphmh.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gwizlnsgv.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gwfoivyyt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwgiqwjjj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gqluttggc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gqdevsejd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gkxwkojvs.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gxewvlbtu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gqboofjng.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gexqbvkyw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gbsukebve.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gtiohbxgf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gtaazlrod.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/ggusheowg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gajgjwsvs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gifqwxcqu.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gqtihumrw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gmmpjyjgn.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/giqzlmvyu.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gfbrhisob.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gjlgmxted.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/goynygvsi.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gcokzzxzr.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gnomjtbts.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gisgympmo.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gbxnlzgrf.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/glkultpyr.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gawuowipv.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/guwhmnzgg.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gyujtklkv.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcusguwmb.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/goyoxknbu.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gtjnvbnyl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gelagrbrg.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gjblcxzrd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gubinygtt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/ggimjhffq.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gehhybnxl.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gdszrofja.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gakujtbyv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gxmqgjesm.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gfvjiynmp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gwdmbibjv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gmlfgeksk.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gzdlhqjgj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gwwsggxpz.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/giwgyvwsc.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gkixipyhr.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/grebjhpaz.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gmwthiocc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gvecfzhnt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gdycucuhn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gracfeysw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gjwlevxvi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gnpoiwzrx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gjdnqhira.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvuukqgmv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gkyzpibue.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gvnuyyjsc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gsxczpscg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gpkvpuufb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomdpzxce.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gqmjnmtyf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gofcyaqpy.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gczulfkdw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxelbrpbe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/glhzqeexk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gppapvsyf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/geaatuftj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzgrrjzwu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gndlzcnqm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gokejxfvr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gliyujzok.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gzrtsmdrr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gespyckkd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gxwbfyetx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gszagrujr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gzdybcjwl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gqiscppfx.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gacwsuqjd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghhqeurmh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gvgbwzoch.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/grwdiydxa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gjetpmyrx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/getqjfiul.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gvrymdaff.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/grumnlyol.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gxrwizuwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gexjanspt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gjucyvgaf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/grwlfgmtz.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gdoleizkh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gkctnsltt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gyobbbswf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghbzlvhiy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gpjtgodex.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gxffppghw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gncpyqvfb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gxmmjyzut.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpztkqsf.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gyzwvzcnc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gqeutttmo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsfexenwu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbitwavu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gipvozloy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/grviyfjuc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gsmbdjiox.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gjrnzcity.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gpaocuzsd.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gdbpemojn.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gildfjuhy.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/glnnssvjw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gudljmxop.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzmgixmhh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gokmjlrwo.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/grfmusaen.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqqtedpfg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/glmqqyerx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gbnlecrkx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/giodumdzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gezsmwkvb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gpfluyhdv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gwpstcbeh.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/grkolrwnc.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gsozaoufb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ghheotazf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gappitpzm.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gfrqkoyao.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gwsbbcyck.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gcrzdxjtg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzaknepin.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghmoqdhau.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcjnhezwu.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzvtjgddg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gxdfvztug.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gynybwwvm.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnreerkvq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gozgfdtal.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glchdcmzz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnlkjqogj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/griyplqmu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gudacrpws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/ggfustcra.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gamulqtwr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gdtghnoce.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gomfkrkhk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/goffansuq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gkjrcchtq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gybxfkxiv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gitpwmjar.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gbcknjngs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gagodaocg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gplkdgdqi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/glzmcooly.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/ginnppozr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/guvxzmhuq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gklngycip.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmyiwslzs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gaeziabwd.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gbseajlud.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfhzvqzgi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/glhecqpgj.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggabvgiqr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/glulnjawl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gnluwaoep.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gfzrakyxq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/ghrqmxsfk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gidmyzqkh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gsnoabspn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gsicwutvp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gezbzlbjh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gprsogltr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gllpevass.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gayqnitob.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvyyvroux.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/glmvdqfcu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbcwjmjq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gadcmkudh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gzahjofzi.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqhunqpyg.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gniguvjfc.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/grgvrwfnq.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ghrgbjzkt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gekkqwuwq.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ggefhzvdh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gbssqvjoz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gqujxbuxg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gohseryik.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gpefuexzs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gwpgcdtib.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gxwtqvrxl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gbtgdkcne.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/ghlkghlly.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/grswsojue.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gpcjrjtku.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gqosiwxex.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gsvnejrwc.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gqgbolagt.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gozmpngbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/grzcrsvfj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gukefvnja.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gaxdhaxyf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gqulsuipt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gfhnvurgi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/ghxsdauno.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/glhqbhjxv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gyhtujwta.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gnefqvbom.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gcxuoonqq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gngdchdmk.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gtotnyawx.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gqvivfwjl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/grhsjixbl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gbzdbhdiv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gcqeosefw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gvpuemrxu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/glrllziuc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gfmxilvgr.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/glfwvglnb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmloyjqik.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/ghqoonrss.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gssmsipdg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gejpnfqnp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gfxlmgjmx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gpuwalwvt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gicdbjouo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gnzyjwuvq.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gmelvahuk.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gonybmwmt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjzaapsro.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gzqzehkgx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsoeiohty.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gwwiirxso.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gngkbqhma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gapaldvgr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzaqhsvwp.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gkmzuecly.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gaycusbcd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gjwbtmieb.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gptkptapu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gmqtlofcu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gbefhgfta.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gmuoufspc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gkyvgkutc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gpwsoniwi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gyoiwhcxy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gtwdtasfr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gsfceweup.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gcgpjzwsc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ggybxkqne.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/ggyassngk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gnhzpuypw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gkqnddicn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmdbrioyf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmragduoo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gewdqbsut.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gaojpweel.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gzuifyayc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gepuvtfri.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gpulpzehb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gukniwumh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gofwablel.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gonsfrjst.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzlvegrjq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gjhmzntxq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gxsfbtgpt.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/guulyhysu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gvqhwsddw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/ghxxgcnaa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gvhdnxdfp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gnmjdngus.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gzcdgpvht.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gjqyicnkh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gdfihautd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gedudhzmn.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gfbebzqry.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gsftaioqq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gskhktslw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/grwhlebep.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gyykuveuv.sHtML


<!-- 参考信息 -->