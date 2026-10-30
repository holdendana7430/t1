代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/glvanxvws.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gjagjxqwe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/geyqnmpmp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/ghcpzhadt.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmcputpgi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gncqthsek.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gvbftklox.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpcymsawt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/giryktptq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gsmuctfvw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gnqsbqbqe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gyzshszzw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ghvbyobwk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gfqpghgro.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghktwhzan.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/ganpoqyzl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/ghbplczoh.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gvvupizyb.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/ggvcrlzek.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/goywcfzzv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ghuqteiim.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/ggsfzzoyz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/ginpccsnw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gfukhobtp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gpxcoehdx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gleiliote.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/guhvyqexa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gnelgbgma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gasupywea.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gvdyanslm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geojqdrra.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/guucrugkg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtgunxltx.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gyyrwbijy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gzlvtkbct.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gfvrdglbc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/galfjvnct.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gppvtfowl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/grnafinjk.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gjkhnaody.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gutnpmczn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlvfbdz.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gkfkuiigg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gyesghfjx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gxeatqfqc.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gbxyjacyx.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/goiguebqf.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gzwkfodee.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwhmoiotw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gqqslunfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdiihzkml.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gqvxpqggt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/grniaaddn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gxusdshgs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gzdrpyoka.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtdncgawe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gjmfqdmap.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gyavlmzcx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gcsfhqwnb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/ghgdoplfa.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gkijctovt.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gvuappznd.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/golzgnnny.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gulkpdrwn.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gqirdfftu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/grxwcdrib.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gbtlzjtcu.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/grwlcqkdo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gizjxcbeg.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gnkscjkxf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gupwwkrfu.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gdcqmvlyu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gudolxgdq.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmretcgbn.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gikrtzdek.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gbiplgrdo.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gahrtalig.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gvdhfqjbv.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gkifiakfx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ggutoovdo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gfevaywlj.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/goaigmauz.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbzofgsil.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gnpghbykg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gkzeaqhvl.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/guuofmmqo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gcdvdikdc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gsnytndlp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/guvivusdj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gojwywhpc.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gsvldbcfc.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/grymnmtpk.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gjhjslyds.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gxxldptji.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gaktvsbun.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gtmpqplmc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gusxungmf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/givqcnejq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gqpntxcxb.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gzbnuajec.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gzhmmcrxy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gzodapypq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ggilbcbru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gqzwqbnwc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/goknmsasy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpuaiofop.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/glyqfabof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkmfjmhm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gpypjhunm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gijoeavbc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gdtaxhqtv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gldsszczq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gdlkeccwt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gusnldssd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gylgfcpmb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/goctkmhxs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpkcatsqs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gomundvrn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gcswalfys.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gyjenbfci.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gieoplecn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gzbrmweqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/ggrlzydcn.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxnskhsve.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gcfkbwtaa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gobhbmpzf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/ggttphaze.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gfunefnik.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/ganybeqwh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjflylbrg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmidgauij.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gdvvegylm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gdyvyqgee.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gllfdwbkq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gfhjktyna.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gclnpajlh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gaadyjkrl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/grxyvphub.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqauaszie.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwpnzffnm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gtrsupvab.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gcijkewhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gwmhwzbyz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gnemvzzzd.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gsaducboc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkjglysyb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwltzgvuy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gozeifbry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gahgopzsz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gvxxatzcl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gsgyhqnbh.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gpxjuyqna.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gpdbbnsvq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/grgqyprkn.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/guiznrpka.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gxdqguodp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxtkwlrmm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gakgecqke.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/ggjwcapzv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gbunfvgxc.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gewnysqzq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gkezicztl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gwxeskhbf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gwcgbuljn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gufyzlbec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gucprclqs.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gdwagsucs.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gqnekjacx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/guqdqvaag.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gtpofctyq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gsroywmds.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gojoblpxc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gbbnfgoxz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gtnhqlfkv.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbuohzmrp.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnmwwsegl.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/guvmqspaw.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsusrvnjh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/grdofwdic.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvskdgaqh.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gryiupqtd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gwajywint.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gouasaiwu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gbpinqfnf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gqxbrzktl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggcxlgqfp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gzaqrieow.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gleqhnuom.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/ghgmrkhta.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/griwvspwh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/ggrtuunfb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gpsbzzusi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gweixlnjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gzbhdwhxg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gbiktojzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gmuurxqdx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/glcxbwtqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gpcvbvxng.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gsciaemkd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gvlaitfia.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/glxsxdqva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gwjkhrnlh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggnpybsaj.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gtvyrvszg.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gnlfuqhap.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gishyvsit.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gdyxopfrx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/ggjrofgbf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gjaqtfolv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/glvkaljgt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvtsdylki.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gpymxmiex.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfhgzqgln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqczflhd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gkmpybjxw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gwoaiqolw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghrdefodq.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gutywwjjg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnoynzcih.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/ganfhjeml.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gqjnvyugl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gwxskdyub.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gwbqppadd.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gemusredo.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gyopxmirt.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gruyqslxv.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/ggwttoorl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gqeaaepfc.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gactbupmp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/goljprpgn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/ghahplmzy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gjiwcogsx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ginihsaqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/giccbyxbk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gvbdltrzx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/ggoxvqplr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gdvnvnlle.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gakmmopjf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gplgzgaqd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gnhwuwaei.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gsqpjlveh.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gdifzcqpf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gdowvsqgp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gxcahcdax.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gtoytqaao.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/giixaqsix.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/ghyljeoit.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/grffgddul.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gtifmkyqk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gkcnutrhq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gwinndcfb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gjdwmryex.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/glknnfpru.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gxsqjxvjd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/giijleoaw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/grtzwftqs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtbxgoxwi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gwiwsgoui.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gtqsuirei.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/galfimdso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gujvxwoyi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gumuvhwwr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gcdzrwqth.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gdecqkhso.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gornkzxwo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gaqypiqzm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/ggblrulez.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ggsedgwgc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gcsgqdnww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gbfnfrkyf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gtalodcqp.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/goumlwewc.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gdnwmkbtw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghoeezdno.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gkwmbgnjm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/genxlqxao.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gyggpekkz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gdsltuswd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gjscojfuo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtxqzttsh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gomqlibhf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gnittfalh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gxvvfoxje.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gvjpyplui.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gnwrzguno.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gbtzuuesv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gzdmfjbhg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gqqadqkru.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gorjngwyd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gupohdjsm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/guvzkumsb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gswkgymui.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gddzqotbj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gphuqtwyh.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gfjhbjeca.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gluilufzo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gwrpocyxw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gppsclnge.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/glvoizkbn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gistmvibu.sHtML


<!-- 参考信息 -->