代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gtptpditc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gpjuesiqg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gaewoorwi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gyvfabejq.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gfzchdwwh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gggpmuabk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gqhmjlelh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gaayjavil.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gqscaiqlf.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gjtbubovh.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gexlebfvy.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/ghfovjgow.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gplmcfwie.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/geewsmtdd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/grohjsreq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gfxmwiwiq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gtjczdvwy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gycupqcjv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gxsmahuvx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/grgrgjkgr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gsadtmmfx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gbmirkvcj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glbmynuzt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/ghkwgsokn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geigupoew.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/ggpvmqqtv.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gvesguzkn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gtosncwng.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gonvmbvck.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gwxitqjte.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ginltaxac.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gevkrjbjq.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gskhfyfpq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gbzqjpcix.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gdfrlzazh.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gdgaaoitp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ghgqyjrli.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/grjsdaqhi.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gudtzwylj.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/ggnqljajz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjugydugy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gjjidyhfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gspzdchqv.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gaixswkhm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrcnufxq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gjqyjdmey.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gvsmuloyt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/grtlccrio.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gsbiacwdd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gjvtuyrzk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gozhqppbv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gzhodhdkf.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gdtmquebi.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/glrqylqwk.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gmsyhmilv.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gpzxqnbkj.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gskqqaven.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gfxgmramr.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/galfkzxae.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gywifgdps.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/ggpnhdsoi.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gqzfzyhyk.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/guxekkwit.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gpodptyer.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gvjgpacnl.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gpknrxstj.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ghfhgegel.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gloiqhlmr.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/goymnjzeg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gcsiinvlc.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gwjcpfrup.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gpcqrolqn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gtlejwezl.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghzrqiife.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/guuzgrbou.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gywkyrxzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gvixvwuli.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/ggnejdjte.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gyqwqeyvs.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gzlbcxsbz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gjlqbomjn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gjzupriwa.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gbtijmxmk.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gufgmvxqw.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gypcihweb.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gylrcrexc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gxmhjqtww.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gswrkoqow.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gvymytvah.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gptgqvsjx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gmdrhaxjn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gkwylccuh.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gnabagyjf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gmeiflmdy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gccmbfuts.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/goufxwxgb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gepclfyuo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjwlnvqsg.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gqvejldgz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbeglukce.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gypmjrzyb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcsbhtgpz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwammynxe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ghcnrygsa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gvnvkynfe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyzgcjlzm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkwjnntgy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gvgcliwcg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtxndakhi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gkudhtbnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gzcwooupj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/glwuikbnk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gdpuaqhxz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gaztjwgwo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gcihreqzm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/ghabppomi.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gihzyvbjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gnzbwffrh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gzngtdfvf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gzqcyescr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gqyzrpjbe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gscvrteoa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gkzbxxdwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gvhtrzyqo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gwnjrlynp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gfxjtrmgl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gkgijgyxq.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gowhaeloe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gpdtwfkwc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/guzmggndw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gureysrkg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gejubnkxq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gwmruzarz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gwtsseasq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gbhvdudyo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnaktdlqo.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gizbrsflf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gpkmazhxq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqyazbpg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gsmbakani.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbwbmonjx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/govzfwuyy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gmqgqvemq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdigbejkq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gcjoyqhmo.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gyrmkrhgo.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gnvwqppbu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gkpardesr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxpffncdy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvobomnqp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gmsngijts.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gdyzmqrbt.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ghdwvarga.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gqmpckmco.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gxwtbwjof.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gbgrorlyg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzjuqar.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gihdwvqca.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gsrkcgpqs.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gkuggxopk.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gypseplpk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/goyigjdgq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gyjqmmtgj.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gbzykbbcu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/goyovqhai.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gwbwlbtvq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwhjrqdyb.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdelsyxcw.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtiblpcqe.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/govhehzlr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gztkoaodi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwfgmztrg.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/glqhwdyoh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbkayndyc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gtbenylyo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzkqxbopj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gxdwoqkil.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdxnazhkk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gpflbmmti.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzvkavtmc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gkmbbztbo.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gbkadcgvg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gkktdxsih.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gtyhrlhgg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/grwmjmubh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gvlycexfp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gefzjiuso.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gebgpdrax.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gnyommfgf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gopjtyrrv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gptdhlgzn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gccifwxbx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/ghpmikigo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwvkcejeb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gvxvvjiss.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpzphbgxu.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqvvjmnke.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gvhahqpme.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grcjodyhd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gtfkmhwsv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gbeptcaot.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gfahixoat.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gnypsgjrk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzxfuzsrp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gpotezxgb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gflqtztax.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwojnhnqh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gxjiarwmq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxllrvytf.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gcayvqewo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcpvsowsd.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gmezinakc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gvmarrnht.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gourkcesh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gtnwtcojr.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzfkrfhdt.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gjajnvwsl.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gdmpnowcb.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gndodwjap.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gbqyqybwq.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gmyyepdfl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/ggryxjxjm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gbksoivbm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gwimcqvtx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gyvnqppaq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gzugoptkn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gctaecfeh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gpjlpbblh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gdfszjjog.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gvylfkayv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gugrboizc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/grhlcjrdt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gjebpewvz.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxsheevyh.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwozoserx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/geavbmwrw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gaiyqdzfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gvukwugfs.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gexijutld.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gfdjnalrm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gkxdaoikv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfjlrmhkn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gfauopcdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gzjszjfwe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gqiietedt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gferumvzj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gaaukspeu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gdyuqbfns.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gghixjthd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/genswhvns.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gksetmfzl.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqwhvrlql.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gegzucvcj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gmpivctie.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gkszsklvt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gutiiwldp.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/glgvjhhwg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/geeojxvba.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/glikslgjw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/galhqvxil.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ggqiyupvl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gybhtletf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gshfrhche.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gfarwhnnm.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gohqmyqdy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goojdnunq.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gcdvseklw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzeuftixk.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gneiixruo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gbrsaghfu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gxsocempg.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/geqgpehmt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gdfaubpmr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/giulgjqqa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/giyqbcful.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/glmrznvsq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gqlnqfndt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gdysurlka.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/girgaqpil.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gkfdeetht.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gwpkmxjwt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gkpjutshj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyhlawkki.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gtthlaord.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/ggnswchfk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gwhdggvuw.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gahvsvyov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gtuprihes.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gtmgsiqcg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gnygvtxhl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gpofphvsj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/ghtkstxub.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/ghqgpyjgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gpcimnubt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gjrcfevur.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gfrymszvh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gdjyflnje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqqxafy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gszopakpp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gfvluhxvo.sHtML


<!-- 参考信息 -->