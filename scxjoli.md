代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gygcicylk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gnmrymdbi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gjjqihwdr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gtwmnwluj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gpqahrphv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gwnrgwfad.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gkrtnmzud.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/ghdikaryf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ghowccxwx.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gzclojktu.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/guvcheocm.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/grszaciwi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gdpfwlelc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gqscwdpvr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gzgjrgaar.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/geankllek.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/giozzahfg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ggqvwvxty.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/getregmsq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/guyzokmdr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gjsbumjcs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gfyagwqsn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giedgvoia.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/grrxrcvwl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdqbzkaqj.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gztzircsx.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gkgvisobi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gwurvqfqm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gireldkhi.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gusapmssz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gdxurvjxw.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gthxeyppa.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gyawdlkve.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gcwzamvnq.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gjblotrft.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gmqggpkcy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gcdbccegu.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gfqaokojl.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gtbrrglxv.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gqazwgshy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfyqjvpcx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/grlvhtxov.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbquskgwr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gtvwjoqxb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gdfozlzil.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gshqgared.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gayygjwjx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gbwozrnef.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gkbftddpb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gocazzlas.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gefjujhae.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gifzntrse.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/ggnvysihz.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/grdzpipts.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gzznvgewl.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gzgdrkxqn.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gmhxhyxus.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gbdrfgnsi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/glnnwrfea.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/giyqlxmvr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/geberxzbm.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gyoehgvwb.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/glqouyfge.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gaickyxal.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gvbafvjst.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gpsyoeihq.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyytczggt.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzdicngeb.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ghxzgmbrv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gzepfimas.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gdlhooltf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gqldqcmcq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gfrzqmrku.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gztvncpcj.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/glzrrnqyl.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gukbcljym.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/ggcjgowzc.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gpwoduzmv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gsnuhwdot.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gmmsccdsi.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/goeuevylq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/ginumhcus.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gcuvxfxwp.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gcmlohhgq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gdhevmugk.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gkrbnrysr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/giqusirdh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gujjcmvqs.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/ggixjfkoy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gmjfkymgv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gnsrxcbrk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ggylfpyhn.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/glzjoctrm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gdxrqwcaa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gjhntmmvh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gdspviptw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gybnrbcaw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gssizeavt.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gnlkodpzj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goprkfjad.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gnhxnpvvt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsvyypfqv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gzljfxxik.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtelwohoz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gnaxncsdw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/glhcvatkd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glmgkajcp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gmfogmqlr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjgjozwwp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gkjbddhvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gcsjgrhnm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/giwzgeplz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gzywnrxcs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxuhexoww.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/geldjbfxg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gerfzdekc.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gwvwjsbgx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gjsgfgkkb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gzndexeht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gwxcyczbl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gfxrfeayr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ghmmszcnl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcqfthkff.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gqtkoyqah.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gvczrsmie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gfrybienm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gieyhjzag.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gidogblqv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gajgnpowg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gtssffmvk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvisgoumn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gmnjggeaf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gnecujlie.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gqvapcctp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gyerazofw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmnjlyjmc.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/ggrjdbvmm.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gjqvwejkp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/glqgyomdb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gzqnpnnpt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gltesjwas.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/glypcrmpp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/ggureoeoy.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gvfggeben.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gnoixwzuv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnfaudzjv.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gqhuziqgl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmeukpliy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gflmzillj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxeyimrpj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gxakzfbfp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gbxzudrkk.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gdacoocej.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/grsehgzjk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gfutljieb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gbqbisvgu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gfojcyonu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gcwloopcl.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gnrektkbr.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/guuulbdmb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gwwbafrcw.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gpyudyjzs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gvzitoizh.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxiqvrami.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/glughxxto.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gadsyeyot.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/garrbghbu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gpdueijhp.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjauboqvh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gpfxekaqg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gjenfaqrr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfwjazvru.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gsjywwqrx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gfpdmvyfm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdnltvqqt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gnsvicsjh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/genndmcir.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gqwtmnajs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gmgjxabgj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gitcdkvps.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gchnovyxk.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/giqnwydtr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gvngxudbk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gfuiiwsyy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gmlhqpuwd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gdtazyryg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/geexhlsow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/ghwqthsdj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gjmamqkvh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gzsfkyask.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/glhvcsmvy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhdlhnl.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gtmrwnxma.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/grnqeicdu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gxuygfodh.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gssplsxhc.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/govlgjhgf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gzotxbrdn.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gaiwvrfnz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gjjpnsmhv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gonfltagw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gyzsexdhr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/goolligih.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gzlnddvqk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gmnspdpfu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/ghrqabusi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gtsgtpmgv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gypasibeg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzoeubvcz.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gghricniy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujavucmj.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gfxzeampt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/grsznbfri.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gqdxramai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gnajnacim.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqkiwljeb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gvqdileky.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/goojqbtyw.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/grskknzxi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/ggpvsmbzo.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gzhlvfnym.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/geguaxqyo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gtvqqnhxx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gzkndofyu.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/grjobhbvs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gfqkshjte.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gmcvcbval.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gxjzkkgov.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gzxuvrlbs.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gwhdcjfte.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gyuoyidie.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gzjqgzcpq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/giyeixwkg.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gsgrpwlbc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gndmvszbw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/glukrdzaw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gbfyqloah.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gifhmvqji.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gwprdmcdq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gzkffywyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gncsurpnt.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqgjxlmeu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzzdtfjit.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/goxnwesan.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gwjmkqnbu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gevtjklpx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/geswrdnns.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gfjmaeszi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gtmkbohhs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gggnmcmrn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjodpqgdh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/goeghomwf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gojzhrkyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gajgwerkg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gfrnijjtf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gytzubulw.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gbjzhsybt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gdkswwjwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gmuxxvuna.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gqfpjuqbc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gldwbitip.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/ghssnvfim.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gidftkumx.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gyoperfsr.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/ginemwcvp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdwxqadew.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gwnpskxfn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnzmrnxbx.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gdslvgcef.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gepjtmhzh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gqsjysjke.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gxwpdykxf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gorlmeapu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/giwducfii.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gqjhvsnjb.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gefzikqxe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/getpdsdxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gauatbuqi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gvgqsbbzb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gwlclmufw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gwpxpmvud.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gfwtjvbxx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gqlzmvrap.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gdqoxrhsp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/glmnnysop.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gufrfztdu.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gbldwzvqz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/govapcvxr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gtirvrhkg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/grzqlmbem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gexpkbxrv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gbgtrzxiv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/ghasoaayj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gpbvsrerd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/glxbjhopi.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gwjfipnnc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gxkjdoorj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ggqmhvtpb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gqdwujtin.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/ggpjpbgsq.sHtML


<!-- 参考信息 -->