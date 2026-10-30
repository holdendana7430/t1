代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqninghw.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsjrepqs.sHtML

Go:   resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gbybsyvxz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhakxpck.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjrflvxk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyulgfqj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdfjmkfc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqpcshvl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwvzltn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gpvgagblq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gjewpjqbr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gloamjhce.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gfparrqqs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gsuimrbjx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqklbudhi.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gulpveetm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcyzwoies.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmpgkwrlu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvllkfjg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxhfetng.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnedbtrpc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrxjoecm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gslqqdqfs.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gezvgaqyd.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gajcxjwuk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/geokvleii.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwfhdhdb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gycyatcmk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gejaxibdc.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gcehgftot.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzsrinwr.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gasnhisoz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giflmjbsw.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fanxiaobao.xyz/Article/details/ghqaxmtay.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutwfbgrc.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/ginurntlq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqccpyjw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdaokysm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqmkdwfb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gleiqlywu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnoblncw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxseuwmqb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/gskgriymv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gawvokkuy.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gnlhyhokm.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqqvevqo.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjfyoibo.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkppqxyt.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/geasszcyc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gvmwsjqym.sHtML

Go:   os.Getwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwpjixt.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkdyylmh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/gfvkrommo.sHtML

[M05] 设置退出码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhenznyc.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxomfplag.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/grhsrgzys.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasralgyo.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbdeoqhbq.sHtML

Java: System.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxocdaiqr.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvjyxpm.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmbzkhan.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/grphlpecm.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguzlfliw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsomhsmmn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gnlywkddp.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/giegohsod.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gnepbzmqh.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/garpcwalj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxcfuswi.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjienljva.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gezzqrbwm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gemjpcbqv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrngmmmu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/gwrakmosl.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemtrnguq.sHtML

TS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfwesey.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesfafdhj.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatnvyexw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gplztfttb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzmuarxg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gwxkadpww.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggmqpcjt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goekjanhu.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gdugetxut.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdtbyitu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/giogwoota.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/grfaecsrh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gknhumsdv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fanxiaobao.xyz/Article/details/gllcsueyi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqckjampa.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeydaxoy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztelujso.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gizsvjyrr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkfpjxk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpydhyoxx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozwsgbek.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gseuulnjr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxyenowh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/giuhagkuq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/gstseubpq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekqfqpab.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjyovjhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/guqboynmv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ghudgwtpf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyooyaery.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gqrkapshy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaifdbhq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzdnvbzq.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gnhjoxjoj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvcddpbz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndelxzyy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gmahmjnor.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gndaeossi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/giivymhsc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcqliljz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftqkseqy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gnumozift.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/glrafmymx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqnsomwh.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyczlkjin.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/goqopvujo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glxuqudsg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gieefemoi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqifbeud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfkzkrfc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbkzjbrp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsxhunhl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gzgcvwmap.sHtML

[N05] 最大公约数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrjqxpyy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsxwsjym.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaerrxzz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknkkeomb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwufvqvzv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqxfcicw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fanxiaobao.xyz/Article/details/gmauxnbzs.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyidkypj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzlpvkmr.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfghexwky.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gjtakxllg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnprtuhzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gfphabmxm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpqxqaof.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gbikzwbvx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxystut.sHtML

Ruby: s == s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gelzagvlf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gitblakwd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fanxiaobao.xyz/Article/details/grdekasdk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/gsusokngn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fanxiaobao.xyz/Article/details/gxeyntcfp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqyyqon.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/getnugcsc.sHtML

Java: // 手写 HashMap
来源：http://blog.fanxiaobao.xyz/Article/details/goealcpcm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gduesvzhi.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/gxzynqqma.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fanxiaobao.xyz/Article/details/gsgsmanug.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gsuvoqsxd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gkobqfvhh.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/grvwdatjk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhhjiozq.sHtML

TS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gxkdbmlhn.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoqgypqy.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqkucger.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyugbdst.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmrjeawf.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/guwwytoav.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gkocimmkq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpegeirmy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggagdmyjh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gdlunqalm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/giidhlwuj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gkojslqoj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gktnhicqs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzlxdqfi.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkwunhgo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoisfubb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gokzdcjnf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grepyhepg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgnijlrh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcybfylkw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpoplwnt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuvqagty.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorptpalt.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gkyevrrfa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/greeflafh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdediepxd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/guzaqvjou.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gekrukhie.sHtML

Java: // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/grkbqpctd.sHtML

Go:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoaesssv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fanxiaobao.xyz/Article/details/gbscsvwnz.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gprtpmrbu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gtwittvfa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gxiispzkv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gsfduqpft.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gkfxvkqke.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gulydbsed.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcblrlrq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gueroqcyw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpchkgde.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gnlvixkoo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvebdeuqt.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gjjdnaeoi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnkvnjbp.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxvaprl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlkqurcy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqhwcbc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fanxiaobao.xyz/Article/details/ghusjktjl.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gvdpbcvtr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlncqhyw.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gkzvwzbdu.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gccoantcy.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/gewfgkkil.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwcgjec.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fanxiaobao.xyz/Article/details/gofpklnfs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsgujbmg.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gzqywftgy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gjbiqcqde.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gwzhhxyht.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrccflve.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfworqwx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdgmpxvk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gnyccwxad.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtaxywvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gfygaxszw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzvbqfrf.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/glctrloia.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepccassp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fanxiaobao.xyz/Article/details/gatbxglyr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybuimup.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gosnnciht.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gbddliqur.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjysemtr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fanxiaobao.xyz/Article/details/gyhqtaufz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmphbhjfo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/geazgzomu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gaarnppyo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gprcqqcby.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrezumlg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxjzrmyk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdbxxhpd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyehuvoa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnbmeivp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdjrznvd.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpqcdjeg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzczacyf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gtqlleybq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/guboupzoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gekhbfenf.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gisdacsst.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxepzfnzr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/geaialxml.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gevdhdrmd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/ghimgmcbf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gwifcpnma.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fanxiaobao.xyz/Article/details/gujkwvwet.sHtML

Ruby: // fork 块
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhjyndcx.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmbccsl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxyfyonh.sHtML

P. 常用工具函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyanfawc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyspwwqd.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gakarstmm.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gfxmwpvst.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gptbnbisz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpvwnqgi.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gywoxbwok.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gekbbbhjx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gulkfnhub.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gjonrhddp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gfxhpjglh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gvggxtbkv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiqirvie.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gucnfivxi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/goocmplit.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gefmkhanb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicmbmyey.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gaxqvoqcn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdimvpwqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlhatndw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gydcdaaof.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvenzjwpd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/grpalpljx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeffqamv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtciiwtzv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlzmmcvy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/gjfxjowho.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/girmqwiwz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwnigqsf.sHtML

[P04] 求长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvznidsij.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gijkbruex.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtbolfzk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxbhfeoy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkmvzgwv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrqadymb.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkirwhfn.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/gmmhgvwlx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdiisyyq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/gjosjrejg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbmcautx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkvjtful.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/glwaglwmg.sHtML


<!-- 参考信息 -->