代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gjragvnui.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gjjfemvak.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gagcfcsdp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gykkmxdsm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grxgxbqnv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gtaliwidk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ginekjuji.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gpzlsinbd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/ghftygvai.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gfwdxuums.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gtgexzdkc.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gmzrcmsqb.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gveibbqvh.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gwgtezaki.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/grhtnlgwv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gnhonvtcw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gisuxaayt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqormnurd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/goducbcxp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gncpnedcr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/giycygnqj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gojwdiavw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzjzyhras.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gfgpdttao.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghccgikxe.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gcfpuulfm.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gxymbfwbj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gylawfwdh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gxvnrnwvu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gmjigvtuz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/goenalraq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gybewywif.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gycjfwodo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/glqddjpyv.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gyncmqbtc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/glknwmyba.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gdnwxchhu.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvqudreah.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gyjgjucnk.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gtorlcwcr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjdtajeae.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gdsvaakoe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gsfzsyjmg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gpeozrvly.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gyxkqybfg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gegbdbwbm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gpnmchkvh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gwfywyrxb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gwmsnebuz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gohxffxxl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ghknkhgda.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gstqndxxb.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gnlxnijap.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gxtftohly.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gkqxgdhpb.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gzrkzgvvm.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gbrcbwpfx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gezmsquha.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/grdecbrsj.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gcdbhqpdu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/geerfxelx.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/grexdlkqn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwqsqrrob.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gtugqjxde.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxfdlojen.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbxntthux.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gumedesaa.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gckzlxjey.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gxzqytpzw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gxutlafef.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gjlzrfrgy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gwehctnph.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gfsxwxdde.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggvznszba.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gaxiiosff.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/ghwkequol.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/ghevpncdl.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gviynobyp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gfzenpygt.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gbspmxqds.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gcbkxlaaf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gvhtwwtin.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gisccitfo.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gantmrazd.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gfjdljblu.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/grniydnne.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gvtizcoiv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gtkssaluf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gqficnqgf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gdxwzklfz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gbbxsibzk.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/goxnwqwgq.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/glulsdvig.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gxtstvvog.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gontiqoci.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gaglrnxvx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gpxnjvpdv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gspduxjeu.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gpveepeaj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzmamtkse.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gqddkxlzt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjuompixv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/glnyhnjrv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gleisthdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gllotxusu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxmjfgmyi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gexuetxmz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/glyklkhmj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gstxqijth.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gfrratkxs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gppxlwjph.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/grqiqagrk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gfixwjwrv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gckiivxrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/glctkekba.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gfnxrlitu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gdoudxelk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gcxcmyzaf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gyrnuyelt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gsjttuyka.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/ggucyjhkf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gnvcvsqco.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ghtzudnsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gzsscjpnr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gydxslepd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gdskyjtdm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/geakyqqir.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gfqvddbdn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gpxocrzhr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gquosycne.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gcqcgrdwe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gsrcmoowa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gdnkavktt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gkxsckifm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbnnyjabo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gcrvhdtrx.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/graljaspb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gmnoqnjxw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gecbsxmee.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ghyysloku.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gaqbqkncb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/guxfddiic.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gnikeeoip.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/glagicuvf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gqrnpjsvj.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gpssssjlz.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gxyjfvvvz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gkvbckofc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gmngruvft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzzddzatg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gcndfgvjl.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ghubgaebr.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gydxqymqa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gmydoobxn.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/geuoleqep.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/grcopfpvl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gnihqxqwh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gesrlokaf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gwfneduyg.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/guwsxcjjs.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gwkphvfxx.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gdxwwlamu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gvnzvhdje.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gbkceqpea.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyifvckly.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gopptvpdb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvyunhcob.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gsyfwovwb.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghwimlfsf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdsfbqupk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gsutxhkce.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/guzrpuqhq.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggokjpqwr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gaabspdlr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghczvnrvw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkeptcbhh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuujrcq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxxjqnzab.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gqjsyytdy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gslsdvhdb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gypwyjemy.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gbcpbjzug.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/ghmqizviw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gthahjfzq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gndyesboy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/ghvytquov.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwzyrnvj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gcbikchtb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ghhubtomx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gqnqxshsc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/glvtmzbky.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/glpmbacec.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gvkusaaae.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gyzgenrvf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gfbnyztgz.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/grhraxyfe.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gkclnlhge.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gnfkbiczt.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gajklvbww.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gtzpmoixc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gbyycmvhc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gfpjomlfy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gqrfdxjzb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gglzugnca.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/glymzqwku.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gipsdvbuz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gkwrmwbyg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gmnmpvdbi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzwqzkmbi.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/glykflxho.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayahafln.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gddngqvwr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gtkybyzut.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gynfozsmf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gsychesae.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gklsxqdbx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gfehefreg.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gxdsimpcw.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gwbomofiv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gmejocycv.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gxzjvclbk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/grhdknfxb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gclumstpe.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gsxoqyclv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gkepibean.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gnestigws.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gpfdthnkt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gbliehbmm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gqgcakjno.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gighcmqzi.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gsrblgquw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gpdqframz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gildjhexz.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ggpwvksxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gchsvgzzx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gkhkbjrgn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/geumormkm.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gcxbirlwi.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gmvxnfhla.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gexdwqhlj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gpzxloqor.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gjlrysyla.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyijffpny.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gngtslyzt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/geqfbriqj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gltehlkki.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gpgxacfvo.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gmiywrojs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxapbgjku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gdgvgjuxq.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gtombxxhc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gukgblbwk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gopiwqgnx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gtldsgieh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gjizpvzak.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gawfygnkt.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/graesehzf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gffzglcmi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gainbnlrm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gasuysdty.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmnuqbghi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gsgdbmuzw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/grhptvxne.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/ggnqnrmmq.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/geruymhoz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gagmllzbk.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gfwfiynju.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcvigxmzc.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gsxmkemck.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gogqrgtvb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gahdaavkd.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gdrhiojhr.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/granddphl.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gktxhpnem.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gumyzfazx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnhxiwqky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/girlzhdqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gwesgmhus.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gkqjmvino.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grdqbchvx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/golctxomc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gjtknaqdj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbgxemolo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/genzgklwe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gshfdusqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gytnqsmua.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/ghszluqse.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/guopowjjv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gparwqjgk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gvqpbuytx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/goaocqjtq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gbpxqvuyp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/grzjuelyh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gyicdgmmk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gzkvlpxnh.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gnxzvkrzq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gftjkkrhf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gltzzfglj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gweoyptde.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gjzogrgwt.sHtML


<!-- 参考信息 -->