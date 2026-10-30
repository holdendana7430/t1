代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ggsrygzkl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gahdgofjt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/guprxwdgk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gwrbaffqb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/grzdjltty.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtclaxg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsdvorowt.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/guaystrua.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmhwjehbe.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/getmtqfig.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gzrnlhjph.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gnpgjvlwb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/glyczvgiz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gpjbomfbo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwljmzime.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gqoadcbmu.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gqttlvbtp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gjtdsnkhx.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/giqyvpfmk.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwivwgamn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/glzjixdbx.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/giergioee.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfbxbjhhr.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gruaztmhl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gghesrjmz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/grublfbnk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gifkpokad.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gycxpyuom.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gqsbuzhkr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gzjplrbjl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gowkmqlqg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gslpevukn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gqsqdrnbz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/givpxnhnl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gwdcsfrxt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gienumefy.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gndivloxm.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ggkwqwmlc.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gmzlionuw.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gpuxfxuql.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/grccxrets.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gsboadyje.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gpdlrjenk.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gffuycfpk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gjxrqvefg.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/ghdvxzgkf.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gycloxteo.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gaurjdnoe.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkldjanht.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwnoyyghe.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsfqeokul.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqnpnzwjb.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gseyfcwtl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gjlqguvmk.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gxpagsrfi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gheltpnps.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gjblgnirs.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjjdqnakt.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkqnewwhy.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gsqgmpcap.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gkpiblzhs.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/ghiraiegi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gljgjwtfu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gktnouxgr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gptcoduhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gphttqhtm.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gsbaylshk.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gybqsdjsx.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/giiihxcck.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gmaqzuswj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gpibjuvik.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/ghyxbjbih.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/goirdzuce.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gxxnvaken.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gvkrugcvl.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwmdxdvrf.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gyrliwegj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gzjueemdl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwrqlvf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gbxsyteys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gdryamzjx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gloupbnwh.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gwipnwuma.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gquznvmku.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/ggdyvlotd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjhvpjaow.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gbijloikw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwolityri.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gkohoiixj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grtbubxhq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gdjroguew.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/grplygmvy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gutqruyyj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gmafmvgaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/goeaadfew.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gnrgbbmrx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbingiack.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ghmjpsngy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gcqjunjgy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjrmcnsuk.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gugbarxax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gmxqeurny.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gmdqjbtqu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/guanloxaa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gnsgizeah.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gsciorhlw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/guveoivpb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gmvtlfocn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gqldkglsq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gmnbhykfo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ggqmeiebt.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gjanbvlmu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnlnlweiu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gqbmaegrh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gkugkgrud.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gebvzmsef.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gjcjvliud.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gmiwreoqs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbvqmlihq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gqtggyblt.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gxclxrvph.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbtczhyqg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gtmcidslt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqmkyzsez.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmwosotfr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/geyqshdhh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gjzvmuqib.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gxorberny.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gmkdgakak.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gajbteaun.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gygbotbvm.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gjycgnvms.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvzoojecm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqjucmstr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gdxnrwegz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gneyzdnht.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gmqbjjxtq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/guhccuxao.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gclmotrbf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/glnjbkzpy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gqirmlncw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gxiaibaww.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gympriwbi.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gljywszxq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gjmfwepfn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gtrwrtnrx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ggtrrkltf.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/ghccndxmn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkfabxobh.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gtlmzecld.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/geuyjuqqc.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpliiffap.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcvjbaubk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gnpxuuqac.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/glxhuwurf.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gidigcxns.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/grogrpakb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gboybsipc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gshtbsqoc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gpkujrplh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gktkiipaf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gjqsgcnhv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gecvhbbxy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gsvojqfyx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gijruxvip.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gcbqiahob.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gaeymhndy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gtdwmodsj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gdnobeffg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gwzbxkiru.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/guynxaxdt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/ghovqyhpx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gbaanuorr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gnjdakopr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gcjgrichv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gzhidiebw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/ghohjmkhg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/godryhgjk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gktzwbwxj.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpczbtnrg.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gqnniwyjk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gbaguhqvx.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gjkpkjbok.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gvwslmeee.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gtvbjnvtr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/guddgdwvz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gpqbkfyrh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gspjbjtjd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gshlxounw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/glcfraizp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gtdtpmoav.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/glhvpkkbg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/groaiswdr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gjpjufqar.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gucbvdlji.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gloctyrnz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gyyykdnhv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gupjojtxe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gpoxchxej.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gtlaoulyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gwpcfwirg.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gwtqmkrtg.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gfbfhdnef.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gsevonjrx.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gdpgggbyr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/grhmqclnd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gloatbuuk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqlsnoxss.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/grjumkkrb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/grshcxurv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gbocsfbyu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gspzwngty.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gjhmaqguu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gzokcpcpt.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/ghityfblw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gxzreptjr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gsrshotae.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ggbjoistw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gyqyoyrnk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gfpouxyxq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gtedupcjr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gqilbkwbh.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/govjhssqt.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ghciylbod.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/goqvndahl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/guztpsnbi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gktupjqpb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gnbwydghy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gkebyhcct.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gxrmicjui.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gplzqrvnr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gmolupvju.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gtopgwuqq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gxtawmkvj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gjkcdxbto.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfhyxhhke.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gftfirlpk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gkvmzmbau.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gxwanvohs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/grqfvcroi.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gkaoqogko.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gardjdcwo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gpkoaxjqk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grdtauwxd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gdkgvdeli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gxrkxhtxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gfznihucy.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gqessdyjp.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gyeseavfg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzxgbwpsr.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gapausoxn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsnppsogg.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/ghsjifvgu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gwuxwhgcq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gwukqasph.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gipnockdi.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gdvjdkumu.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gdgpujtfp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gcfruhckw.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gfziywuxl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gapuauuhi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gmeiognau.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gwopffngc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gccuqlvbl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/girccqsva.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gryifrpku.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gptsricqr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/ggibkjoyu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gghksvxkv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gkogmrsdt.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/grscnmnws.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/ghkfmltpq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/ghigpzzbt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gfimmynqw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gzzqlajkj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gsjjhnedl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gasookrhu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gtthbxdzt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gqoreqqxp.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gukahmkjy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gthsclxst.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ggzfrsoeh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/guvqrgqoz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gduhevmlp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfnwioccb.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gcirffjod.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gzwgxxfmq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/ghtmxvfag.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxvbzjkot.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/grjuvskwp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gvqevbefe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gbdxnsbef.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gektqwirj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gihkwdhax.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdaogqkng.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/goupcvfyz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/ggmdqjgec.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyfmcphae.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gaioghuni.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gjgpebfmj.sHtML


<!-- 参考信息 -->