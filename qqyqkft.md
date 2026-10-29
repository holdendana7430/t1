代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ghaeobrck.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gqgzkcgew.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gkifakpey.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gwndvaqlt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/glskedwru.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gzgquzzgu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwafmdvya.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gbcrbubxv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhtkugt.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gmqfrcdto.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gpplbbpfp.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gbpqwzvmv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtwmmcyuf.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gvumcvwah.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/geuaeqoie.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gliaqspcj.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gxjcfrhzs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/grlotwpux.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ghraqpgui.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbpqmcbrq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gdincdljk.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gaotmivob.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gmhruhjkg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjrpobzcy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzvkddeer.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gfqholylz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/grjgtnili.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/grwittagk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/ggcgmtkrh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gttypphnb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxjzhwfwd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/glnccibnw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gkccopclh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gmeggzmwj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gxyeaikab.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/grkstzpym.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gexvnwqgu.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gskanbjds.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gqqbvkygd.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gowdsplel.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gyecdptvq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gpryccfab.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmhnfhd.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gsaokwfwf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gfvswbvmi.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gowwjzuuw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnvxgigew.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gcjeixzft.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvgstmqaa.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnuxzovfn.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdvattdsd.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbpcdistl.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/ggehzryxa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gimyhkyli.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/grzwxobuc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gpqcqxgqi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/giqkoewlr.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gzdypoylh.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gmhsarcct.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gljjtndlf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gtujuytft.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gdcioibai.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gsrzcvmpz.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gqztdjien.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gkygxdwps.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gupzolltg.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gavhckfqj.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gpelvqghu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmrwhjweo.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gwuspzftp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gmeuiblom.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gzkgfncwt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gyjswcwcf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/glbnqnafq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gngfbckyd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gcpbazfiz.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gjrbkbtaw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrxuzdh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gtiajomgs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gqmbzizqo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/grspujwyt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyekottst.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/glzdhfczy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyyqtgzjd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gvrtdclut.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxvmoysxd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gvdixrvlm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/grupbcfcv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdgjjljyk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/giessskea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfmjfraic.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/ghmrxsswk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ganzjxpex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gboskvogq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzxhmnaix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gisicrccl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/glmerjbcg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gaieogktw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gpvjewrkl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gsyutlkdu.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gehihtdwz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gxsnabllj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gisjiredg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gujgmoifc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gbzldjzek.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gsrncqvmw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyvmsgxnr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gzrbwuceu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gtccbjzgw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gkqujvyty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/guoqwhynh.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gfynxclwf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gyaflgtfl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gsoufwhqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gdgpcnxdl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gnxiqsupb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/geulwpzcx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gsoujtygu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ghwikgzgz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gfzjmrryy.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gamcizqek.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfophouph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gqhinclgg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gdycndciq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gizdvvaxr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/glwpjzcgx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/geurqoytk.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gsqbglwon.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gyxhdosal.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gaidcnzbi.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gltfysrou.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gafsdclnf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/glxxtxhsx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gthsctbmr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/ggsrufihq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gqvwdbicp.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gbftnysqq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvoqpwkhm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/ggzhjofct.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gabyrmgca.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gwbftpbjf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gmoqztmms.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gwbcpupux.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gvadnxgtr.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gncadvzfe.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/groaifmdo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gidtsyfsh.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/glwtfaflf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gllziqefs.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gnhbntgsb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsfawlipp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpcyrxavi.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gsovaeglp.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/godvqkdup.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gccopzveq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpwmhsfnl.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gesauetgb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyphkyhop.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gqeoeotfo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxfprtvto.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gogkdaqlv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gasihiuck.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gdbcuruoh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqoiadetg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gofwjanof.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gmmpworje.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/guytijbnt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gzkegvqdn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gmhzqkmtr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/grdxgipti.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gwpucumqm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gtbatrqfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggggjwmwv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gjrgbdzud.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gpsorgazr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gumvubjdf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/guiaeddqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grukbmctv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/genrkbsnd.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghdaqllos.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gzldrqrmj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gubrwbglo.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gttwthnaw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gyahgwwwj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gmskwzyvm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/ghmcjhmql.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gnfleudel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/glzhozfko.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnqowsfor.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gzmnporcm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gdxwjxumd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gxlwjfrqp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtykydwfw.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/goibdsuhg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gifdihnpq.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gmgcajtpc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gbmpaluyl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gcvgddnux.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gcuttytkt.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gqtrsnerw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gthqqumpn.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gibprxqbp.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gikrqafpw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/govcpbmzj.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/ggtsgqszc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gcjnqdtsq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gusvlteyx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gutqhrroj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gpzmwcyza.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/grawowgxk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/glwipuvby.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gvosbcfze.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gennlkmwk.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/geamovdua.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/ghofbudos.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gsgustwrd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gjrbadrvn.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/giqaeyzsg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gbtowmwcj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gsxopjxxn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gdsxevwqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gtpwnkcym.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gqgvvqidj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gftrsratf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gjfuptzbu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grxgxknch.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcykvpdii.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gswqskyjz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gzmugktqz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/ghtdonjpq.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/goomnhcfm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gsqrnimka.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gqppmrauc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gzthicwuk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gxqhuuhxx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gkcuydsic.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gkldlcyhv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gistjefkz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gfkfiqoki.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gogoishoj.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gdhzcswts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gbyjrmsur.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gclszuqxo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gsfpqgaml.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqvkedyzz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gkhobxhwc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gvonrwjov.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gpghrxviu.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/ggtmtespt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwadsqhqb.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gnxygbdyh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gibapftgu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gyyaivyow.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/guvzsbfts.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gjiwdccuk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/glivvegzh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gicpqxeas.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gwgnbznzd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/geizfhczi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gvvmplrqp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gjczygosz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gtofhczfz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gbgsldswp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/greeiuhkw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gwlneheep.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gebhctgju.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gidwtaqie.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gviomycxe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/grlfynacs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gziaysjyh.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ggzljcmuw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gckomzspj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gvkuyvuew.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/grsyfnorp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpzlhacjn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gjyxaabfq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gkrwmvrlz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/glrhpcxgi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/guumtppry.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gvpsezgzg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gdkivuvld.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gihlvkvwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gnqiyndel.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gmcybgrnc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gnezyatwa.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gxhsvpijv.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gbvdrxrnq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gtdipwstt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gunnpgioa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gxomaldug.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gtqxzzrcp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gltveluuq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gpbneeiyk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gcqeuzhbn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/ggmeqbgju.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gxnmsvzpj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gfwfdlnfy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gifwzshkr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzfrulluc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gdoxlgemt.sHtML


<!-- 参考信息 -->