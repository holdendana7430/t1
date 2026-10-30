代发 wailian999

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqizzisrq.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gwvsfbcfr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gckoheoqe.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gakokrpjx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gyurvsklp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqdubrgxd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gjbbinrkb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gyfdhzxot.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gvolrgmme.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gxzuljicj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gurqrgqwr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gzfnimrso.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guffzdqbq.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gbbatllod.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gzvnavjeg.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gadpybtar.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gmkcgtcan.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/goalktxom.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gelpkhtuw.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gfnczicfv.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gahmkxrhu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ghpoaaxkl.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxbpwtuyv.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gfnhpoung.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/glfsevodh.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gumpgmaza.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gbpmgisfv.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjuhquwcv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdwxjknuz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gzbrnjyix.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gminmyxkd.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/giwyfwzzl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gyejurdnh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/goxdhbnxr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gxpvscpky.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gsrkflmsx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gejvopixh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gzkkippbp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/glwspyngi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gbmydctjc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gszuyrhty.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gggyvnzgz.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gizilaryv.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gwipvxprh.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gkbmfzwmo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gwzzldvoj.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gonfsmtol.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gbcmyylsi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdbjgss.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gyfedizbp.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnyjoenwf.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gypzadxtn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvhxjjswn.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfccovhhq.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjevrjlsu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxocygznn.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gumtmcecx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gynvourzd.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gxxbwjlsx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gobwvahwu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gulkmrjdr.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gpxsvobau.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gxdlaafed.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/ggomzqamb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gugrsoosa.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gfyzreeke.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gpwiaoodw.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gaqjmczcv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gxpzcwsnq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gvmizmvxx.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/guemnplmz.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glsmjalim.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/grjibkhde.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gxhgndzoj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/grtriyxif.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gazgqxwhx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gqrwjcgol.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/ghmafilym.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gixgzqczt.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gzrgoykmk.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gbfsmkebz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gvmntsvir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/grthrkizs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gvsckxabl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gzcbhkeny.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkpcpjwkh.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/glkbcboiz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxvzebrry.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gsreiwyhv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnkojpviv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvosvfs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gcrlprsov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gozfxuize.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjrbukboo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gncfehgui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gwizpqukx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzcmgqpum.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gptrzuctp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gvcfngibq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gwvtlqczt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gawmymece.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gfrytuhgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gvysfteyf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzgcdevwv.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gemphttze.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gftefrfdw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/goxgdjrnc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gtmqyowgb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gberuwuwl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdoadmcqs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gmgugbtbp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gmcqaauhb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gmttuamvz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gurxmkvck.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gjwjlvanl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gjzitfsnv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grwikjagb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gtrcrpubn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdhgnfsad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gruyqakgu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gtttkwepr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gsafctibg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ghgvaajei.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gascmsdpy.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gnaaeehkf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxmuxjfhh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/griabhgdq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gfksbiqdq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gyqsbviic.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/grvajmegf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/glhyrkgbm.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gdlhrlcdu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/grzpvjnyd.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gtbnhgils.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/geftoncsy.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gvmgiiqri.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/giinncnjj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gznqjybve.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gyhpyjnth.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gmdoirqcp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gjoxmfadb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gnxdgyvdl.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gecqvcisw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gatdexshn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gnofsvkoj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gfevckcvy.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gydufacbm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gsoiqjqlm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gapdqgllz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gthtkipnv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gfmuvkbhy.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gsqatjprl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gjhjqjuih.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/grlrigysl.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbiaavxmm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gcvsjcftp.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmmiipryu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmjpztrrh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gpujyfhkt.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grqauurgn.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdygvjugq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gktwyrqsm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ggovtetls.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfsqifxsl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/ggescmqbl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gzyellyqs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gfyqgciho.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/geuhhtekw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gyjgwfkwo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/glzafzohj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gqifrzdwm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/ghqeotgom.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gbcznhikq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/grgizodty.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/grdkxwspt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gqeqjcays.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/govlfgqep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/grluvcmma.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gxoryvhtf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gmwjapnuf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gpudkuwen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gxzdxotwk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gxodseyqs.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grenhfoah.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gknsslhbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gdjfolmkm.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwofqnsxw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gfflbqewc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbpvojbuf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gtxibajrq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gprqotifo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ggkljxuqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/goxextqyy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ghssptduo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkrgqflqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gkychxwdn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gntzrcpav.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gtryaxcbc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqtoowdwg.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gkkfgzzus.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gisocfrdf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gzgbmryxe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gssykmxcp.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/guqyjdecj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gqcpjlrid.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gdeqnskfw.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gtfauqobx.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gbkoqulpx.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gbbdzkshn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gnvhpquhi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gsrfsqiiq.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/glkzfkott.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdvvpxawx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gxlobgkyh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gkbtegclt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gxvtmizne.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/geptkezkq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gxsdhnzkx.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gkonesgio.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/grnhwlugp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gwgfzisnf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gtlffqjux.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gjccnhddo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gtfkouxdt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gwbqpfvya.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gzuteluje.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/ghyygpper.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gykmuishj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gxvwjczec.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmmsskiaf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gfvbajael.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/grprrolkm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gvyswwjaz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/ggvdroyxm.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gybhdiwlw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gaootewrx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gjrkmszyx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gnijtthug.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gwbetwfgw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ggotksomd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gumcchpoh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/grhepjjxh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gmtyjrnib.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gufelebee.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gqodmftko.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gdkhimvqh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gsvaovqqk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/genuzmnwd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjmuhuyhu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/goherauup.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gjjpzpupz.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gmmjogezr.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gbmhtmjsd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggcbevays.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/ggahxykgo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmmaeptjo.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtnxnptfb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gkozlgmqh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gfwyibgzp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gyznkxfxv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjknbmfhy.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/glbizsold.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gyftzimhf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gtsjmbytp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gtkwxvsho.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gspzblwsh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gjkieqqfj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gslpcdpea.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gddnscoyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gzuhpbcjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gtezwwirh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/grpgtlsru.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gcwyjxfkn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/giisvwmmz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gsqzryrvr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gxhuswszt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gofkitmmn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gnqfgqgds.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gcrkelkis.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gqozjsorf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gilprdwag.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gbsrgcefj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gkkwrvyxr.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gtizqctes.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/glytfxyfy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gcovuwbqy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gaxbsukcj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gffladasq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gmftvrqwr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gqscwrpsh.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gxwytinwp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gsiuguepe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gsrssmrbe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gsbzbxyzm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gyjoqhbba.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gtecvercs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gincrnpqd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gyaneawud.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghwqbifjo.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gwabnplal.sHtML


<!-- 参考信息 -->