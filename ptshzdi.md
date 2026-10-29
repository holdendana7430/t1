代发 wailian999

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ghbjnpyww.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gwlxtakcf.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gpzqdtiin.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gujlobpws.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ghmpzcimb.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gvupivmry.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gjwfcluyt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gpxkgtlkg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gimowpfai.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grhasauqk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gszospzrd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gfkgutwfg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/glacqbasp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gugxlsfll.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkzsoyzlc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqwadzw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gckorhpdu.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gnqklepaz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gvgdcbzua.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gbtqeingh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gpfpwmiqt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gmukhcsnv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/giyqynvfk.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gjrlqammh.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gjifqtvrc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gazchuxio.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghgovofzc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gpnvpazbf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gabnmieet.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gandlcwjf.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gvpqksxqx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gytpesjoa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsolugsvb.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gwbtoxlgd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfamvtqsr.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gtndqzngd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/grodyigbw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gfjpyuust.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gtgaqdmmx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gnlwjwpil.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ghzptpqdy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gkuuarqqo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gwwmuvkyz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gkiwngtxu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gogprizfu.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/grbgdwpbs.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gkutdsfms.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gzgpowuhs.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gvmwjaztc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gcicvmsyb.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gjnrwplrt.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/geszfsoqo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/glngatvfr.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gvqcqtwqx.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gycwnfchh.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gaqfihvdj.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggsccpxww.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfgsuaqvd.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxtaepjyq.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpvrifsbe.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gvvzzdloe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gckrfhtdn.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gtggzpnwt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gypvzmnga.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gasmzxmmx.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/ggndowuru.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gxnnacdxp.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gtqjmazes.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/godfcwlnu.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gvluefomh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gyrkgqskq.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gduljdaps.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gpvspdluf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gkmheujsx.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gpaqsgjze.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gqxqnbcyz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gszmykyuo.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gjwksqlzy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gcwradgts.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkagzibog.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/ggquiagde.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gxeermduc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/grfoimxmh.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gdibqmdbz.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzwbviyfn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gdslfhpzn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gqiijrouw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gaxavwpxw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gjapjumzb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzztomjiu.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gmifefcro.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqmqvrqlw.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gufqiuyuv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjkhnnqej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/geamavaap.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gogpaibbg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggeugwvsr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggykgmrne.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfnxroqih.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gotgaponr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gofgwqdwu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/geuujgguj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxxzgumoz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/ggbaqhvvr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gilcstbdi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gkxymztfy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gftgxhlwz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gokgvmmwa.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glarbwlzs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/ghmihhvnu.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/glgqwiprk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gxuftahuf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/grvkoophd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/giylkzwtb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gfgxhsayr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/grlxafnht.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/grchnjydu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gsisdyhoj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gmjpwurwc.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gcmbdpgyp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/goairklnn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gpcfklgmp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzhxzfosu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gwgsrcmgo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gbgeurpyd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gkylgqjag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gbtrszert.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gchceymse.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/grngsvnqu.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gzctyhmck.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gblfukgui.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxljnsji.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gihupzaif.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gidfoivkl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gxiwqwwai.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gsqymjzlb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gmqddbptc.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/ggbjgtanu.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gpgoxanqc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gnehpnuwe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnwnljqfu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gaxetpcyw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gbqsyfsox.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gzyisiurn.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gahlzzjnf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmvotyjua.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gjqdeuwak.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gvnctbsau.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gyimxvgkj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/guhcmzagv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/ghzjjrecy.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gysqaovfi.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gtnmaorsl.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gxkfjxvuw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gatxiwamm.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/guuggpyqj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/grrqwmcim.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gfjfwtbio.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gmufdaiog.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gekftelvy.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghckuhecc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gvynhsrbb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gtlcaaixc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmonjzgti.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gfwtevshp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/ghvwntvvl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gljwjsfua.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvfqprtbh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/ggagwccwh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gsfjazipm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gzokkvqjf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gkptpcwab.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gtgizubpe.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gbolxdsrx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gfoymszpk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gipqgvssw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gonaizhyq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhxmxnm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gjutmpbzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gftkasafm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gibvmcvbu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gtbgykitx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gnnqimjsq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gzojtpevh.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/ghhdkhtfq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/ghbiidnwu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gumwkejay.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/glximvasc.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/guvdgucmf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gbfgcymcp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gatrssacd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/glsxslxva.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gamxgpyjm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/geithvptn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gekfxolpv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gcgcrwvkw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gbivsfzbs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gjqskdjsu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gpxaoqqck.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gljvnrkzz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqxcrifij.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/giwlbxbdj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvaicjdok.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gvjyubixf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gdlehjwql.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gtqrhgryr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gvalmsejq.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gnjfqgtjx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gkraahpkw.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/ggmyhjaim.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gyyadpyzf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gaomhkvud.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gyijnitfk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gkqczqjfr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/getsznrwt.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/glarhnsth.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/grculduqc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gjmrczoao.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gtfmlhblb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gkckwwtrw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/geiulsvge.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gdnzirret.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gxfeubzec.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gjsswmjxg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gqtokwwee.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gfhxjfaio.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gyuuwgqwa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gxsfslzaz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gcbrngcqe.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gemdgzxzl.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gzlxvzqzi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gpldyzpur.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gfyviaujo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gemgyrqov.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gclhdlpht.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gogqflojp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gihcwvdtu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gzgvtnlbs.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gkvjzhkth.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gutucuxws.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gnrmxtqaf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gzifxydis.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/geidyfweu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gjogmfugo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gvenyjuqv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gzhseugju.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gxsslisgi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gwkdnzaqe.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gprqospws.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/glbebmlpp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gqzmzehzv.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdouryrfy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjvobhvry.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gqueumucx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gqavxakji.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gerjcabev.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gdbzejrdz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxseqcbji.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gmwvprxof.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gawcjyzpv.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/garuexrri.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gsugjpgjk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gbyuulxzc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gwkdlqnxn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gspuawvqu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/giedhhkxm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gpqrnrhbq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/geaziionz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/ggeqqmhkc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/ggoytajgi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gfatghtvj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gmeijgpxa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/guoziyknp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gdvrdmthx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gntlkzybc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/ghyireshh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/guubqarbw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gmsdenmmk.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gkdlootqb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gybrfblnb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gorujgibi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gtizunwpc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gsryotxsq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gralcidlc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gmjkazreb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/guvltvdel.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/ghycwwrkf.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gcoxqdakg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gptrxsbex.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcanapkgx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/goyhbbbov.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gyqdyudcx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gijnaklgq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/guhaqfslj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/ghszsmzsl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcdgcilem.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/ghudmndpw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gmpvngqcz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gytrdkhrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/geocuzvzh.sHtML


<!-- 参考信息 -->