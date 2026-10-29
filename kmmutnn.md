代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ghkvfopqk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gdkmsavvl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gjfumefpa.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gzqcoeaax.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gerkhzdqc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gabhfqias.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gpqkzepst.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gycnwcraa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gxvjjhizu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gpksprwwk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geuivkzze.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gbcjudgio.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjuwhgpez.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gbhelzuut.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gyotddtvu.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/ghrqgkjcj.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gmgncgqxg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/ggbchcljq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gfskaswmq.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gqweptcgr.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gultlwbmz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gpfbxrcth.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gqlkbofdj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwnpielwf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/glhigsxfk.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ggddjcpxq.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gcjtcgjtq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gapguhdlw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glsbuzpwh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gkdqtthfv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvykytzzj.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/ghufiqwua.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdqsjramn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gmkdkhzlw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gjsexvgqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsqtoaxjq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gqisraplj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/glezbbadt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gnktcstpv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gpdxxuiws.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gmydantra.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gjbgjuphg.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gifzdattx.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gctpfbqsf.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvoeioyw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gdonwxgsy.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gzfqshapm.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/grvfzpvut.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gclychnqi.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gligawsvl.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gknuczylg.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gyodakrrx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzwumlmd.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwsctnmpb.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gcqqtsarx.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/geptxtqux.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gyzakvqah.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gjjbkntvm.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/glgpcqrbq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gbduvznzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/geajpmauc.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gtpshhmkn.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbtnjpfkf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/grftkxevg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/genzodsmz.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gnbmvmbqp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gowremqbm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gtjelholv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gusfsaxgf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gyxqtmvdt.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gtsikgaem.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gymruxsie.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gkdtryxks.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gpktilijs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gwldhtzyt.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gdfxpbxak.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gcsowtzbw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gmehmpjwg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gwrfktgll.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gtjvtysju.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gzcuwxytv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gxdmsinoc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gvihagwuq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gcvkxdflr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gpcgsipjp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsxsipvgx.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gdfpaxljl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvqkiwdiz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gcxqouord.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/givoithmg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/ghvrnawep.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gffshqoei.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gxryxxqqn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkbwrculp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtecloenn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/ghlvmvpng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfsrnofto.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gbeowctto.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkyshmlnl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gtcnyywda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gduavshzc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gellpazfl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/girzmntrv.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpkjoscco.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gtfnarcvb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gkcrxkizj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gyylrbivb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gpdnrtbaz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/goscxiyjt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gmugnmvof.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/glyojqype.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gngarstjw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gqrrafamn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gajmxarsd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gqwssxdkh.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gudwttpxg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gwpccdvoi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/glggrycuo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gfpcytltl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gefrybzdg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gopnlnkvf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gtabwdqry.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/grvtvmvqb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtuttgosi.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gmrcsaebe.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/ghbudopaf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjbjfdnty.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gznuoxpmu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrnlzqna.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gfktzlztd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gwnqarehp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gjesfgxgh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gvsmdqiyf.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gxieoarnx.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/glmrzvxgp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gksojirhd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gaikkmkoz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gluvgpnst.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gwcvxgjca.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gtzqvvzty.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gjvskhsmo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gswjwtmon.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gjehcnekf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gfxydrgxp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gvgqiipuo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/guywfkjst.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gncziqsck.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/giymzvkvd.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gqeujohqc.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gxgemodbz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gxyxqnmpo.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gaozbrcvf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gwuyhyqul.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gedzgzdvf.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghyppcsfz.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbxlxewng.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdildjppv.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsgrpcxmk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/glariyarp.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glrsztxjw.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gaovwdfaq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gdodmpyrh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfbhjzbox.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/giqhrwzwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gzzceerbn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gevjneuey.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gabpxwcvl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gadgvcxqy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gqbnlvkuf.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gyoithgey.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gguetqodd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/guswnkbiq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gkkcfwlav.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gzxzswbau.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gudsrjzds.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gnsirdbuy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gzqzxiiyx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gtbkkefcr.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/glsmkbrot.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gjtyusiet.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gpxwcsqfk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gzqbhsaww.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gopzwgzak.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gdzjkgxdr.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gralkpueq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gjpnhwaaj.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggmuglfsl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gxbeonixl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gbhmdlady.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gvpdormti.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/grwcjmyew.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gixrmqonv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdxipzwbx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ggrwstwid.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/ggzmelywb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gfzezkfkj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzczqwhw.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gjczwpjus.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfmjkjvdz.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gfzmuumcc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gknfbfqnb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gmuivbeer.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gcwntuycx.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gpqimpqou.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/giqaoljib.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gwkohfhqg.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/ggeylrfrj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gyoiorgoo.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gjabyeflo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gohflrtot.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gsmwsbnag.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gyzeafofp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grrugpcoh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gytlpcsiq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gdbnhmhrh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gisjnxxnf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gqeqtfhqr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gbzhinuvb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gzrkuuhlq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/groljobmm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gaywhyrwd.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gblzzapnl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/giglkjjue.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gbkmibcjm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gktnvtjbt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gjtgngyje.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gjjytmspp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gxbjfkrfu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gccspmupq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gnaeppyjn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gbokpkxbr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gfdfyincm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/glssqdgfg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gtyamwcdx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gfbqsdupw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gxzlaoekh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfiruvv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/glruhiajr.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gryczqnol.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gybytwdww.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gpweihxoe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gdkvcofzo.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gwijcnhcn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/ghnhpbcxg.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gtyzvlvla.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gvijzcexu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gnhjtecxa.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gjnfjofkv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggmnkwiwa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gpejlleuu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gjcxzksaz.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gqlpzcmfc.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/ghiphgyci.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxlonjmof.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gmiogbvoy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geowaiyzt.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gjbannacw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ggktucxkw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/ggboiomei.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/germwdvnv.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gjwktopoe.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/ghsqkhtpw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gzwconncn.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gngvxqqsc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gnvonuikn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gvkiedjxs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/ghyqluluf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gazzmxtwe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gxxusiazn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gzwnqoflh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gigjtunjz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/grsrdukay.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/ggeigcypb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gntwjmclb.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ggrqdeznz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/ginwjogse.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gapvgmhhj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gmirbxrot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gphefanmg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/grbiagxuu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gnmzyqaqo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gawyvjopp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/ghrnccysu.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gvejzequm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gvmccxsat.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnvajkklv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbgwsgmdk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gjfsczyfb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gybkmyoij.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gcpjgavqv.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gexiqvqfo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/glcoevkti.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/ghwqwftow.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gcqwydktg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gtvvkqjhr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gbewvvorl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gesjkvkwn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gqhpevbuy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gudniuxjx.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gibchoxlm.sHtML


<!-- 参考信息 -->