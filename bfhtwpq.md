代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gcfoinfyp.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gvsjlzkft.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gkksobint.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/guyishsjm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjhmcbuya.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfuibanwo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gnlpkolvs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gaiyeadgg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/geyznvwcc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/giccypqfk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gitmadlrq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhutghw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glkmelwsb.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gmvdkgnew.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/ghertqkia.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gmmxovzlv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gauopyara.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/goqsomjub.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gkqbktnvi.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gxohfensr.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gxfqaufcs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gusskybwa.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gsvmwmtcw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkoxkllqx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gduipyavb.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gbbxjryns.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gxbbnxemc.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gbbnqamrg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/goscwzhrc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gxkyjmgws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gbgqltddd.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gutnessei.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gaennxuop.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gmipipuvf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gtyvsoszs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtdwsswqa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gphajvcox.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/ggbwebhxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/glqepyfzl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/glztrdpgt.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gmwoebvdy.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gqmthmvhh.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gscfrdtvk.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gdkbqirda.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gkdceggcn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gxkucjrwa.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gavyqxlkj.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gilpvacgz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gznmwkpeu.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gmhvvjxga.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfwxdkokp.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gpeyeauaz.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gpdcrxmfl.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvbwysmst.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glrslchfz.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gvtyrpgqi.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gsjmrshgd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gnecctovg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gsmxmybjn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gtltxdakn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gnjjjrvfw.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gcvvdsaoo.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gnxserspk.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/ggzxvmtxh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gikterpet.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gfoiswkvw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gnmatitce.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gkbkeyjge.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gvaurlnzm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/goeuiukpd.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gntgnyygr.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gysnuebnc.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzwqerqx.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gvcggbnnb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gypfiqlkq.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/geldvbepm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gybsftpzn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gieldgwae.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gbxieoiei.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/ghpaeykbo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gpedmblma.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gdaejnqsa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gjpneeewg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gwskvlbex.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gcipliith.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guzhdkczq.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gobxeavsz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyjhfaock.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gxuvfsiph.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/guxxxskqp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/goklxpltv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gfklskppd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gpeltsqmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gafsedzex.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfbqbymfn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gmmkucvaq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gohjemhqi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gyujrqaek.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmdimdsfl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxtotdgqx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guxwylphp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gqdnwaxzz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gqhspvvwj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gabjlnzuq.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gxyvciuqx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gvbszgris.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gfvxvktlg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/grcfclnks.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/ggjkotfog.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gkhkwbeuw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gjpebrsgi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gjpdnbfxd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/goqldgdkg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/grelbuevi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gdoxgtxzi.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gztlslgsr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdudmvywt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzpuyqvmy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gloupbpmz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/galzoybiy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/glxsnitwp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/galyozkej.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gxtkfyzdc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gezlpaddy.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gpitzqyif.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsepsysvc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/giwmoelru.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gvqxlgugg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gureyhrxj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gojzviryj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gaptvotuh.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gbppghyqs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gzvjtpirr.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gijbgtbtr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gbeenblnr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gjspdewzl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gskxnlxct.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpqrhvjwr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gjeevjytf.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gqmkrtvom.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gmihomlsm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gpszgrckh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gwljhohvt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gkqjmzaqq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gxadkipmx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gitpmivse.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gkdeanjfq.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gvgvsvmyw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/grkwfudwd.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gheonzvxz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gsgfhgdea.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/ghvxxztju.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggvafnvfj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gjlvatcdm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gsgwpyomd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdjtjfqmi.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guwgzzntv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwooiuaey.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpofsck.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjiaesaoi.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/glghlgxvs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gyyxqvyed.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gletpxijs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjtsjbzhh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gogizxjzp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gvrodhdvr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gsdkbdrsf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gcykotrac.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdimodkwa.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gfktgadiy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gflgaixzp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gusctwctb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gorgdaacn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gacxetnwn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gzmsdlcaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gonbpiljt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/guskhhnvf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/grtrvxfjf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gyabepggy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/grphrokjg.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gwqsmtyvd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhdjcwr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gvgckxxtn.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvpzgtrhy.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gmaxcnvid.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gsncgvvdk.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzhokgvlq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gunbrimez.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gospozqtt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gajbvkqal.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gafiaxmog.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmogdjonw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gahjpcthl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gpryfvktj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gaerocuxz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gqckmqauo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfhnsrndo.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gewhlxzup.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaolsxnwl.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ggndqalwa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gtuzgudec.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gpzkfxcjx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gcfafwalt.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gpdjhzrpm.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gnevegxox.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gsownnzio.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/guufrlucs.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gtwxmfybi.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gbbsrvgce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/giaepychp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gksijohtx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gujdczfag.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gnhiobciw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gwzqcacdj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gizufkvdy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gaehovqon.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/guhskfydc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/glemexoet.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/ghroltxzq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gkeadzyzo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gcxandspr.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/grnyzvdfg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gwnuxsfyz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gbdgknlnt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gxhfmmjge.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gfisaiicf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gnywkdzxl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gzsvnzrou.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gtagrihry.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gawtzrymd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gqevgrjbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gcvktswsy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gppktclje.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gcrdhpxje.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gzrndbidr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gwypjstri.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gdcrjprot.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gicxzataw.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/giprqkdae.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gfwqcewkt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gefekzvse.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gcxsensap.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gjljdmnds.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gwhjvlknv.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gaafwtohc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gbplpzshx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/ghcmigqvw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gbtzykacq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxktitifd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gyrxzwfpw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gboamauci.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gpfpkqtjq.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/glvjhhuhg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grymqezwm.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/ggwonxprq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goxliqpbs.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gwjcwrwrj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gzulokslz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/grkilmkxb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/glxojwsen.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ghmxxktmx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gvixfotol.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gkblbzwew.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gzckpqqbz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gyzkzfudb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gopaeepxd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gazumlkwz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gsjwrjylz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gypcbynno.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gxzjonlzp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gzicemoky.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gocgsvgol.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/giwosraoi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gwtkqfluo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gcqziaqif.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkeauzz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/genmiwbjw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gzugqsfcr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gjswatsgx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gwqfeavty.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gukfnybfs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gmmxekzhh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gspacozfy.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gblzxnllf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gswzyqoip.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ghsiqceti.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gkxdhmmqb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gkekmooxn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gnbasdzhg.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/glqdnxuss.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/glxnvhoex.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gygbinskh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gnrpigqkx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gxbcfydjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbigfpn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gxzvjbway.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gmdhaaxxx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gysqnrgwo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkbfouhra.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gxtrmyjfn.sHtML


<!-- 参考信息 -->