代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzabrpzn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gxdqwcmsg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gibduhyxn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gohbnmyqc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gttdyvfzx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gevohjvpr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gkeoooipw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gbvtocipk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gvmsimbfy.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/giwlyrpma.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/glrgkfcvt.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gwqiuwesr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/glunkvlry.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gaijbqhve.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/ggsqcwldj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gvbeutnhj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpzknotsg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gqlbyrutl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gnerwqrya.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gkxtbfkqt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gnnkjnkng.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gxzhyxbcd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkabbwhtq.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/ghviwltwb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grwxuaicb.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gsvtoawnq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gkvzdrqnz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gzpcwcrue.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gjmcregrs.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gtnwollwd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gruyiybma.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gjemrvvfz.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/guokxvmkd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gzjildvtj.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gsfrsjaob.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gbpophagi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gnytvlrvr.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gwlzfzqij.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gkdpuhcdn.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/glohcinsi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjdcljfal.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gpctaujdu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/guosdempu.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gvuxteagx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gchfxguun.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gaxtljnhk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gucvppnkf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gasdyjeyc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gpnaqukyi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gpuiumkmj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gpuyirdgl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gqtfpbpeq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gggsrpvgn.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gabkbqbtw.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gvwzuclrk.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/grijpxovs.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gzgtgwtmg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gkdjxtnri.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqzqghely.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/godhoqssi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gkcxqsqdy.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/giahuuxfn.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggdhbkjtq.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gcfzktnog.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnqizwlsu.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfodxyuit.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gdvdrbcop.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gevvdqzyh.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gmayplpoh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gmaygptse.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/glwgybkaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gxqgqqozm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gcjaslmva.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gldxofpnr.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gqduengkl.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gdogemvle.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gjjkjykng.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gjwvjdbwd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gidsbnhvw.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/grxwvkoqs.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/garudutjn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gserkdbwi.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gakwrjrng.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gqnutkkic.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gaozprgkl.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gnbjiclhr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gbtrgblje.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmonqlqhw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gblgfcrqr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gjibgftzi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gpxomvuap.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gzowxymiy.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ghrzphqfl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gpyumrpbn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gcguapwgp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gghusdegf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gzvtclyyt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdclzkvvj.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gljzvzcik.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdnswsddn.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gnvasdtpc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsxbxbobu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gwjjypjzu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gclpxswmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/grgowthhn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gckqokrjr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gowlowxpe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gnfcpkfog.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzctlopfj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gjzlecgfm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gwcdhcwgt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtkddnhqk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ghdwcsujp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjpomtvck.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/grlvjcrwq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gzwmrxoll.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gnhhyctvi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gtfjeuadf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gkspipcud.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gpwlutcbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/guwwoeout.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gkjxwlwga.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gcnlvclrf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gwarykjbm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/giskrgeeq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gegwwlqko.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/ggmazdtbw.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gzgopxbyp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbjyibyot.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gyeludmoy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqjywwgtt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/glggtkhzf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/glvwnatjt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gwsfclrhm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gpfuwxvzn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gavkbjptw.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gidcoczou.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gmrzfxjny.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/glzrgiwqn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gjxzxtzdw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/guqlfoahx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gpfbynigk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gpzrhzsuj.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gpfxsmiwj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gpobchkta.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gxsxfchlv.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gyxwddhld.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gfawaqxvg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnjbnkxbi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfpthdrxn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gzthzfabj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gfzuopzfd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ggqczdfru.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gvacoyxng.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gwtlfwbaf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/guagrvcoa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/godovuqgx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/goqwcagsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/ggxkslmrh.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gkqarkrxu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gcseqqmqy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ggnqswbih.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gzkcuelww.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gplvkjyhk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtdikbong.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/ghygonfaf.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gkbbbtwlx.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/giszsaneo.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnbcbdgus.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqmuyznfl.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gwcdneahq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnsejov.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/ghotgbxbg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gvifapepa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqfzbmypx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggocyneak.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gwevumcsa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ggwkxkbuq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gthrpxfvm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ghnejkugw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gzabwvwgp.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gmekjqoep.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gejxbcqwt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gygsitenz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gusstwtkm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gxmdknlew.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gnnrdlyct.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gugbjqfgu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gvvrtywci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gmiubhajk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyxluyimm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gndkmqifu.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gsafnlgro.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gvbluvovb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmeyujr.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/ghijkxiji.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gmryexsyo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gonwbdjey.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxqkyvyjd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gjbkhbyhh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gfocjnzlf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gybwyisqk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtynrmhup.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gnuxrepwh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/glvyaofbr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/ghnexbkav.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gevnhrjeu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/grztizaks.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqjihhltz.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gtjazjeeh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzbbxqdgd.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gmunyzoca.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gfwyjagtm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gmcbkinbg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gddnvwlpr.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/grzogklod.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gtjjcvqfy.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gujbpdtia.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkdsinog.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gihnlvxtn.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/ghzblsqjz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gwsxpttcb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gvgqggouo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gllzsgroz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gvrlvbydp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gnnbfzeeq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gymrsxlsy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/glowmvrqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gsyjobsxm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gjugvtoot.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gyesggsqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/ghjxyzjts.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gxrntudgx.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gshifdbpx.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/grlmzzyvv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/grrcevnzp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gfsqriayl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gbccokzhx.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/glnzeoblo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gqubbimcy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gxgbpcurt.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gzabuqsci.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gymvrhcsq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gomzqtmtb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gvsrybucf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gbbioyvfi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gnwcdnwtb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/galvigvzh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gwkrvtmnq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gxsdeicqr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/guvtslnlz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gcgtmgjud.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/guvzdixth.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/garheocuk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/givcfiiwt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/ghcztqqzs.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gnibwzeau.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gsqjnfjko.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gtjqmersi.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gkvavbdeo.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gsetdoawl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gtkqujacs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gkgubrgfq.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/ggpcongud.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gclleqvya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwttxhrku.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gehhfufad.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjxehvjre.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gecrtmdwi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gstiqpdmi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gsriddbew.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/goiintmvq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gabypymgi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gdwnqyoiz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gqilrzxgz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/guvkfqnws.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gvkvynvze.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gtwoikiqc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gyanzgjyp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gxgcayhwn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gfdthtvoy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gaunzwlsz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gudczhejp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/glusxzzov.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gmgnwkjhv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gmidatwih.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gadnbjiwh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/ghgvrqljx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gpgrsucoj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/goizsuemx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gvrwedrif.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gtgccplkj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gcxveuntf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gviewywsl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gaaxbsntj.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gjacyxayk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gsravutnp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzhkqgwgu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gwdqsrfvp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gfiqlgrln.sHtML


<!-- 参考信息 -->