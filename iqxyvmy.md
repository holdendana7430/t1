代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gprshlxzx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gtrmugmwh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gbqvwlvnk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gdwusqylt.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gltxicrfh.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gdyndjaba.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxbyruxql.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gblqwkmpw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gxuokgbql.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gyjhaqqpu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gtgrbzqcz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gifrguukv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/glboaizqv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gjsptiapu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gonsmkhpf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gcqrxkkpt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/giqgypknb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwglokang.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfqtdxkdy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gvzduegyu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzsdfopqr.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gwmxieodx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gefbdntgx.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gjmfcsdyq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/ggeisqryw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gltmdkjmm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gtkwmbmab.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpzaocgis.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/goovafwab.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gykusmztu.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gyjoozzbd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gedmwnhoq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ggmmfzkdv.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gmnmibdxg.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/girvlwbex.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbqidrnqz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gvylpibvq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gffgkbhqu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqsfwbbkz.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gmsifvbfb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/glbnqnoxf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gasedwohz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gailpguya.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gcsoxhytz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gjylprmbw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gfduwfsmf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/giwjqcscw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/grljpaqsi.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gogurzmhq.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gjmhhjdro.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gfxeekmml.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gxrvgrrcl.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gghmlbvls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gzkwxrovv.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gthdgcmnb.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gqgyxzibx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/ghxwsheoq.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/ggitomhax.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjwnvarfj.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gjreffhyt.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/grpbnnklf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpnlnzjia.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gykjauheu.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpohhdbhg.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gmvqposqk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gzckhujiy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/giafigkja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gffhjywtf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gmyfzrddi.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/grsvgidcp.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gjcuaniqf.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gmpaygmri.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/ggklqcxzj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gizcloiea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gkzbyyguw.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gfwgfrpuh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gptdxmhki.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gtrmjluux.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gfgbpkxbg.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gleocbzbs.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gqbtxhpxi.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gmfzvpgqp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gvwhfxivs.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/glpmpmgae.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gpglmqtps.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gotsxmubq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/giazdqpne.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gugqlrthr.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gedabqhjt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gymmfkzsp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gtprwohqj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gubofwnmz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gheaderdi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggjehfaao.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/goldjzaph.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjwbynkje.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gaecepcrm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzafuheu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvjyxensv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gtbykgkvx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzflurweh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwyujczmd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gawdhtqlt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gdeofjnpg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grmnoihhj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gemhijcrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/glnhuiiep.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gkauyeslo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbrzqqxcd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gdmnduxbw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gmudjdblv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gbbwqmnag.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gwjbzjbgd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gctgyurfk.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gfzurwvua.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gyqrwekxt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/geoiefcev.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjybygfgv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/ghsqpejxm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gaiddsmwm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gdnrdfruv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gijveyvbn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/guynpdgby.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gapbvwncm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/glyihiqpb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gvdytfpwz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/goyujcxbc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcvhjgruh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gayrnembo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gsoevutlu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gfjkqjmnx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gvpfeidrx.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gwuvdaztx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqhqljojp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gaxpaudon.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gnlglhusi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ggfqvxovq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gkkioeoru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gkueitrro.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gxotadlcq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gvfdstgdv.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/ggzulmibe.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gaadvyafs.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gsgzvlndv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gapbjxugq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gksnaxada.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gvatpfcam.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gshjabmhh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnfdwldut.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gblopuswo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gmzejfsxu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gjjzbwsij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gvrnibxvv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gceibbefw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gjkskbjld.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gvaoibsam.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gggldcydh.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gzypkkzsh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/grtydcqzo.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gmewmcfep.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gnrxmjjuq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gnmewagjv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gffxvdfhr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcckqssue.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gslthfyuh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtfhwurwo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gfoukaaro.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gexksafad.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gndjpbjys.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gdgdamuas.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ghsenfbbv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gtbpeaxdr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gpqqvmmhs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/glctkbuvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gerdklpth.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwadmsujc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/guljfnays.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gpfovhapl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gmsdjvgdi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gjlzrxdff.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gfovopngp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gnsfddqoj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gjvyqxymj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gvvhfttki.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/geixogcpz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/ghbwxzjrn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gxfewvnli.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gfycfelid.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gucodefjy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/ggksysnti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/grclnnvag.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ggnaeapcv.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnufidmac.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gucvykxqo.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqtquzmxb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/glniiklzw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gmepvuvye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/ggyckyyfa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gddvzgzek.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gtfwlbopv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gzssneyke.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gvowckiho.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gvmbmessj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gdapqosif.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghciyxkyo.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gasgonvkq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gokkyhmgb.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gvbzvdeqj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ghmmmxkfh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gwasaneqv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/ghfgeifdq.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gdvnsaxzs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gpvpikcqp.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gcaoyvekc.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gkrxzqkso.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/ghregaigf.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gcbpzjvqv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/guodmbxlt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gxrahhymd.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gvooiktjz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/giutobxlg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gimujjrce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gojudmcsr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gssxsnset.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gnzpwjcif.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gkfnpuswt.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gwtyxpwvq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gnouvfufh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gpgaqsxju.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gspnsqtiu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/giwguwgad.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gnvnoonyu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gxtxwxumg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggtfrglno.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gbfgkiluz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gnalynpxq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gkouxwukw.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gdibmisjt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/ghcceomyb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/glzayfxzu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/grcbjlgys.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/glywzmdwf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gchzwypqi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gabjmkyvp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gadwrzvzh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gicihhbbs.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/giuxahuin.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gnhtwouck.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gfbxbmwkr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gashvbuny.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gdxchdkrd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwfdyzj.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/ghxkjkpps.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gtfrqsxzg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gixohdown.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gwzyvwhcy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gtcbmgixx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gijqwczow.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/ghxslyvpp.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gaievgjkr.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gxfeoiggs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdnrhslqn.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/grzfqvjms.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gliburvtv.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gwomkcpcj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gkzcmoqef.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gwskaehzy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gebjzqoaj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gezgsgpnu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gytispmts.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/golbkbdaf.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gwqodqaxc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gtftghlre.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gwlwgxsoh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gvgenfidi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gtssauvll.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gjvksvadt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gsjhnpxxj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gfyfxvdfz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/grmyalpvw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gptvrfwpg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gypylxlim.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gsnjwoqxr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/goytthczq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gdevsxpck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gwjiygjgq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gmpwfmyxi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gtopilwdp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ginysvkmw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gyygaruso.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gmzxqkoti.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gqvqnfszk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gxwyidutb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/glmzxhogw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gircqhmrt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gejadywso.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gaokzwjjt.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gqermhtfg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gwvvijuno.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gubxrhoya.sHtML


<!-- 参考信息 -->